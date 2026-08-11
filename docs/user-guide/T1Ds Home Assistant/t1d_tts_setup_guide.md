---
meta:
  - property: og:image
    content: "https://github.com/user-attachments/assets/e3471e96-c31e-4c09-aca2-d553cd4ceacd"
---
<!-- this is  on github server!
docs made by D.Galloway 2019- 2026-->


<div align="center">
  <img width="300" height="Auto" border="0" src="../../../assets/images/T1d TTS Setup Guide Logo.png" title="T1D tts Setup Guide">&emsp;&emsp;
  

  <h1 style="text-align: center;"><strong>T1D tts Setup Guide.md</strong></h1>






<h3 style="text-align: center;"><strong>📱 Setting Up T1D Glucose Text-to-Speech (TTS) Announcements)</strong></h3>
</div>



This setup guide walks you through configuring Home Assistant to read your Type 1 Diabetes (T1D) blood glucose levels and live trend directions out loud using text-to-speech (TTS) announcements.<br>

 Whether you pull your data via Nightscout or the official Dexcom mobile integration, this guide covers finding your notification targets, cleaning up your sensor readings into proper mmol/L values, building the automation script, and exposing it to voice assistants like Google Nest and Amazon Alexa devices.



<br>

<div align="center">
 <h1 style="text-align: center;"><strong>Coming Soon! in Sept 2026</strong></h1>
</div>

<br>

```yaml title="S24 Announce T1D Glucose Trend From App Dexcom"
alias: S24 Announce T1D Glucose Trend From App Dexcom
sequence:
  - delay: "00:00:01"
  - data:
      message: TTS
      data:
        tts_text: >-
          {% set bg = states('sensor.dexcom_g6_clean') | float(0) %}  {% set
          raw_trend = states('sensor.dave247_glucose_trend') %}  {% set
          trend_map = {
            'Flat': 'steady',
            'SingleUp': 'rising',
            'DoubleUp': 'rising quickly',
            'SingleDown': 'falling',
            'DoubleDown': 'falling quickly',
            'FortyFiveUp': 'rising slightly',
            'FortyFiveDown': 'falling slightly'
          } %}  {% set trend = trend_map.get(raw_trend, raw_trend) %}  Blood {{
          bg }} millimoles, and it is {{ trend }}.
        channel: alarm_stream_max
        ttl: 0
        priority: high
    action: notify.mobile_app_sm_s928b
mode: single
icon: mdi:waveform
description: ""
```




## 🌐 Step 1: How to Find Your Nightscout URL and APi Token

Before you begin, make sure your software is set up on both ends:

