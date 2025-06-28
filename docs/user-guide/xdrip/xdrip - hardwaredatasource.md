<!-- this is not on github server its local only and run my mkdocs server!
docs made by Tunasalad 2019- 2021-->
<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/c0b76e2f-d6eb-4a2d-9adf-e58b966cbae7" title="Hardware Data Source Header"/></a>
<br>

### [Xdrip+ Settings](Settings.md#settings)
### [xdrip± Specifications](Settings.md#specifications)
### [xdrip± Hardware Data Source](Settings.md#6-xdrip--hardware-data-source) 

<img width="400" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/92a803ba-ebcb-48fb-af8a-e10c104544ab" title="Choose Data Source"/></a> If you don't see this on installing!<br>

This is where you will be selecting your Hardware Data Source to work with xdrip.<br><br><br>


!!! note "Note"

<br>
In xDrip+, the Hardware Data Source is the setting that determines where your glucose data comes from. Here are the common options available, depending on your setup:<br>

I mostly Use Dexcom G7/G6/1/1+ (Transmitter) when I'm using a Dexcom One and Companion App for when I'm using the Dexcom G6<br> both of these options work in AAPS and my Galaxy Watch 7.<br>

To get to the settiings for it, by going to :material-menu: hamberger Menu > <span style="background-color:#26AF06">**Settings**</span> > <span style="background-color:#26AF06">**Hardware Data Source**</span><br>

<br>

<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/2f3bd557-f522-4294-a76b-798dd43255fd" title="Hardware Data Source G6-G7-1-1plus and Stelo"/></a><br>

<br>

