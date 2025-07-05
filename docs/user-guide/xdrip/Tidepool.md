<!-- this is  on github server!
docs made by D.Galloway 2019- 2021-->


</a><img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/72fda25a-d629-402d-ba7e-e93fe0bc2806" title="Tidepool Original Logo"/></a></a><img width="450" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/4b5ab512-b7e7-418c-83e1-40929b34d60c" title="Tidepool "/></a>

# **Setting Up Tidepool** <br>



??? info "Intro"

    Key Offerings:<br>

    1.	Tidepool Platform – A free, cloud-based application that aggregates diabetes device data (from insulin pumps, CGMs, and glucose meters) into one easy-to-use dashboard.<br>

    2.	Tidepool Loop – An open-source automated insulin delivery (AID) system that helps people with diabetes manage insulin dosing more effectively.<br>

    3.	Big Data Donation Project – A program where users can anonymously donate their diabetes data to accelerate diabetes research.
 <br>

<br>

#### First Step:

You will need to choose first between what you want to use with Tidepool to connect to it.
There are several ways, but I will only be explaining two methods.<br>

Nightscout and Dexcom Clarity are the two main ones we need to setup first before we can connect to Tidepool.<br>

##### Step 1: Download the Dexcom Clarity App

:octicons-dot-fill-16: For Smartphones:<br>
:octicons-dot-fill-16: iOS (iPhone): Available on the <a href="https://apps.apple.com/gb/app/dexcom-clarity/id1019225730" target="_blank" title="Dexcom Clarity">App Store</a>.<br>
:octicons-dot-fill-16: Android: Available on <a href="https://play.google.com/store/apps/details?id=com.dexcom.clarity.mobile" target="_blank" title="Dexcom Clarity">Google Play</a>.<br>
:octicons-dot-fill-16: For Computers: Access via the <a href="https://clarity.dexcom.eu/" target="_blank" title="Dexcom Clarity">Dexcom Clarity Website</a>.<br>

##### Step 2: Create or Log in to Your Dexcom Account

:octicons-dot-fill-16: If you’re new to Nightscout, then visit <a href="https://nightscout.github.io/nightscout/platform/" target="_blank" title="Dexcom Clarity">Nightscout Docs Website</a><br>
:octicons-dot-fill-16: If you’re new to Dexcom, sign up for an account at <a href="https://clarity.dexcom.eu/" target="_blank" title="Dexcom Clarity">Dexcom Clarity Website</a>.<br>
:octicons-dot-fill-16: If you already have a Dexcom account (used for the Dexcom G6/G7 app), log in with the same credentials.<br>


##### Step 3: Connect Your Dexcom CGM

:octicons-dot-fill-16: If using the Dexcom G6/G7 app:<br>
:octicons-dot-fill-16: Clarity automatically syncs with your Dexcom CGM data if you’re logged into the same account.<br>
:octicons-dot-fill-16: If using a receiver or pump:<br>
:octicons-dot-fill-16: Manually upload data via the Clarity website (requires a USB connection). And for you to download their dexcom-uploader-4.6.0 software from Clarity Web site.<br>

<img width="auto" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/a9c0c6c3-24e6-4650-b8fd-9d02558b637e" title="Dexcom Uploader"/></a><br><br>


##### Step 4: Share Data (Optional)

:octicons-dot-fill-16: You can invite doctors, caregivers, or family members to view your reports:<br>
:fontawesome-solid-1: Go to "Share" in the Clarity app or website.<br>

<img width="700" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/5053bf60-613d-4143-bec2-ac97430c027d" title="Dexcom Clarity for Clinics"/></a>

:fontawesome-solid-2: Enter their email address.<br>
:fontawesome-solid-3: Choose their access level (view-only or full access)<br>

##### Step 5: View Reports & Insights

Dexcom Clarity provides:<br>

 ✔ Daily glucose trends<br>
 ✔ Time in Range (TIR) reports<br>
 ✔ Hypo/Hyperglycemia analysis<br>
 ✔ Average glucose & GMI (Glucose Management Indicator)<br>
Reports update every 3 hours when connected to your CGM<br>

<br>

#### Share Dexcom Data to Tidepool

To share Dexcom data with Tidepool, you need to connect your Dexcom Clarity account to your Tidepool account. <br>
This is done through the Tidepool Web interface and requires you to log into your Dexcom Clarity account within the Tidepool platform. Once connected, Tidepool will automatically fetch your Dexcom data. <br>

