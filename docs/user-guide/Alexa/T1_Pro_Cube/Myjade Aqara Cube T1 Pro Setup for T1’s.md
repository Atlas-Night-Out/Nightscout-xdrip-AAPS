<center><img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/6debd03a-8066-4b23-85c8-154d1fe8e282" title="T1 Pro Cube"/></a></center><br>

!!! Warning "Important Notice - The video below shows the old way we used to get readings read out to us with Sugarmate, which Ceased  to work in Feb 2025"
<a href="https://www.youtube.com/watch?v=bTc6qBVb9d4" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/11905f15-ab17-4bf2-9ee9-8f618b9505c3" title="T1 pro Cube Reads out Glucose"/></a>
  
<br>

!!! note "Note - Jade is the new way now in 2025 to have your reading read out to you!"
### Jade the new way now in 2025!
<a href="https://www.youtube.com/watch?v=za9m8ZiOY80" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/7ea298cb-250f-47a4-878f-2fbf21371be3" title="My Jade Aqara Cube T1 Pro Setup for T1’s to Echo Show"/></a>


## Short Intro
The Aqara T1 Pro Cube is a sleek, smart home controller that interacts with your devices through gestures, rotations, and taps. Here's a quick intro to its key features and setup:
The Aqara T1 Pro Cube is a highly efficient device designed to provide glucose readings by responding to specific dice number positions. This versatile device not only aids in monitoring blood sugar levels but also offers home automation capabilities.<br>

Additionally, the presence sensors or motion detectors enable the automatic reading of glucose levels at any location within your home.
The Aqara T1 Pro Cube is a sophisticated smart home controller that interfaces with various devices through gestures, rotations, and taps. Below is an overview of its primary features and setup process:<br>

Key Features <br>
✅ Six Gestures: Shake, rotate, flip, push, slide, and tap for different controls.<br>
✅ 360° Rotation: Adjust lights, thermostats, or volume by turning the cube.<br>
✅ Smart Home Hub Compatible: Works with Aqara Hub, Apple HomeKit, Google Home, and Amazon Alexa.<br>
✅ Wireless & Battery-Powered: Uses a CR2450 coin cell battery (lasts ~2 years).<br>
✅ Customizable Controls: Assign actions in the Aqara Home or Apple Home app.<br>

<br>
!!! Warning "Important Notice"
Sadly, Sugarmate is no longer doing there App now January ,1 2025, for it to work in Amazon Alexa App to have your Blood readings read out with Automations. Since when I wrote these setups up last year, so I will have to re check on my setups to change them due me having me Finding an alternative now called My jade which is a good replacement, in 2025<br>

!!! note "Notes"

My Jade has kindly done a New Alexa-Only Plan for SugarMate Users due to me asking them to help us all out.
We’ve heard that SugarMate has removed their Alexa integration, making life harder for vision-impaired users. So, we’re stepping in with a simple, affordable Alexa-only plan!<br>

This plan will announce your blood sugar levels through Alexa for a <a href="https://store.payproglobal.com/checkout?products%5b1%5d%5bid%5d=107441" target="_blank" title="MyJade Subscription">Click Here</a>

<a href="https://store.payproglobal.com/checkout?products%5b1%5d%5bid%5d=107441" target="_blank">
  <img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/7235c814-da14-4b41-97a1-7683cefdd419" title="My Jade Offer"/></a>

</a><br>

I will be trying to help you set up an Echo Show 10 (3rd Gen) or an Echo Dot or a Samsung Tablet. So that , it will read out your Glucose readings. I will not be going through and explaining the unboxing as this as been done in other videos.<br>


<br>

## Hardware Items you are going to need

Due to me setting up on a PC computer and not a Mac, I did not have any Apple Items to use Homekit to get into Home Assistant has I wanted too, so to get around this I got a HomePod Mini. So you Harware needs may vary to mine! <br>