* You need a Nightscout web app installed and running in the cloud (you can set up a new user via the [Nightscout Heroku Guide](https://nightscout.github.io/vendors/heroku/new_user/)).

* You need Home Assistant up and running, and you can also check out the official [Home Assistant Nightscout Integration Documentation](https://www.home-assistant.io/integrations/nightscout) for more context.

### Important Note on Units (mg/dL vs. mmol/L)

When you first integrate Nightscout into Home Assistant natively, it usually comes in as **mg/dL** (for example, a reading like `132`). 
If you prefer or require **mmol/L** measurements, you can use a custom REST configuration in your YAML file to pull the data directly and convert it mathematically. Like we are doing here to adding your Rest Access Token. <br>

### Getting Your Parameters

Before connecting your data, you need your unique cloud parameters:

1. **Find your Nightscout Web URL:** Locate your main Nightscout cloud address (for example, `https://your-nightscout-site.herokuapp.com`).

2. **Find & Create your API Token:** You can easily create and manage your token directly from your Nightscout site using the **Admin Tools** 
(accessible by going too `/admin` on your Nightscout URL). 

<img src="../../../assets/Images/2026-08-04_15-02-41.png" width="800" alt="Find & Create your API Token" title="Find & Create your API Token">


3. Once logged in using your main site password, you can generate an API token with 
read permissions (often prefixed like `aaps-`) which goes into your Access Token part after you make it.

<img src="../../../assets/Images/2026-08-05_14-41-57.png" width="800" alt="generate an API token" title="generate an API token">

4. **Understand the API Endpoint Format:** The endpoint for pulling current entries requires appending the REST path: `/api/v1/entries/current.json?token=YOUR_ACCESS_TOKEN`.

5. **How to Put It Together:** Home Assistant needs the full web path to pull your live numbers. You take your web address, add `/api/v1/entries/current.json?token=` to the end of it, and paste your actual API token right after the equals sign (`=`).

6. Then you will need to add this into the Resource section, and place the code correctly into your configuration.yaml file in Home Assistant 
making sure to indent it correctly before you restart HA. 

7. You can test if the code is correctly  indented, before you restart by going to the Developer tools YAML and check configuration.

<img src="../../../assets/Images/2026-08-05_14-59-15.png" width="700" alt="Developer tools" title="Developer tools">
<br>

---

### Adding Your REST Code to Home Assistant

When adding this code into your Home Assistant `configuration.yaml` file, precision is key. 

* **YAML Indentation Matters:** YAML relies strictly on spaces (not tabs!). If your spaces are off, Home Assistant will fail to boot. 
* **Editor Tip:** If you edit files locally on your machine, make sure your text editor is configured properly to insert spaces instead of tab characters when you press the Tab key. For a complete walkthrough on how to set this up correctly, check out our dedicated <a href="../AndroidAPS/notepad++.md" target="_blank" rel="noopener noreferrer">Notepad++ Setup Guide</a>.

#### Test Before You Restart
You can verify if your code is correctly indented *before* restarting your server by going to **Developer Tools > YAML** in Home Assistant and clicking **Check Configuration**.

<center>
  <img src="../../../assets/Images/2026-08-05_14-59-15.png" width="700" alt="Developer tools" title="Developer tools">
</center>

#### Your Configuration Code Block
Add the following code block to your `configuration.yaml` file using your file editor:



8. To add your Rest code to your Home Assistant configuration.yaml file by using the File editor.<br>

```yaml title="Rest code for your Home Assistant configuration.yaml"
rest:
  - resource: "https://your-nightscout-site.herokuapp.com/api/v1/entries/current.json?token=YOUR_API_TOKEN"
    scan_interval: 60
    sensor:
      - name: "blood_sugar"
        unique_id: blood_sugar_original
        value_template: "{{ value_json[0].sgv }}"
        unit_of_measurement: "mg/dL"
      - name: "blood_sugar_2"
        unique_id: blood_sugar_2_fixed
        value_template: "{{ (value_json[0].sgv / 18) | round(1) }}"
        unit_of_measurement: "mmol/L"
      - name: "blood_sugar_delta"
        unique_id: blood_sugar_delta_fixed
        value_template: "{{ (value_json[0].delta / 18) | round(2) }}"
        unit_of_measurement: "mmol/L"
      - name: "Blood Sugar Trend"
        unique_id: blood_sugar_trend_fixed
        value_template: "{{ value_json[0].direction }}"
```
<br>

<img src="../../../assets/Images/2026-08-05_17-58-15.png" width="800" alt="configuration.yaml" title="configuration.yaml">

---

### Alternative Method: Dexcom Integration (Direct Mobile/Cloud Option)

If you use a Dexcom CGM (such as the G6 or G7) instead of Nightscout—or if you want a native option straight from your mobile app data—Home Assistant also features an official built-in **Dexcom Integration**.
You can check out the official [Home Assistant Dexcom Integration Documentation](https://www.home-assistant.io/integrations/dexcom){ target="_blank" } to connect your account directly

#### Prerequisites
* You must have the **Dexcom Share** feature enabled inside your Dexcom mobile app.


* 👉 Need help getting your Dexcom connected first? [Check out our Dexcom Follower & Share Setup Guide](../Dexcom/Dex%20Share%20Followers.md){ target="_blank" }



* Setting up Dexcom Share typically requires configuring at least one follower.

* Note: Home Assistant will log in using your primary **Dexcom account credentials**, not the follower credentials.

### How to Add It to Home Assistant

1. In Home Assistant, go to **Settings > Devices & services**.

2. In the bottom right corner, click the **Add Integration** button.

3. Search for and select **Dexcom** from the list.

4. Fill in your details on the setup screen:

    * **Username:** Your Dexcom account username, email address, or phone number (format phone numbers with a `+`, your country code, and then your number).
    * **Region:** Select your correct Dexcom Share API region endpoint (such as *US*, *Outside of US*, or *Japan*).
   
5. Complete the setup, and Home Assistant will automatically create live entities for your blood glucose values and trends.

### Cleaning Up Your Dexcom Readings

You'll also notice that the raw reading displays way too many decimal digits (for example, showing something like `9.93561278863233 mmol/L`). That’s why we're putting together this help file to show you how to clean up your G6 readings for a much tidier view before using them in scripts or automations.

<img src="../../../assets/Images/2026-08-05_18-34-34.png" width="300" alt="Dexcom Decimal Digits" title="Dexcom Decimal Digits">

#### How to Create a Clean Dexcom Template Sensor

1. In Home Assistant, navigate to **Settings > Devices & Services > Helpers**.

2. Click the **+ Create Helper** button in the bottom right corner.

3. Select **Template** from the list, and then choose **Template a sensor**.

<img src="../../../assets/Images/2026-08-05_20-43-54.png" width="300" alt="Template Helper Sensor" title="Template Helper Sensor">

4. Configure the fields with the following details:

   * **Name:** `Dexcom G6 Clean` (or a friendly name of your choice)
   * **State template:** Paste your exact code snippet:
     ```jinja
     {{ states('sensor.dave247_glucose_value') | float | round(1) }}
     ```
   💡 **Note:** Remember to replace `sensor.dave247_glucose_value` with your own sensor's actual entity ID.

   * **Unit of measurement:** `mmol/L`
   * **Device class:** `blood_glucose_concentration`
   * **State class:** `measurement`

<img src="../../../assets/Images/2026-08-05_19-34-01.png" width="500" alt="Template Sensor" title="Template Sensor">
   
5. Click **Submit** to create your new clean sensor.

Once saved, this creates a neat entity that displays a clean, rounded reading (like `7.2 mmol/L`), which is ready to be used smoothly in your scripts and read-outs!


***********************************************************

---

##  🔍 Step 2: Find Your Phone's Notification Entity Name

Every phone running the Home Assistant Companion App has a unique notification target named after its specific device model. To find yours:

   1. Open your Home Assistant dashboard.

   2. Navigate to **Developer Tools** from the sidebar.

   3. Click on the **Actions** tab at the top.

   4. Type `notify.mobile_app_` into the search bar.

   5. Review the dropdown list to locate your specific phone model (for example, `notify.mobile_app_sm_s928b`). Note down or copy this exact entity name.

   
   <center>
  <img width="800" height="auto" border="0" align="center" src="https://github.com/user-attachments/assets/cb356146-27bd-499c-abb2-e5699b3d9390" title="Mobile Notify Entity Name" />
</center>

   6. You now know your Mobile notification is ``` notify.mobile_app_sm_s928b```

   7. Go to Developer Tools (found in the sidebar of Home Assistant) and select the Actions tab (previously called Services).

   8. Under Action, search for and select notify.mobile_app_sm_s928b you just founnd.

   9. Then in  the message part  add ```TTS```

   10. Add your configuration payload into the **Data** section:

```yaml title="test_s24_tts" 
channel: alarm_stream_max
ttl: 0
priority: high
tts_text: "This is a test of the text to speech on the S24"
```
<br>
11. Click Perform Action
12. You should now hear the message spoken aloud from your mobile device if it is working correctly.
<br>
<div style="text-align: center;" markdown="1">
  <img width="800" src="https://github.com/user-attachments/assets/497249c6-3924-4db2-828b-d36fea1812a7" alt="Action Data section" />
</div>
  


---

### 🛠️ Troubleshooting

If you click "Perform Action" but nothing happens or you don't hear anything, check the following:

* **Phone Volume & Do Not Disturb:** Ensure your phone isn't on silent, media volume is turned up, and "Do Not Disturb" isn't blocking high-priority notification streams.
* **App Notification Settings:** Check your phone's system settings (**Settings > Apps > Home Assistant > Notifications**) and verify that notifications are fully allowed.
* **Battery Optimization:** On Android devices (like the S24), aggressive battery saving can put the Home Assistant companion app to sleep. Set the app's battery usage to **Unrestricted** or **Not optimized**.
* **Test a Basic Message First:** Remove the custom `data` YAML block entirely and try sending just a plain text message (`message: "Hello"`) to see if basic notifications are getting through to your device.

---

<br>

## 🛠️ Step 3: Create the Script in Home Assistant

 1. Go to **Settings** > **Automations & Scenes** > **Scripts**.

 2. Click **Add Script** in the bottom right corner, then select **Create Script**.

<center>
  <img width="800" height="auto" border="0" align="center" src="https://github.com/user-attachments/assets/9ad1d988-c32a-4471-8059-b615c8de91aa" title="Create New HA script" />
</center>

 3. Click the three vertical dots in the top right corner and choose **Edit in YAML**.

  

<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/b29a4ed5-241d-4771-8ae9-11bbb5bb0595" title="Edit in YAML"/></a><br><br>
   
4. Clear the existing code and paste the script template provided below.

---

## ⚙️ Step 4: Configure and Save the Script

















<div align="center">
  <img width="300" height="Auto" border="0" src="../../../assets/images/T1d TTS Setup Guide Logo.png" title="T1D tts Setup Guide">&emsp;&emsp;
  </div>



  <!--  
  ******************************************************************************************************************
  
  UK Flag
*********************

  <img src="../../../assets/images/Flag_of_the_United_Kingdom_(3-5).svg" alt="UK Flag" width="24">


<img src="../../../assets/images/Flag_of_the_United_Kingdom_(3-5).svg" alt="UK Flag" style="width: 24px; height: auto;" />

******************************************


  Facebook debugg
********************************


---
meta:
  - property: og:image
    content: "https://github.com/user-attachments/assets/7607c150-ee98-4f9b-97ff-abb894de6ba0"
---
  


---
meta:
  - property: og:image
    content: "https://github.com/user-attachments/assets/28413724-9144-4d82-8d46-7280865f2728"
---
  
  
  
  
  mkdocs.yml    # The configuration file.
    docs/
    index.md  # The documentation homepage.
       ...       # Other markdown pages, images and other files.
		
		*************************************************************************
		center text**
		## <center>Now Do  </center><br>
		
		*************************************************************
		
		
<a href="http://nightscout.github.io/pages/update-fork/" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="/img/Nightscout/Time to Update Nightscout.png" title="Update Tool"/></a>		
		

adding 	Green Hightligher!!!!!!!!	with bold too
<span style="background-color:#26AF06">**Choose Device**</span>


adding 	Yellow Hightligher!!!!!!!!	with bold too
<span style="background-color: #FFFF00">**Marked text**</span>

white space:

&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;


<a>
  <img width="auto" height="auto" border="0" align="center"  src="/img/Nightscout/Time to Update Nightscout.png" title="Update Tool"/></a>	

***********************
link
**********************

* 👉 Need help getting your Dexcom connected first? [Check out our Dexcom Follower & Share Setup Guide](../Dexcom/Dex%20Share%20Followers.md){ target="_blank" }


[test](../Dexcom/Dex%20Share%20Followers.md)

To make the link open in a new tab, add `{ target="_blank" }` right after the closing parenthesis of your link.

Here is the exact format to use:


markdown
[Your Link Text](../Folder-Name/file-name.md){ target="_blank" }


### Quick Documentation Cheat Sheet

*Save this snippet or note so you don't have to guess next time:*

**How to insert a local link that opens in a new tab:**

1. Type your bracket text: `[Click Here]()`
2. Inside the parentheses `()`, type `./` to open the Path Intellisense file picker.
3. Select your file (or type `../` to step up into parent folders).
4. Add `{ target="_blank" }` immediately after the closing parenthesis to make it open in a new tab.

**Final Result Example:**

```markdown
[Check out our guide](../Dexcom/Dex Share Followers.md){ target="_blank" }

```







<a href=" https://github.com/" target="_blank" title="First create a user account by going to">Click Here</a>


Adding a image with link
<a href="https://www.youtube.com/watch?v=MFsbm45b6YY" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="/img/Part 1 Setting up Github 2021/Github account details.jpg" title="github account details"/>
</a><br>

***************************************************************************************************************

Link with image size and external link in new tab also as description in it too...

[![Dexcom G6 Clean](../../assets/images/2026-08-05_19-08-53.png "Click to view the Dexcom follower setup guide"){ width="300" }](https://github.com/Atlas-Night-Out/T1DDiabetesHACard-App/blob/main/Docs/dexcom_follower_setup.md){ target="_blank" }



<a href="https://play.google.com/store/apps/details?id=com.dexcom.follow.region1.mmol" target="_blank"><img width="30" height="Auto" border="0" align="center" src="https://github.com/user-attachments/assets/7607c150-ee98-4f9b-97ff-abb894de6ba0" title="Dexcom Follow mmolL DXCM1"/></a>


*********************************************
Adds links to my Image files with the correct path

<div align="center">
  <img width="300" height="Auto" border="0" src="../../../assets/images/T1d TTS Setup Guide Logo.png" title="T1D tts Setup Guide">&emsp;&emsp;
  </div>

C:\Users\David Galloway\Visual-Studio-Code-Projects\Nightscout-xdrip-AAPS_2\Nightscout-xdrip-AAPS\docs\assets\images


******************
extern just a link
***************
link
<a href=" https://github.com/" target="_blank" title="First create a user account by going to">Click Here</a>

<a href="https://www.mongodb.com/cloud/atlas" target="_blank" title="Click Try Free">See Here</a> 

********************************
link to another page!
*************************

****************
Relative Link:
*******************
[HardwareDataSource](xdrip%20-%20hardwaredatasource.md)
[HardwareDataSource](xdrip%20-%20hardwaredatasource.md)

[What is AAPS](../AndroidAPS/What%20is%20AAPS.md)


# <center>Part 4: <a href="https://atlas-night-out.github.io/xdrip-Nightscout-AAPS/user-guide/Fork_and_Deploy_cgm_remote_monitory_part4/" target="_blank" title="Fork and Deploy cgm remote monitory Part 4">Fork and Deploy cgm remote monitory</a> </center>

********************************************************************************************
Adding Video
*******************************


## Visual Reference & Video Guide

Need a visual walkthrough? You can watch the official step-by-step guide video from Dexcom here:
* <a href="https://www.youtube.com/watch?v=uRzaL7mfUck" target="_blank" title="Click to watch the Dexcom guide on YouTube">Dexcom G6 - Setting up Dexcom Share and Follow on YouTube</a>



<iframe width="850" height="415" src="https://www.youtube.com/embed/MFsbm45b6YY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


Adding an embeded video
<iframe id="video3" width="560" height="315" src="https://www.youtube.com/embed/o7-T2IrDJ_A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


Video with image but this if a false Video!!!! And just and image with a link!
<a href="https://youtu.be/FZvuVlHOh8w" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/f44c325b-d1d0-483a-813b-bc45813f846a" title="Alexa - Jade - Skills & Games"/></a>



Note
**Note:** a note is something that needs to be mentioned but is apart from the context.

************************************************************************************************

Admonitions
*************************************


!!! note "Note: Once this connection is active, Home Assistant will be able to securely log into your Dexcom account and pull your real-time numbers."


This is a note with a drop down! you have to keep the format the same for it to work!!!!!!!!!!
??? info "Notes"

    Before proceeding, ensure that you've downloaded and installed all required applications on their respective devices. Once everything is set up, familiarize yourself with each app’s interface and functionality. <br> 


!!! Warning "Important Notice - This Video is a Old Way Watch with Caution"



??? Warning "Important Note - This Video is a Old Way to do it! Watch with Caution"

    This Xdrip+ Install 2019 video installation process is  old now and the video really needed to be updated, which I done now. But will be leaving on the site for reference sake only <br>

??? info "Notes"

    This Xdrip+ Install 2019 video installation process is  old now and the video really needed to be updated, which I done now. But will be leaving on the site for reference sake only <br>


****************************************************************************************

List
This is a regular paragraph.

Paragraph:

1. **Now Open another tab**  to make a Mongodb Atlas** Account: <a href="https://www.mongodb.com/cloud/atlas" target="_blank" title="Click Start Free">See Here</a> 
  and **click** Start Free
 <img width="auto" height="auto" border="0" align="center"  src="/img/Atlas/MongoDB Atlas start free.jpg"Click Start"/>
   2. Sub item two
   3. Sub item three
2. Item two



font size
<font size="4">

</font>

link
<a href=" https://github.com/" target="_blank" title="First create a user account by going to">Click Here</a>


Table
| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |


Video in a box border!

<table width="1166" border="1" style="border-color: #000000; background-color: #ffffff;" cellpadding="1" cellspacing="1" height="98">
<tbody>
<tr style="height: 16px;">
<td style="width: 1158px; border-color: #000000; background-color: #5B9BD5;" fff=""><span style="font-size: 14pt;"><span style="color: #ffffff;">video Instructions,</span></span></td>
</tr>
<tr style="height: 56.4063px;">
<td style="width: 1158px; border-color: #000000;"><span style="font-family: tahoma, arial, helvetica, sans-serif; font-size: 14pt;">
 <iframe id="video3" width="860" height="515" src="https://www.youtube.com/embed/6o3AdkQBVog" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>  </span></td>
</tr>
</tbody>
</table>
*****************************************************
Warning Note<table width="1266" border="1" style="border-color: #000000; background-color: #ffffff;" cellpadding="1" cellspacing="1" height="98">
<tbody>
<tr style="height: 16px;">
<td style="width: 1158px; border-color: #000000; background-color: #FF0000;" fff=""><span style="font-size: 14pt;"><strong><span style="color: #ffffff;">Warning!</span></strong></span></td>
</tr>
<tr style="height: 56.4063px;">
<td style="width: 1158px; border-color: #000000;"><span style="font-family: tahoma, arial, helvetica, sans-serif; font-size: 14pt;"> 1: Some new features, updates, or bug fixes may require that you clear your browser cache before you will see the changes taken effect<br/> 2: If you get no errors and no readings after a while see about doing a <a href="http://127.0.0.1:8000/user-guide/Redeploying%20your%20repository/" target="_blank" title="Redeploying your repository link">Redeploying your repository</a> </span></td>
</tr>
</tbody>
</table>

************************************************************************************
Subscribe
***************

new way with external link

<div align="center">
  <a href="https://www.youtube.com/channel/UC9TwtBefjjKw_uKHiIWMkBA?sub_confirmation=1" class="md-button" target="_blank" title="Subscribe to our YouTube Channel">Please Subscribe to our UTUBE Channel</a>
</div>

<br>


old way

[&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;]()
[Please Subscribe to our UTUBE Channel](https://www.youtube.com/channel/UC9TwtBefjjKw_uKHiIWMkBA?sub_confirmation=1){ .md-button }

-->