Here's a step-by-step guide: <br>

1.	Open Tidepool Web: Go to Visit<a href=" https://www.tidepool.org/" target="_blank" title="Visit tidepool.org"> tidepool.org</a><br>

2.	in a web browser (Chrome or Edge) and log in to your Tidepool account.<br>

2.	Connect a Device > Account: Navigate to the <span style="background-color:#26AF06">**“Devices”**</span> "Connect a Device Account" section.<br>
<img width="Auto" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/4384b779-9a32-409a-83f2-241ae8904f71" title="Connect a Device"/></a><br>

3.	Connect Dexcom: Click on the "Connect" button next to the Dexcom logo.<br>

<img width="auto" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/20af76ec-978b-4155-84fd-9960dfab60f8" title="Bring Data Into Tidepool "/></a><br>


4.	Dexcom Login: You'll be redirected to a Dexcom login page. Enter your Dexcom Clarity account credentials (username and password).<br>

5.	On my own setup I used Nightscout to connect to Tidepool and not Dexcoms, but it is done in the same manner<br>



<br>

!!! note "Getting Started"


If you have a Tidepool account, you can automatically upload your data and share it with your diabetologist ,endocrinologist.<br>
If xDrip+ can display basal information from an external source such as like AAPS or pump, it will also be uploaded to Tidepool.<br>

#### Step 1 - Sign Up with Tidepool

:octicons-dot-fill-16:	<a href=" https://www.tidepool.org/" target="_blank" title="Visit tidepool.org">Visit tidepool.org</a> <br>
:octicons-dot-fill-16:	Click "Personal Sign Up" or "Sign Up" <br>

<a href="https://www.tidepool.org/" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/55315183-22ec-4bde-b7ad-a2dea2ceebd5
  " title="github account details"/></a><br>

:octicons-dot-fill-16:	Enter your email and create a password <br>
:octicons-dot-fill-16:	Choose "Personal Account" and click "Continue" <br>

  <img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/3f334dfa-43cb-4f28-94e2-23d4552a44f1" title="Create Your Personal Tidepool Account
"/></a><br>

:octicons-dot-fill-16:	Fill out the patient information and accept the terms of use <br>
:octicons-dot-fill-16:	Verify your email via the link sent to you <br>
<br>

#### Step 2 – Enter your credentials into xDrip+

:octicons-dot-fill-16: Go to :material-menu: and select Settings <br>
:octicons-dot-fill-16: Go to Cloud Uploads <br>

  <img width="400" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/0001636f-e0cd-4bf8-83e2-415906bf3fae" title="Xdrip Cloud Upload"/></a> <br>

:octicons-dot-fill-16: Select Tidepool <br>

<img width="400" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/5d81acbf-33bf-4bee-8385-8bf06c125408" title="xDrp Tidepool"/></a> <br>

:fontawesome-solid-1: Turn on Sync to Tidepool <br>

<img width="400" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/d30c85dd-1f27-453d-abc1-cd12089d5fe4" title="1-2-3-4 Turn on Sync to Tidepool"/></a><br>

:fontawesome-solid-2: Enter the email address you used during registration <br>

:fontawesome-solid-3: and password you used during registration for Tidepool <br>

:fontawesome-solid-4: Test the connection once done. <br>
<br>

<br>
:fontawesome-solid-1: Avoid using test servers (keep unselected).<br>

<img width="400" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/5f88ec5d-2d8d-4c26-88d6-b17f839cc133" title="1.Avoid using test servers"/></a><br>

:fontawesome-solid-2: You may choose to upload under specific conditions to conserve battery life and minimize data usage costs.<br>

<img width="400" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/e082cd98-bd13-4e95-9059-227433b37d45" title="2. upload under specific conditions"/></a><br>

:fontawesome-solid-3: If you manually upload pump data, consider disabling xDrip+ treatment uploads to prevent duplicates.<br>

<img width="400" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/a07be38a-525a-4ed2-9778-7481efe56c5e" title="3. manually upload pump data"/></a><br>

:fontawesome-solid-4: If upload fails, enable the new authentication protocol.<br>

<img width="400" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/82501f51-b783-4504-9e69-f77531dd1801" title="4. If upload fails"/></a><br>

<br>

#### Step 3 - Enter credentials into AAPS

:octicons-dot-fill-16: Open the “:material-menu:” Gear menu in the top left and select “Config Builder” (or find it among the tabs at the top).<br>