1.	<a href="https://www.amazon.co.uk/dp/B0BHWS3VTZ?maas=maas_adg_F2E7A71BEAD7E7012F8DA4528E905764_afap_abs&linkCode=sl1&tag=paulhibbert-21&linkId=17f5a99c41bcb0d2cd1cdd6c378794b3&language=en_GB&ref_=as_li_ss_tl" target="_blank" title="Aqara Cube T1 Pro">Aqara Cube T1 Pro</a>   (Also REQUIRES AQARA ZIGBEE 3.0 HUB)
2.	<a href="https://www.amazon.co.uk/dp/B09BJCNCKM?psc=1&ref=ppx_yo2ov_dt_b_product_details" target="_blank" title="Aqara Smart Hub">Aqara Smart Hub E1</a> Aqara Smart Hub E1 (2.4 GHz Wi-Fi Required)
3.	<a href="https://www.amazon.co.uk/dp/B084P3KP2R?psc=1&ref=ppx_yo2ov_dt_b_product_details" target="_blank" title="Echo Show 10">Echo Show 10 (3rd generation)</a> or an <a href="https://www.amazon.co.uk/gp/product/B09B96TG33/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1" target="_blank" title="Echo Dot">Echo Dot </a> (5th generation, 2022 release) Or your Samsung Mobile or Tablet
4.	Android Mobile Device in my case a <a href="https://www.amazon.co.uk/gp/product/B07W6XFX64/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1" target="_blank" title="Samsung Note10 +">(Samsung Note10 + But I have also tested on S24 Ultra and S25 Ultra and still works)</a> 
5. Apple HomePod Mini <a href="https://www.apple.com/uk/shop/buy-homepod/homepod-mini" target="_blank" title="HomePod Mini">(HomePod Mini)</a>
 <br>

## Software you will need to have Setup