You will need to pick a Hardware Data source to add into xDrip for your CGM to get readings. Take a look below to see  what might suit you on your setup you have, and then follow on from on from [Start Source Setup Wizard](#start-source-setup-wizard) below<br>



### Common Hardware Data Sources 

1. Dexcom G6/G7/1/1+ (Transmitter)<br>
&emsp;&emsp; :octicons-dot-fill-16:  Directly connects to Dexcom G6/G7/1/1+  transmitters via Bluetooth (no need for a separate receiver).<br>
&emsp;&emsp; :octicons-dot-fill-16:  Requires the official Dexcom transmitter or compatible third-party solutions.<br>

2. Libre Sensors (via Bluetooth Bridge)<br>
&emsp;&emsp; :octicons-dot-fill-16:	Libre 1 (14-day): Requires a Bluetooth bridge like BlueReader, MiaoMiao, or Bubble.<br>
&emsp;&emsp; :octicons-dot-fill-16:  Libre 2 (EU/US): Can work directly via Bluetooth (no bridge needed in some regions).<br>
&emsp;&emsp; :octicons-dot-fill-16:  Libre 3: Fully Bluetooth-enabled (direct connection to xDrip+ in some versions).<br>

3. Nightscout (as a Web Source)
&emsp;&emsp; :octicons-dot-fill-16:  Fetches data from a Nightscout site (if another device is uploading data there).<br>

4. Dexcom Share (for Follower)<br>
&emsp;&emsp; :octicons-dot-fill-16:  Pulls data from Dexcom's cloud servers (if using Dexcom Share with a receiver or phone app).<br>

5. Companion App<br>
&emsp;&emsp; :octicons-dot-fill-16:  G6/G7 (master only) apps.<br>
&emsp;&emsp; :octicons-dot-fill-16:  CamAPS app <br>
&emsp;&emsp; :octicons-dot-fill-16:  Omnipod 5 app <br>
&emsp;&emsp; :octicons-dot-fill-16:  Eversense apps <br>

<br>

### **G7,G6,Dex1,1+ and Stelo** <br>

If you connect xDrip+ directly to your sensor (G7, G6, 1, 1+, and Stelo), you will lose access to the suppliers app and Clarity uploads. However, you can use Nightscout or Tidepool.<br>

Sharing via share servers may still work if set up initially with supplier’s apps, I don’t think Dexcom One has a Sharing App, but Nightscout could still be used.


<img width="Auto" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/3913299d-3eca-43b1-ad5c-c7ee704e6f3b" title="Hardware Data Source G7-G6-Dex1-1+ and Stelo"/></a><br>


=== "🔄 G7, G6, 1, 1+ or Stelo"
``` mermaid
graph LR
  A[G6,G7,1,1+ or Stelo] --> |Bluetooth| B[xDrip+];
  B -->|Commands| C[AAPS App];
  C --> D[Pump or Omnipod Dash];
  B --> |Cannot| E[Upload to Clarity];
  E --> |Can upload to|F[Nightscout, or Tidepool];
```

<br>

### **G6, G7, 1+** <br>
 
If you use the supplier’s (G6, G7, 1+), you can connect xDrip+ as a Share follower as long as a follower has been setup with the supplier’s (vendor). You can do this, by setting up [Dex Share Follower](../Dexcom/Dex%20Share%20Followers.md) and setting up a  Dexcom G6 App (Share)

But to use a Dexcom One you will need to use Nightscout.<br>

<img width="Auto" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/9e77914b-197e-43a1-9eae-b821fd6a2f9f" title="Hardware Data Source G6, G7,1+ Flowchart"/></a><br>

=== "🔄 G7, G6, 1+ "
``` mermaid
graph LR
  A[G6,G7,1+] --> |Bluetooth| B[xDrip+];
  B <-->|Can| C[AAPS App];
  C --> D[Pump or Omnipod Dash];
  B --> |Can| E[Upload to Clarity];
  E --> |Can upload to|F[Nightscout, or Tidepool];
```
<br>

### **G6 only** <br>

When using BYODA (G6 only) if you've enabled Broadcast to xDrip+ you don't need a network connection to have data in xDrip+. Use the 640G/Eversense data source
<br>
<br>

## **Start Source Setup Wizard**

You will need to go to choose your Data Source, for your setup.
And to add this you should have a Start Source Setup Wizard on your main screen at the bottom of your screen from when you installed xDrip+ or <br>

 Go to your  :material-menu: Gear at top left! > Settings > Hardware Data Source<br>

<center>
<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/c5f43f30-779e-41d2-abbe-2ba0dea46fbb" title="Start Source Setup Wizard"/></a></center>
<br>

If you do not have one of these at the bottom of your screen in xdrip+ you have two options one is to do a long press on the xdrip+ image at the top of your main screen :drop_of_blood:<br>
<center>
<img width="400" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/836b64bb-3a0d-4151-81e4-2b7222ae8bcc" title="xDrip+ ImageBlood"/></a></center>
<br>

And turn on your Source Wizard Button.<br>
<center>
<img width="400" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/25906db8-10b4-49d4-9581-143a22622925" title="Source Wizard Button"/></a></center>
<br>
To be able to select you Data Source, but Like I said above, if you do not see yours then <br>

 Go to  :material-menu: Gear at top left > Settings > Hardware Data Source <br>

### ScreenCast Video: Example on how to add a Hardware Data Source


 <a href="https://app.screencast.com/auVVGHgrXsial" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/1c28d34e-800c-4728-93be-37f242de2d1c" title="Hardware Data Source video"/></a>
  <br>


### UTUBE Video: Example on how to add a Hardware Data Source

  <a href="https://youtu.be/5Mh-tl7_yPo" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/1c28d34e-800c-4728-93be-37f242de2d1c" title="Hardware Data Source video on Utube"/></a>
  <br>

<br>


You will see a long list of Hardware Data Source options to choose from. <br>

In this example I will be showing on how to add a Dexcom G6 with  using Companion App  <br>

<img width="250" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/a065a7c4-7c5f-42a0-8f25-607e3f7a87d3" title="Hardware Data Source List 1/2"/></a> &emsp;&emsp;<img width="250" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/07725ac5-88b7-47a8-80b9-f401f19a303c" title="Hardware Data Source List 2"/></a> <Br>
<br>

#### Make sure to Unpair your mobile

!!! Warning "Warning! Do not use your mobiles bluetooth connection"

Do not use your Mobiles auto Bluetooth connection to pair your Transmitter! If it does connect, unpair it from your phone first, before you begin to use xdrip+ has it will ask you to do it on its setup when adding Hardware Data Source! <a href="https://www.youtube.com/shorts/YVy_qxeHpog" target="_blank" title="Dexcom USA Account">See Here</a> <a href="https://clarity.dexcom.eu/" target="_blank" title="Bluetooth connection"> </a><br>

<br>

Unpair if already connected.<br>

<center><img width="250" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/d729f9a8-81d3-4b7a-b043-fd0e0524649c" title="Bluetooth Unpair"/></a> &emsp;&emsp;<img width="250" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/18c7bc21-77f4-41d6-a118-2fc7c81216bc
" title="Dexcom unpair"/></a></a></center><br>

!!! note "Info! &emsp;&emsp;  "

Sensors and Transmitters can only connect to one Mobile (or tablet) at a time, and only to one app at a time. There are ways around this, that will allow you to connect to other software packages like Android APS!<br>

I will not be going into that now though.<br>


<br>

#### Sensor Start Pairing Request:

You, should be getting Bluetooth Pairing request from when you Start your Sensor in xDrip+ unless you are using Companion App and then you will need to Start it from that vendors App.<br>

In my case Dexcom G6 App, <img width="30" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/a029ff04-61a8-4eb0-ba00-0acd214b7c04" title="Dexcom Follow mmolL DXCM1"/></a> but I have a Dexcom Receiver too, so I use that instead of within the Dexcom G6 mmol/L DXCM1 App <img width="30" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/a029ff04-61a8-4eb0-ba00-0acd214b7c04" title="Dexcom Follow mmolL DXCM1"/></a>(Android). If you do  not already have it <Br>
installed, <a href="https://play.google.com/store/apps/details?id=com.dexcom.follow.region1.mmol" target="_blank" title="Dexcom Follow mmol/L DXCM1">Click Here</a><br>

<img width="250" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/7d268930-2b40-4f12-ae06-895b2f849937" title="Bluetooth Pairing Request"/></a>

<br>


[*Last modified now*](https://github.com/NightscoutFoundation/xDrip/releases)

<br>


<center>
[Please Subscribe to our Utube Channel](https://www.youtube.com/channel/UC9TwtBefjjKw_uKHiIWMkBA?sub_confirmation=1){ .md-button } </center><br><br>


<a href="https://maundyrelief.org.uk/" target="_blank">
 <center> <img width="300" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/585dd221-4f22-4e83-978d-3eedb39d3ca9" title="Maundy Relief"/>

<br>
<a href="https://www.diabetes.org.uk/" target="_blank">
 <center> <img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/21b87537-f1fa-4e01-904c-132085884544" title="Diabetes UK"/>
</a>               Why Not take visit <a href="https://www.diabetes.org.uk/support-us/fundraise/fundraising-events/pedal-for-progress" target="_blank">  :man_biking_tone1:UK Wide Cycle Ride - Diabetes.uk :woman_biking_tone5:</a> **or** <a href="https://swim22.diabetes.org.uk/?fbclid=IwAR3XSygKTkbU7l_Xgu88WU3Q3EYFrFoAj1STvQTVz_6X-xthmjqOUWMTiww" target="_blank">Diabetes.UK Swim22 :man_swimming_tone5:</a> **or** <a href="https://www.diabetes.org.uk/support-us/fundraise/fundraising-events/60-miles-challenge" target="_blank">:man_walking_tone5: Diabetes UK Month of Miles Challenge :woman_running:</a> for all of your Diabetes Needs!
</center>



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


white space:

&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;



link
<a href=" https://github.com/" target="_blank" title="First create a user account by going to">Click Here</a>

Adding a image with link
<a href="https://www.youtube.com/watch?v=MFsbm45b6YY" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="/img/Part 1 Setting up Github 2021/Github account details.jpg" title="github account details"/>
</a><br>


Adding Video

<iframe width="850" height="415" src="https://www.youtube.com/embed/MFsbm45b6YY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


Adding an embeded video
<iframe id="video3" width="560" height="315" src="https://www.youtube.com/embed/o7-T2IrDJ_A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


Note
**Note:** a note is something that needs to be mentioned but is apart from the context.


This is a note with a drop down! you have to keep the format the same for it to work!!!!!!!!!!
??? info "Notes"

    Before proceeding, ensure that you've downloaded and installed all required applications on their respective devices. Once everything is set up, familiarize yourself with each app’s interface and functionality. <br> 


???+ note "Note"       dropdown!

!!! note "Note"         normal!

!!! Warning "Important Notice - This Video is a Old Way Watch with Caution"

*****************************************
white space:

&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

List
This is a regular paragraph.

Paragraph:

1. **Now Open another tab**  to make a Mongodb Atlas** Account: <a href="https://www.mongodb.com/cloud/atlas" target="_blank" title="Click Start Free">See Here</a> 
  and **click** Start Free
 <img width="auto" height="auto" border="0" align="center"  src="/img/Atlas/MongoDB Atlas start free.jpg"Click Start"/>
   2. Sub item two
   3. Sub item three
2. Item two


Big Header:

# **Install xDrip+** <br>


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