<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/c2ecaebf-20ca-4f62-94f7-d487fdb00a3a" title="AAPS Config Builder"/></a>
<br>

:octicons-dot-fill-16: In the “Synchronization” section, check mark “Tidepool”.<br>

<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/9b63fa68-707f-44c6-810b-96add25646a7" title="Check Mark Tidepool"/></a><br>

:octicons-dot-fill-16: Click the :octicons-gear-16: gear icon next to “Tidepool”. <br>
:octicons-dot-fill-16: :fontawesome-solid-1: and :fontawesome-solid-2: Enter your username and password created in Step 1 for Tidepool.<br>

<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/13b2369c-010a-4ca2-981d-e1dda4091b16" title="AAPS Preferences 1-2-3"/></a>
<br>

:octicons-dot-fill-16: :fontawesome-solid-3: Click “Test Tidepool Login”.<br>

<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/5d91680c-0f0b-4d25-80e1-8e2ea8bbaae4" title="Test Tidepool Login"/></a><br>

:octicons-dot-fill-16: If you see “Successfully logged into Tidepool”, you’re connected. If not, verify your credentials and email address.<br>

:octicons-dot-fill-16: If You Don’t See the Success Message:<br>

:white_check_mark:  Verify Your Email & Password.<br>

:white_check_mark:  Ensure you’re using the exact email registered with Tidepool.<br>

:white_check_mark:  Check for typos or extra spaces in your password.<br>
<br>

:octicons-dot-fill-16: Now go to “Connection settings” and adjust according to your preferences.<br>

<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/994285ab-df91-4d83-a5ca-1103b88186e9" title="AAPS Connection settings"/></a><br>

:octicons-dot-fill-16: Thats all you need to do in AASP, If you need to setup a Nightscout <a href=" https://nightscout.github.io/nightscout/platform/" target="_blank" title="Nightscout">Click Here</a> . If you need any help on setting up Dexcom Clarity then see there Web site or call 0800 031 5763<br>
<br>

<a href="https://www.youtube.com/watch?v=Bg4msmy8vuo&t=40s" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/3dbc24ba-4885-49c0-9c7b-a0871662ae27
  " title="Tidepool in two minutes
"/></a>

<br><br>


### Upload Data 

Tidepool primarily syncs data automatically from supported devices (Dexcom, Omnipod, Medtronic, etc.), but you can also manually upload data from certain devices like blood glucose meters (BGMs) or older pumps.<br>

:pushpin: 📥 Supported Devices for Manual Upload <br>

:octicons-dot-fill-16: Blood Glucose Meters (BGMs) – OneTouch, Contour Next, Accu-Chek, etc.<br>

:octicons-dot-fill-16:Insulin Pens (if using a smart pen with exportable data).<br>

:octicons-dot-fill-16: Old Pump Data (if automatic sync isn’t supported).<br>

!!! note "Note"
:octicons-dot-fill-16:  Dexcom, Omnipod 5/Dash, and Tandem pumps sync automatically—no manual upload needed.<br>

#### :pushpin: Steps to Manually Upload

:octicons-dot-fill-16: Download from Tidepool site by selecting Upload Data <br>

<img width="auto" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/3e388aeb-56c0-4b5f-be24-aee1b8195adb" title="Upload Data"/></a><br>

:octicons-dot-fill-16: Download and install the Tidepool-Uploader-Setup-2.62.0 to your computer<br>

:octicons-dot-fill-16: Log in<br>

<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/59e1bc3a-b170-4667-808c-c9c6e3c95f2b" title="Tidepool-Uploader Log In"/></a><br>

:octicons-dot-fill-16: Plug your device into your computer with a USB lead<br>

<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/cb4f9bcd-4a7e-42bf-a00c-db6f5a4735cc" title="CONTOUR®NEXT"/></a> &emsp;&emsp;&emsp;&emsp;<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/afa39326-3967-466a-98f1-94c10fb5d266" title="Dexcom G6 Receiver"/></a>
<br>


:octicons-dot-fill-16: Select the upload button, related to your device type you are using.<br>

<center>
<img width="400" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/6002d74e-78b1-4c1b-a5a9-c23209d91de9" title="Tidepool-Uploader"/></a><br>

:pushpin: For more support on how to use your data once it is uploaded to Tidepool please visit: <a href=" https://www.tidepool.org/" target="_blank" title="Visit tidepool.org">Visit tidepool.org</a> </center>

<br><br>