1.	[Nightscout](../../Nightscout/Setting_up_Github_Account_part1.md#part-1-setting-up-the-github-for-nightscout)
(Which I will not be showing you how to setup in these instructions) But will add a link for you to do it if you have not done so already 
<br>
3.	<a href="https://www.jadediabetes.com/index.html" target="_blank" title="My Jade">My Jade</a>  on a  PC (You will need to sign up)
4.	<a href="https://store.payproglobal.com/checkout?products%5b1%5d%5bid%5d=107441" target="_blank" title="Jade Alexa-Only Plan">Jade Alexa-Only Plan</a>  -  subscription Plan for the year
5.	<a href="https://play.google.com/store/apps/details?id=com.managebgl.predictbgl2" target="_blank" title="Jade Insulin Dose Calculator APP">Jade Insulin Dose Calculator APP</a>  On a Mobile
6.	<a href="https://play.google.com/store/apps/details?id=com.amazon.dee.app&hl=en" target="_blank" title="Amazon Alexa App">Amazon Alexa App</a> 
<br> with an Amazon Account

7.	<a href="https://atlas-night-out.github.io/xdrip-Nightscout-AAPS/user-guide/xdrip/xdrip%20-%20Download/" target="_blank" title="Xdrip">Xdrip</a> (Not needed) if bringing in from another Data Source, But I'm using Nightscout on this setup, so xdrip is needed.
8.	<a href="https://aiot-management.aqara.cn/config/app/aqaraHomeDeveloping" target="_blank" title="Aqara Home">Aqara Home</a>  App
9. <a href="https://www.amazon.co.uk/My-Jade-by-Diabetes/dp/B09YT3VM85?crid=7QCKHXCTLNFE&dib=eyJ2IjoiMSJ9.qh-W7YnlNqBcSfbdJCnJmQ.cN7kltCrJJbqhPwgZNw2EYXpIJV7Y5lePUUzaHAgxqI&dib_tag=se&keywords=sugarmate+app&qid=1722075367&s=digital-skills&sprefix=sugarmate%2Calexa-skills%2C68&sr=1-1" target="_blank" title="My Jade by Jade Diabetes">My Jade by Jade Diabetes</a>  App on Amazon. You will need to enable the Skill
<br>

### General Quick Setup Guide
1.	Pair with Aqara Hub E1 (or compatible hub like Apple HomeKit).
3.	Open the Aqara Home app → Add device → Follow prompts.
4.	Assign Actions: Map gestures to scenes (e.g., flip to turn off lights, rotate to dim).


### My Quick Setup Guide
#### Add E1 Hub Device
1.	First download the Aqara Home app.
Search for "Aqara Home" in the Apple App Store, or Google Play,
Xiaomi Get Apps, Huawei App Gallery, or scan the following QR code to download the Aqara Home App:<br>
<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/1350bde6-8fce-4ccc-a51e-d935a2ac58e6" title="Aqara Barcode"/></a>
<br>

2.	An Aqara Zigbee 3.0 hub is required. Please make sure
you have an <a href="https://www.amazon.co.uk/dp/B09BJCNCKM?psc=1&ref=ppx_yo2ov_dt_b_product_details" target="_blank" title="Aqara Smart Hub">Aqara Smart Hub E1</a> installed and added to
your Aqara Home App<br>

## Setting up the E1 Hub 
<center><img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/cbb3f564-7f59-4a3c-8b68-6904fb776ac6" title="E1 USB Hub"/></a></center>

1. Plug the hub into a USB port that can provide power, wait for the yellow indicator to flash quickly, and make sure your mobile phone is connected to a Wi-Fi network in the 2.4 GHz frequency band. <br>
You will need to make sure your home router is set to a 2.4 ghz bands until you are setup with your hub and T1 Pro, you may turn it back to Auto 5GHz after the setup, All routers will be different on how to do this process, so see your Routers Manual.<br>
<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/77c03546-5c25-4d99-b8fa-c32f34122bab" title="Virgin Router Settings"/></a><br><br>
keep the mobile phone as close to the hub as possible, and your mobile phone and hub are using the same Wi-Fi network.<br>

2. Open the Aqara Home app, click the <span style="background-color:#26AF06">**+**</span> in the upper right corner of the home page, select <span style="background-color:#26AF06">**Hub E1**</span>, from  <span style="background-color:#26AF06">**Add Accessory - Gateway/Hub E1**</span> and follow the instructions of the app to operate.<br><br>
1 <img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/c263bd2a-27bb-4a0f-b308-58beb3977d8d" title="Add Accessory"/></a>
2 <img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/1c6d9e0a-e46f-4437-89a5-87a52a2e6bb6" title="Gateway_Hub E1"/></a>
<br><br>
3 <img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/96925891-d75f-4608-b023-ad5ae6fe5495" title="Add Hub E1"/></a>
4 <img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/ac6f9254-4aab-4205-b175-5645265df0d3" title="Scan the Device "/></a><br>
5.	If the addition fails, please long press the hub button for 10s to reset the network, and then add it again in the app.<br>
6. Once the E1 Hub is connected you can now connect the T1 Pro Cube.<br>

<iframe width="392" height="397" src="https://www.youtube.com/embed/6WkQg_FvaU8" title="Connecting to Aqara E1 Hub after changing Router to a 2 4ghz" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe><br>

## Adding Battery <br>

Open the battery cover of Cube T1 Pro with the ejector tool, take out the battery, replace it with a new <a href=" https://www.amazon.co.uk/LiCB-CR2450-2450-Lithium-Battery/dp/B07V3BQQ76?pd_rd_w=yAQZF&content-id=amzn1.sym.f38095c9-5676-4cd8-8e43-7b80039d1ac3&pf_rd_p=f38095c9-5676-4cd8-8e43-7b80039d1ac3&pf_rd_r=QEN04DQAWV2VKKR10NKR&pd_rd_wg=JXdhf&pd_rd_r=27c76272-96c5-4fea-a134-0a0638cdba29&pd_rd_i=B07V3BQQ76&psc=1&ref_=pd_bap_d_grid_rp_0_1_ec_pr_ppx_hzsearch_conn_dt_b_bia_item_1_i" target="_blank" title="First create a user account by going to">CR2450</a> Be careful when removing the lid to know the correct  position of the cube for knowing when replacing the lid after you change the battery, that you have the correct position to avoid damage to the lid. <br>


## Reset Switch
1 <img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/f37a98ea-e089-4eca-9ba8-d81930065df9" title="Reset Button"/><br>

## T1 Battery Replacement
<iframe width="883" height="509" src="https://www.youtube.com/embed/Ec3coJxT6Lw" title="T1 Pro Cube Battery Replacement Tip" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Adding Aqara Cube T1 Pro
1. Now in the Aqara Home app, click <span style="background-color:#26AF06">**+**</span> in the upper right corner of the home page to enter the <span style="background-color:#26AF06">**Add Accessory page**</span>, then select <span style="background-color:#26AF06">**Remote control**</span> on the left then select <span style="background-color:#26AF06">**Cube T1 Pro,**</span> and select the hub to be linked.<br>
use corresponding to the instructions on the app, and then long press the device reset button for 5 seconds, waiting for the hub to indicate that the connection is successful.<br>
1 <img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/2b95bd7f-6a16-48e5-8e0f-d214f894b881" title="AQara Plus"/></a>
2 <img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/d33198f3-ce04-4ffd-8d41-32bf36a8040c" title="Remote - Cube T1 Pro"/></a><br>
2. You should now have both the E1 Hub and T1 Pro Cube installed in your AQara Software.<br><Center>     <img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/a0dfd51b-6d70-41be-b14f-2f554c3ee452" title="Accessories"/></a></Center><br>
3. I now select which Mode Switch I wanted to use.<br><iframe width="560" height="315" src="https://www.youtube.com/embed/JZXkNemHOjM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe><br>  
4. I used the Scene Mode.<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/e98ed146-299d-4700-8865-3ebd64aee72b" title="Scene Mode"/></a><br>

## Amazon Alexa

<img width="500" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/9f37a8f5-a204-4089-b30b-7a6b32346b96" title="Amazon Alexa App"/></a><br>

1.	Now you need to install <a href="https://play.google.com/store/apps/details?id=com.amazon.dee.app&hl=en" target="_blank" title="Amazon Alexa App">Amazon Alexa App</a> with an Amazon Account on your Android Mobile device rather than it being on the Echo Show 10.<br>
2. In Alexa App, after logging in, at the bottom select, <span style="background-color:#26AF06">**More Option**</span> and then <span style="background-color:#26AF06">**Skill & Games**</span>.<br>

1 <img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/ab056bd3-ad1f-4515-b591-6ddf0adea439" title="Select More"/></a>
2 <img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/65e72258-c145-4755-8bcd-b85001e67132" title="Skill And Games"/></a>
<br>

3 <img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/c18764e6-c40b-4bb9-a8ac-be465ef20eb1" title="Select Search"/></a>
4 <img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/f4d38cf2-36a1-480d-912c-ff83a5cde8ec" title="Search for aqara"/></a>
 <br>

3. Now do a Search for <span style="background-color:#26AF06">**Aqara**</span> in the search bar.<br>
4. Select the Aqara Home for EU to enter its details page as beneath:<br>

<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/ed0a6808-d1c5-4b29-9a3c-4810fb4edf27" title="Select Aqara Home for EU"/></a><br>

5. Select <span style="background-color:#26AF06">**Enable**</span> and a new window will open as shown beneath. Please enter your <span style="background-color:#26AF06">**Aqara account and password**</span> you did earlier.<br>

<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/b50b9c58-a20b-4e9a-9b62-fc3c1157120c" title="Enable Aqara Home for EU"/></a>   <img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/bd9c76fb-466c-44f8-9a3b-da22c9e975d3" title="Your Aqara Account"/></a><br>

6. After registering, tap <span style="background-color:#26AF06">**Sign in**</span> and a new window will open as shown below:<br>

<center>
<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/97d5dec4-e496-48a7-ba11-d0ea040e76eb" title="Amazon alexa successfully linked to your Aqara Account"/></a></center><br><br>

## Enable Jade (Use to be SugarMate)  in Amazon Alexa

</a><br>
You will again be doing something like what you have just done, but now for Jade Diabetes (which Use to be Sugarmate). but now has been replaced by My Jade.<br>


!!! Warning "Important Notice"
The Sugarmate skill by Amazon Alexa will no longer be available for use on January 1, 2025
Amazon has discontinued this process, and Sugarmate is no longer available for free. However, there is an alternative method that works. You can adapt the settings to reflect the new approach using the provided link.<br>


!!! note "Enable Jade Setup"

1.	<a href="https://store.payproglobal.com/checkout?products%5b1%5d%5bid%5d=107441" target="_blank" title="Jade Alexa-Only Plan">You will first need to get a Jade Alexa-Only Plan</a>  -  subscription Plan for the year<br>
2.	You will then need to register, an Account and fill in details at  <a href="https://www.jadediabetes.com/index.html" target="_blank" title="Jade Diabetes">Jade Diabetes</a> <br>
??? info "Notes"

    Before proceeding, ensure that you've downloaded and installed all required applications on their respective devices. Once everything is set up, familiarize yourself with each app’s interface and functionality. <br> 

    This will make the integration process smoother and help you troubleshoot any issues as you go along. Pay special attention to the Jade Insulin Dose Calculator App and <span style="background-color:#26AF06">**Amazon Alexa Skill setup**</span>, as these will be pivotal in ensuring streamlined communication between your devices.
 <br>
 3. After you have made an account and added some of your Personal details, you will also need to go to<span style="background-color:#26AF06">**Settings/Sharing**</span>  to add your Nightscout URL into it, this is not the (Nightscout Base URL!).<br> 
 Unless you are using a difference CGM such as Dexcom or Libre. But I will not be covering this in this setup.<br>

If you have not already done a Nightscout setup then you will need to have a Nightscout site please before you can do this, see [Setting up a Nightscout Account](../../Nightscout/Setting_up_Github_Account_part1.md) <br>

<img width="700" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/671a5d5f-31fa-4807-a846-6d7efdc5b438" title="Jade Diabetes Nightscout Settings"/> <br> 
??? info "Notes"

    You can bring your own Nightscout site or select one of our partners below to run your Nightscout site for you. If you're only bringing in Dexcom or FreeStyle Libre data, just use Jade's native capabilities. Nightscout comes into its own when you are using Medtronic and other device company products. 
4 <img width="700" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/b5650b75-b0c2-4181-965f-af2fb24d66a4" title="Setup Dexcom Share"/></a>
 

When first setting up, please be aware it can take a while to start to see your readings, and to be patient with it, if any issues you can always email Jade for support at  <a href=" mailto:Jade%20%3csupport@JadeDiabetes.com%3e" target="_blank" title="Jade Diabetes">Jade Diabetes</a>
<br>
5. Before you can add <span style="background-color:#26AF06">**Skills & Games**</span>
 or <span style="background-color:#26AF06">**Routines**</span>
, from your Alexa App (Mobile) you will also need to make sure, that in Amazon Alexa<a href=" https://www.amazon.co.uk/My-Jade-by-Diabetes/dp/B09YT3VM85?crid=7QCKHXCTLNFE&dib=eyJ2IjoiMSJ9.qh-W7YnlNqBcSfbdJCnJmQ.cN7kltCrJJbqhPwgZNw2EYXpIJV7Y5lePUUzaHAgxqI&dib_tag=se&keywords=sugarmate+app&qid=1722075367&s=digital-skills&sprefix=sugarmate%2Calexa-skills%2C68&sr=1-1" target="_blank" title="Jade Diabetes"> My Jade By Jade Diabetes </a>, Skill is Enable & Activated before we can carry on with this setup process.<br>

<img width="700" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/221e81d4-24fb-45f1-b722-1965269ae36f" title="Amazon Alexa Skill Enable My Jade Skill "/></a><br>
??? info "Important Notes"

    If you ever I’ve to disable it in <span style="background-color:#26AF06">**Amazon Alexa App, My Jade skill, on your mobile**</span>, you will also need to disable and then re enable it in the <span style="background-color:#26AF06">**Amazon Alexa My Jade-by-Jade Diabetes**</span> again, otherwise is will lose connection to your Echo Show.<br>

Once  all that is setup and working, we can go to enable My Jade by Jade Diabetes in the Amazon Alexa App (Mobile), Skills & Games.<br>
You should already have <a href="https://play.google.com/store/apps/details?id=com.amazon.dee.app&hl=en" target="_blank" title="Amazon Alexa App">Amazon Alexa App</a>, setup from when you did the Aqara Home for EU earlier. If not do it now.  <br>

<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/99dd0930-d75f-44cf-97fe-345f3a655f83" title="My Jade by Jade Diabetes"/></a><br>


## Adding to Xdrip
1.	If you are using Dexcom Server To get the data from xDrip+ to the Dexcom Share Server you first need an account on the Dexcom site. And to add it to your Xdrip Cloud Upload / Dexcom Share Server Upload<br>
You should have already setup Xdrip and have readings coming into it from your CGM.<br>
2. This is the same place you are also going to need to add your Nightscout Datasource in to Xdrip. This is located in Nightscout Sync (REST-API) Base URL and to also make sure you are getting readings from your Dexcom One into Xdrip.<br>

<img width="300" height="auto" border="0" align="center"  src="/Nightscout-xdrip-AAPS/img/Alexa/T1_Pro_Cube/xdrip readings and hamberger.jpg" title="xdrip Readings and Hamberger Menu"/>  <img width="300" height="auto" border="0" align="center"  src="/Nightscout-xdrip-AAPS/img/Alexa/T1_Pro_Cube/xdrip cloud upload.jpg" title="Cloud Upload"/></a><br>

<img width="300" height="auto" border="0" align="center"  src="/Nightscout-xdrip-AAPS/img/Alexa/T1_Pro_Cube/Nightscout Sync (REST-API).jpg" title="Nightscout Sync (REST-API)"/>  <img width="300" height="auto" border="0" align="center"  src="/Nightscout-xdrip-AAPS/img/Alexa/T1_Pro_Cube/Nightscout Sync Base URL.jpg" title="Add your Nightscout Sync Base URL API Secret"/></a><br>

It will now be best to check your Echo Show or Echo Dot to see if it is working correctly, before you do your Routines in the Alexa App. You can see some of the things you can ask Alexa on the Amazon Site Skills, also on Jade Web site or APP.<br> 

<a href="https://www.amazon.co.uk/My-Jade-by-Diabetes/dp/B09YT3VM85?crid=7QCKHXCTLNFE&dib=eyJ2IjoiMSJ9.qh-W7YnlNqBcSfbdJCnJmQ.cN7kltCrJJbqhPwgZNw2EYXpIJV7Y5lePUUzaHAgxqI&dib_tag=se&keywords=sugarmate+app&qid=1722075367&s=digital-skills&sprefix=sugarmate%2Calexa-skills%2C68&sr=1-1" target="_blank">
  <img width="Auto" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/343fdb95-fd51-44fe-9476-c49abb7b81ba" title="Aamazon - My Jade by Jade Diabetes"/></a><br>

<a href="https://www.jadediabetes.com/alexa/" target="_blank">
  <img width="Auto" height="Auto" border="0" align="left"  src="https://github.com/user-attachments/assets/2f1d4334-0b44-4024-9a20-3a86c1528d90" title="Working with Amazon Jade"/></a>
  <br>
  <br>
  
### Alexa skill - My Jade by Jade Diabetes

<a href="https://youtu.be/6ok5uKOZrhQ" target="_blank">
  <img width="auto" height="auto" border="0" align="left"  src="https://github.com/user-attachments/assets/deb46875-64e5-4f18-a335-ae9cd30a5a54" title="Alexa skill - My Jade by Jade Diabetes"/></a>

<br>
<br>
<br>
<br>
<center>
!!! Warning "Important Notice - This Video is a Old Way Watch with Caution"
</center>
### Alexa ask Sugarmate for my latest reading
<a href="https://www.youtube.com/watch?v=IKRYSBTtlJk&t=1s" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/3660151b-80f7-4393-93ab-5079954017e4" title="Alexa ask Sugarmate for my latest reading"/></a><br> 

  If all is working and you are getting your readings read out to you, you can now setup Routines to have it read out your readings automatically from moving the cube.<br>
<center>
## My Jade with Alexa Routine
</center>
<a href="https://youtu.be/j35gkpqP6ao" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/97603cca-f4cf-4957-b247-7d15f37f5c83" title="Alexa Routines"/></a>


1.	Open the Alexa app
2.	Tap the <span style="background-color:#26AF06">**menu icon**</span> in the Bottom left corner, and tap “<span style="background-color:#26AF06">**routines**</span>”<br>
<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/c49dba10-33f6-43dd-838b-4b6ccf742168" title="Routines"/></a>

3.	Tap the <span style="background-color:#26AF06">**plus button (+)**</span> at the top right to create a new routine.<br>
<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/c6ac7b3e-3438-455d-9ced-d4bb10850396" title="+ Routines"/></a>

4.	Enter a routine name (I used “<span style="background-color:#26AF06">**Jade**</span>”)<br>
5.	Tap “<span style="background-color:#26AF06">**whens +**</span> ”<img width="200" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/222bd8e8-44ac-4e1d-aacb-9f2aa2369e40" title="Add Event"/></a>
 then tap “<span style="background-color:#26AF06">**voice**</span>” <img width="200" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/fe9dbe46-f434-44f8-801b-ae93363c98b8" title="Voice"/></a>
 
 and add your custom phrase (I used “<span style="background-color:#26AF06">**Jade**</span>”) But you can add any name you like.<br>
 <center><img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/e6094d23-16be-477b-98b6-79fec99fd895" title="custom phrase Jade"/></a></center><br>
6.	Tap “<span style="background-color:#26AF06">**add action**</span>” then tap “<span style="background-color:#26AF06">**skills**</span>”<br>
<center><img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/9f9e1bf5-1e8a-4ce1-91d8-076a3b5fbe57" title="Skills"/></center></a><br>
7.	Tap <span style="background-color:#26AF06">**Your Skills**</span>, <img width="200" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/f3113272-f6f0-4e72-a9e3-8d1170caab7f" title="Your Skills"/></a>
 tap “<span style="background-color:#26AF06">**My Jade**</span>”.<img width="200" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/98544aca-1a9e-40e2-97c4-94cc993d5e70" title="My Jade by Jade Diabetes"/></a>
 <br>
8. Then tap “<span style="background-color:#26AF06">**next**</span>” upper right to confirm<br>
9.	Tap “<span style="background-color:#26AF06">**save**</span>”<br>
10.	Now ask your Echo Show. (<span style="background-color:#26AF06">**Alexa Jade**</span>) 
<br> 

<br> 
<center>
## Enabling Jade Diabetes in Amazon Alexa APP 
</center>

<center>
### Amazon Alexa Skill & Games
#### On your Mobile:
</center>
<center>
<a href="https://youtu.be/FZvuVlHOh8w" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/f44c325b-d1d0-483a-813b-bc45813f846a" title="Alexa - Jade - Skills & Games"/></a></center>

1.	Open the Alexa app
<br>
3. Tap the <span style="background-color:#26AF06">**menu icon**</span> in the Bottom left corner
<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/f6b436d0-b957-4364-8a34-d6d413cd74a5" title="Amazon Alexa Menu icon"/></a>

4. Select <span style="background-color:#26AF06">**Skills & Games**</span>
<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/d7f9f0a1-c2b3-4af3-a8b9-a19c4e122b44" title="Skills & Games "/></a>

5. Search for <span style="background-color:#26AF06">**“My Jade”**</span> or “Jade Diabetes”
<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/3cfe3a88-6598-41f3-b252-bbcca608e629" title="Alexa Skill Search"/></a>

6. Tap the <span style="background-color:#26AF06">**My Jade by Jade Diabetes**</span> skill
<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/98544aca-1a9e-40e2-97c4-94cc993d5e70" title="My Jade by Jade Diabetes"/></a>

7. Tap <span style="background-color:#26AF06">**Launch**</span> or Enable
<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/931a99ff-98a1-4b88-aa88-2e18e12e0418" title="Launch My Jade by Jade Diabetes"/></a>

8. Tap <span style="background-color:#26AF06">**Link Account**</span>Link Account in the skill’s settings page
<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/e0d67ee0-f81f-403d-b5c9-837e48b1eeaa" title="Skill Settings Link Account"/></a>

9. This will open a Jade Diabetes-branded pop-up window
10. Login using your <span style="background-color:#26AF06">**Jade email address**</span> and <span style="background-color:#26AF06">**password**</span> Account
10. All Done! Now Try the suggestions below!
<br>
<br>

!!! Warning "Important Notice - This Video is a Old Way Watch with Caution"
## Amazon Alexa Routines
<a href="https://youtu.be/u9NZkSLj8ig" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/0a1a4677-04b8-4a71-9267-696d3c31d270" title="Routines in Amazon Alexa for a T1 Pro Cube"/></a></center>


<br>You should now have a fully working T1 Pro Dice (cube) 
Congratulations and my apologize for the length of this setup was a hard one for me to write up with trying to give as much details as I could.<br> 
<br>

<br>

<br>

[&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;]()
[Please Subscribe to our UTUBE Channel](https://www.youtube.com/channel/UC9TwtBefjjKw_uKHiIWMkBA?sub_confirmation=1){ .md-button }

<br>
<a href="https://maundyrelief.org.uk/" target="_blank">
  <center><img width="300" height="auto" border="0" align=""  src="https://github.com/user-attachments/assets/585dd221-4f22-4e83-978d-3eedb39d3ca9" title="Maundy Relief"/></center></a>
<br>

<br>
<a href="https://www.diabetes.org.uk/" target="_blank">
<img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/21b87537-f1fa-4e01-904c-132085884544" title="Diabetes UK"/> </a>Why Not take visit <a href="https://www.diabetes.org.uk/support-us/fundraise/fundraising-events/pedal-for-progress" target="_blank"> :man_biking_tone1: UK Wide Cycle Ride - Diabetes.uk :woman_biking_tone5:</a> **or** <a href="https://swim22.diabetes.org.uk/?fbclid=IwAR3XSygKTkbU7l_Xgu88WU3Q3EYFrFoAj1STvQTVz_6X-xthmjqOUWMTiww" target="_blank">Diabetes.UK Swim22 :man_swimming_tone5:</a> **or** <a href="https://www.diabetes.org.uk/support-us/fundraise/fundraising-events/60-miles-challenge" target="_blank">:man_walking_tone5: Diabetes UK Month of Miles Challenge :woman_running:</a> for all of your Diabetes Needs!



 









</br>



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
		
		
adding 	Yellow Hightligher!!!!!!!!	with bold too
<span style="background-color: #FFFF00">**Marked text**</span>

adding 	Green Hightligher!!!!!!!!	with bold too
<span style="background-color:#26AF06">**Routines**</span>


<a>
  <img width="auto" height="auto" border="0" align="center"  src="/img/Nightscout/Time to Update Nightscout.png" title="Update Tool"/></a>	




Adding a image with link
<a href="https://www.youtube.com/watch?v=MFsbm45b6YY" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="/img/Part 1 Setting up Github 2021/Github account details.jpg" title="github account details"/>
</a><br>
******************************
just a link
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



Note:

**Note:** a note is something that needs to be mentioned but is apart from the context.

This is a note with a drop down! you have to keep the format the same for it to work!!!!!!!!!!
??? info "Notes"

    Before proceeding, ensure that you've downloaded and installed all required applications on their respective devices. Once everything is set up, familiarize yourself with each app’s interface and functionality. <br> 


???+ note "Note"

!!! Warning "Important Notice - This Video is a Old Way Watch with Caution"



List:

This is a regular paragraph.

Paragraph:

1. **Now Open another tab**  to make a Mongodb Atlas** Account: <a href="https://www.mongodb.com/cloud/atlas" target="_blank" title="Click Start Free">See Here</a> 
  and **click** Start Free
 <img width="auto" height="auto" border="0" align="center"  src="/img/Atlas/MongoDB Atlas start free.jpg"Click Start"/>
   2. Sub item two
   3. Sub item three
2. Item two

Header:

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


<!--  
  ******************************************************************************************************************
  mkdocs.yml    # The configuration file.
    docs/
    index.md  # The documentation homepage.
       ...       # Other markdown pages, images and other files.
		
		****************************************************************

[In the the video above](../xdrip/Xdrip%20-%20Setting%20up%20Glucose%20Meters.md#video-instructions)





!!!warning 
    Do not use CONTOUR DIABETES app, when using xdrip you can only have one App running!
   <br><br>



   !!!info 
    Do not use CONTOUR DIABETES app, when using xdrip you can only have one App running!
   <br><br>


		
<a href="http://nightscout.github.io/pages/update-fork/" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="/img/Nightscout/Time to Update Nightscout.png" title="Update Tool"/></a>		
		
		
adding 	Yellow Hightligher!!!!!!!!	with bold too
<span style="background-color: #FFFF00">**Marked text**</span>


link

<a href=" https://github.com/" target="_blank" title="Github">Click Here</a> 

  <img width="auto" height="auto" border="0" align="center"  src="/img/Fork and Deploy cgm remote monitory Part 4/warning_sign.png" title="Update Tool"/></a>	

<img width="30" height="30" src="/img/Fork and Deploy cgm remote monitory Part 4/clipart2068155.png">

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


List
This is a regular paragraph.


****************
Relative Link:
*******************
[HardwareDataSource](xdrip%20-%20hardwaredatasource.md)
[HardwareDataSource](xdrip%20-%20hardwaredatasource.md)

[What is AAPS](../AndroidAPS/What%20is%20AAPS.md)


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

*******************************************************************************************************************************
*******************************
orange table

<table width="1166" border="1" style="border-color: #000000; background-color: #ffffff;" cellpadding="1" cellspacing="1" height="98">
<tbody>
<tr style="height: 16px;">
<td style="width: 1158px; border-color: #000000; background-color: #db4e12;" fff=""><span style="font-size: 14pt;"><strong><span style="color: #ffffff;">Note!</span></strong></span></td>
</tr>
<tr style="height: 56.4063px;">
<td style="width: 1158px; border-color: #000000;"><span style="font-family: tahoma, arial, helvetica, sans-serif; font-size: 14pt;">If you’re on Heroku and have Automatic Deploys enabled, you’re done!<br>
 If you don’t have Automatic Deploys on yet, or aren’t sure, run through these steps below!</span></td>
</tr>
</tbody>
</table>
***************************************
red warning table
***************************
<table width="1266" border="1" style="border-color: #000000; background-color: #ffffff;" cellpadding="1" cellspacing="1" height="98">
<tbody>
<tr style="height: 16px;">
<td style="width: 1158px; border-color: #000000; background-color: #FF0000;" fff=""><span style="font-size: 14pt;"><strong><span style="color: #ffffff;">Warning!</span></strong></span></td>
</tr>
<tr style="height: 56.4063px;">
<td style="width: 1158px; border-color: #000000;"><span style="font-family: tahoma, arial, helvetica, sans-serif; font-size: 14pt;"> 1: Some new features, updates, or bug fixes may require that you clear your browser cache before you will see the changes taken effect<br/> 2: If you get no errors and no readings after a while see about doing a <a href="http://127.0.0.1:8000/user-guide/Redeploying%20your%20repository/" target="_blank" title="Redeploying your repository link">Redeploying your repository</a> </span></td>
</tr>
</tbody>
</table>
*********************************
Blue Note
******************************
<table width="1166" border="1" style="border-color: #000000; background-color: #ffffff;" cellpadding="1" cellspacing="1" height="98">
<tbody>
<tr style="height: 16px;">
<td style="width: 1158px; border-color: #000000; background-color: #5B9BD5;" fff=""><span style="font-size: 14pt;"><strong><span style="color: #ffffff;">Note!</span></strong></span></td>
</tr>
<tr style="height: 56.4063px;">
<td style="width: 1158px; border-color: #000000;"><span style="font-family: tahoma, arial, helvetica, sans-serif; font-size: 14pt;"> You will have already needed to have done <a href="https://atlas-night-out.github.io/xdrip-Nightscout-AAPS/user-guide/Setting_up_Github_Account_part1/" target="_blank" title="firt you need to do Part 1 Setting up Github Account for Nightscout">Part 1 Setting up Github Account for Nightscout</a>. To be able to continue.</span></span></td>
</tr>
</tbody>
</table>



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
<img width="400" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Nightscout/sadface.png" Sad day"/><br>
-->



