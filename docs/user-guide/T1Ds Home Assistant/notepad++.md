<br>
[← Back to T1D Home Assistant Setup Guide](t1d_tts_setup_guide.md){ .md-button }

# Configuring Notepad++ for Home Assistant YAML

Using a local text editor like Notepad++ is a great way to manage your Home Assistant configuration files, but it handles formatting differently than Home Assistant itself. 

In Home Assistant, **literal Tab characters are forbidden**—it only accepts spaces. By default, Notepad++ often inserts a tab character when you press the Tab key, which can cause Home Assistant to throw configuration errors.

---

## 🛠️ How to Make Notepad++ Home Assistant Friendly

To configure Notepad++ so it automatically converts your tabs into the correct 2-space YAML format, follow these steps:<br>

1. Open Notepad++ and go to **Settings > Preferences**.

2. Click on **Indentation** in the sidebar menu.

3. In the language dropdown list at the top, select **YAML** (making sure your YAML settings are targeted).

4. Under the replacement options, select **Space character(s)** (this acts as "Replace by space").

5. Change the **Indent size** from `4` to `2`.

6. Ensure that **Tab character** is **NOT** selected.

Once you apply these settings, pressing the Tab key in Notepad++ will automatically type **2 real spaces** instead of a tab character, keeping your code cleanly aligned and ready for Home Assistant!

---


---

## 🛠️ How to Make Notepad++ Home Assistant Friendly

Home Assistant strictly requires **spaces instead of tab characters** for indentation. To make sure Notepad++ handles pasted text and indentation safely:

1. Open Notepad++ and go to **Settings** > **Preferences**.

2. Select **Indentation** from the left menu.

3. Select **yaml** from the language list.

4. Ensure **Space character(s)** is selected (instead of Tab character).

5. Set your **Indent size** (2 or 4 spaces are both supported).

6. Click **Close** to save your preferences.

---

## 2. Saving Your File Correctly

When saving your code snippet:
* Do not save it as a standard `.txt` file, as Home Assistant won't read it.
* Make sure to save the file extension explicitly as **`.yaml`** (for example: `configuration.yaml` or `automations.yaml`).
<br>

---

---

## Alternative: Using a Standard Text File & Quick Copy

If you prefer a simpler workflow without altering advanced preferences, you can use a standard text file and copy directly into Home Assistant:

1. Create or open a standard text file in Notepad++.
2. Paste or write your YAML code. **Crucial rule:** Avoid using the **Tab key** for spacing; ensure you use spaces instead.
3. Press **`Ctrl + A`** to select all, then **`Ctrl + C`** to copy the code.
4. Go to your Home Assistant UI editor, open the YAML editor view, and press **`Ctrl + V`** to paste it right in.

> **Note:** Even if the file remains a `.txt` format on your computer, Home Assistant will accept the code successfully as long as your spacing/indentation is clean and free of hidden tab characters.


---

## 3. Video Walkthrough

If you need a quick visual guide on managing code files and text editor setups, check out the video tutorial below:
<a href="https://youtu.be/DsLphWTte-U" target="_blank">
  <img width="1200" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/bfb7e553-da0a-454b-8a2d-4749340f0247" title="Resinchem Home Assistant 101 Terminology You Need to know"/></a>

If you need a great video guide on Home Assistant to setup and configuration from scratch, check out the tutorials on the [Resin Chem Tech YouTube Channel](https://www.youtube.com/@ResinChemTech/videos).
He has a lot more videos but Im trying to point you towards the ones that help me out!<br>

The other one is called: **DIY Standalone LED System V2: No external systems required!** which Id of like to have tried myslef, but I went for the Digquad instead, but be intresting to know if anyone as tried it ResinChems way too. 





[← Back to T1D Home Assistant Setup Guide](t1d_tts_setup_guide.md)















<!--  
  ******************************************************************************************************************
  
  UK Flag
*********************

  <img src="../../../assets/images/Flag_of_the_United_Kingdom_(3-5).svg" alt="UK Flag" width="24">


<img src="../../../assets/images/Flag_of_the_United_Kingdom_(3-5).svg" alt="UK Flag" style="width: 24px; height: auto;" />

******************************************

***********************************************
Hiding Pages from the Menu!

add in your t1d_tts_setup_guide.md
check out our dedicated :material-note-text: [note++ Guide](notepad++.md){ target="_blank" } 
*****************

Add to your Mkdocs.yaml file!
- 'Notepad++ Guide': 'user-guide/T1Ds Home Assistant/notepad++.md'
********************

with these links in your notepad++.md file you made! so it as a link back!

[← Back to T1D Home Assistant Setup Guide](t1d_tts_setup_guide.md){ .md-button }

[← Back to T1D Home Assistant Setup Guide](t1d_tts_setup_guide.md)

***********
you can also do it this way but I did not like the not_in_nav showing up!

- Hidden Pages:
    - not_in_nav:
        - 'notepad++': 'user-guide/T1Ds Home Assistant/notepad++.md'



*************************************
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

********************************************
Video Link making your own player with pngtree--video player line black icon
*********************************************************************************

<a href="https://youtu.be/DsLphWTte-U" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/554ad8ac-4b31-4534-a849-b8aae4f84b5a" title="Resinchem Home Assistant 101 Terminology You Need to know"/></a>


<a href="https://www.youtube.com/watch?v=DsLphWTte-U&t=41s" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/fb3ad56d-2792-4893-a1e4-62e00fe91801" title="Home Assistant 101 Terminology You Need to know"/></a>

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