<center>
## Also refer too: 

### [HardwareDataSource](xdrip%20-%20hardwaredatasource.md) <br><br> </center>

<br>

<br>

[&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;]()
[Please Subscribe to our UTUBE Channel](https://www.youtube.com/channel/UC9TwtBefjjKw_uKHiIWMkBA?sub_confirmation=1){ .md-button }

<br>
<a href="https://maundyrelief.org.uk/" target="_blank">
  <center><img width="300" height="auto" border="0" align=""  src="https://github.com/user-attachments/assets/585dd221-4f22-4e83-978d-3eedb39d3ca9" title="Maundy Relief"/></center></a>
<br>

<br>
<a href="https://www.diabetes.org.uk/" target="_blank">
<img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/21b87537-f1fa-4e01-904c-132085884544" title="Diabetes UK"/> </a>Why Not take visit <a href="https://www.diabetes.org.uk/support-us/fundraise/fundraising-events/pedal-for-progress" target="_blank"> :man_biking_tone1: UK Wide Cycle Ride - Diabetes.uk :woman_biking_tone5:</a> **or** <a href="https://swim22.diabetes.org.uk/?fbclid=IwAR3XSygKTkbU7l_Xgu88WU3Q3EYFrFoAj1STvQTVz_6X-xthmjqOUWMTiww" target="_blank">Diabetes.UK Swim22 :man_swimming_tone5:</a> **or** <a href="https://www.diabetes.org.uk/support-us/fundraise/fundraising-events/60-miles-challenge" target="_blank">:man_walking_tone5: Diabetes UK Month of Miles Challenge :woman_running:</a> for all of your Diabetes Needs!


<!--  
  ******************************************************************************************************************
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


<a>
  <img width="auto" height="auto" border="0" align="center"  src="/img/Nightscout/Time to Update Nightscout.png" title="Update Tool"/></a>	

link
<a href=" https://github.com/" target="_blank" title="First create a user account by going to">Click Here</a>


Adding a image with link
<a href="https://www.youtube.com/watch?v=MFsbm45b6YY" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="/img/Part 1 Setting up Github 2021/Github account details.jpg" title="github account details"/>
</a><br>

****************
Relative Link:
*******************
[HardwareDataSource](xdrip%20-%20hardwaredatasource.md)
[HardwareDataSource](xdrip%20-%20hardwaredatasource.md)

[What is AAPS](../AndroidAPS/What%20is%20AAPS.md)


Image link from Github:
<a href="https://www.tidepool.org/" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/55315183-22ec-4bde-b7ad-a2dea2ceebd5
  " title="github account details"/></a><br>

Adding Video

<iframe width="850" height="415" src="https://www.youtube.com/embed/MFsbm45b6YY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


Adding an embeded video
<iframe id="video3" width="560" height="315" src="https://www.youtube.com/embed/o7-T2IrDJ_A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Video with image but this if a false Video!!!! And just and image with a link!
<a href="https://youtu.be/FZvuVlHOh8w" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/f44c325b-d1d0-483a-813b-bc45813f846a" title="Alexa - Jade - Skills & Games"/></a>


*****************************
Big Heading
***********





*******************		
external link
******************

# <center>Part 4: <a href="https://atlas-night-out.github.io/xdrip-Nightscout-AAPS/user-guide/Fork_and_Deploy_cgm_remote_monitory_part4/" target="_blank" title="Fork and Deploy cgm remote monitory Part 4">Fork and Deploy cgm remote monitory</a> </center>

Adding Video

<iframe width="850" height="415" src="https://www.youtube.com/embed/MFsbm45b6YY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


Adding an embeded video
<iframe id="video3" width="560" height="315" src="https://www.youtube.com/embed/o7-T2IrDJ_A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


Video with image but this if a false Video!!!! And just and image with a link!
<a href="https://youtu.be/FZvuVlHOh8w" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/f44c325b-d1d0-483a-813b-bc45813f846a" title="Alexa - Jade - Skills & Games"/></a>


Note
**Note:** a note is something that needs to be mentioned but is apart from the context.


???+ note "Note"

This is a note with a drop down! you have to keep the format the same for it to work!!!!!!!!!!
??? info "Notes"

    Before proceeding, ensure that you've downloaded and installed all required applications on their respective devices. Once everything is set up, familiarize yourself with each app’s interface and functionality. <br> 


!!! Warning "Important Notice - This Video is a Old Way Watch with Caution"

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

-->

