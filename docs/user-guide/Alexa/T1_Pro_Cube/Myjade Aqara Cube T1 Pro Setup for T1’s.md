<center><img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/T1pro_cube_logo860x1147.jpg" title="T1 Pro Cube"/></a></center><br>The video below shows the old way we used to get readings read out to us with Sugarmate that which caused to work in Feb 2025
<iframe width="660" height="415" src="https://www.youtube.com/embed/bTc6qBVb9d4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe><br>

Jade the new way now in 2025 to have your reading read out to you!

<iframe width="660" height="415" src="https://www.youtube.com/embed/za9m8ZiOY80?si=yLtleLflcHm19vAX" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Short Intro
This device is a very helpful cube T1 Pro that we can use to read out are Glucose readings by picking it up or turning it around on a certain Dice number you pick. But not only that you can control your Home and so much more.
You can even use Presence Sensor or motion sensors to have your blood readings read out to you, wherever you want in your home.
<br>

Sadly, Sugarmate is no longer doing there App now for it to work in Amazon Alexa App. Since when I wrote these setups up last year, so I will have to re check on my setups to change them due me having e Found an alternative now called Myjade which is a good replacement, in 2025

New Alexa-Only Plan for SugarMate Users
We’ve heard that SugarMate has removed their Alexa integration, making life harder for vision-impaired users. So, we’re stepping in with a simple, affordable Alexa-only plan!
This plan will announce your blood sugar levels through Alexa for a <a href="https://store.payproglobal.com/checkout?products%5b1%5d%5bid%5d=107441" target="_blank" title="MyJade Subscription">Click Here</a>

<a href="https://store.payproglobal.com/checkout?products%5b1%5d%5bid%5d=107441" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src=" /xdrip-Nightscout-AAPS/img/Alexa/Myjade/myjade offer.jpg" title="github account details"/>
</a><br>

I will be trying to help you set up an Echo Show 10 (3rd Gen) or an Echo Dot or a Samsung Tablet. So, it will read out your Glucose readings. I will not be going through and explaining the unboxing as this as been done in other videos.<br>


<br>

## Items you are going to need

1.	<a href="https://www.amazon.co.uk/dp/B0BHWS3VTZ?maas=maas_adg_F2E7A71BEAD7E7012F8DA4528E905764_afap_abs&linkCode=sl1&tag=paulhibbert-21&linkId=17f5a99c41bcb0d2cd1cdd6c378794b3&language=en_GB&ref_=as_li_ss_tl" target="_blank" title="Aqara Cube T1 Pro">Aqara Cube T1 Pro</a>   (Also REQUIRES AQARA ZIGBEE 3.0 HUB)
2.	<a href="https://www.amazon.co.uk/dp/B09BJCNCKM?psc=1&ref=ppx_yo2ov_dt_b_product_details" target="_blank" title="Aqara Smart Hub">Aqara Smart Hub E1</a> Aqara Smart Hub E1 (2.4 GHz Wi-Fi Required)
3.	<a href="https://www.amazon.co.uk/dp/B084P3KP2R?psc=1&ref=ppx_yo2ov_dt_b_product_details" target="_blank" title="Echo Show 10">Echo Show 10 (3rd generation)</a> or an <a href="https://www.amazon.co.uk/gp/product/B09B96TG33/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1" target="_blank" title="Echo Dot">Echo Dot </a> (5th generation, 2022 release) Or your Samsung Mobile or Tablet
4.	Android Mobile Device in my case a <a href="https://www.amazon.co.uk/gp/product/B07W6XFX64/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1" target="_blank" title="Samsung Note10 +">(Samsung Note10 +)</a> 
If you have an iPhone you may wish to set it up with Home App (but I will not be showing you a setup in this video) <br>

## Software you will need to have Setup

1.	[Nightscout](../../Nightscout/Setting_up_Github_Account_part1.md#part-1-setting-up-the-github-for-nightscout)
(Which I will not be showing you how to setup in these instructions) But will add a link for you to do it if you have not done so already. 
<br>

2.	<a href="https://www.sugarmate.io/" target="_blank" title="Sugarmate">Sugarmate</a>  on a  PC (You will need to sign up) or
3.	Sugarmate link sent onto your Desktop of your mobile phone.
4.	<a href="https://play.google.com/store/apps/details?id=com.amazon.dee.app&hl=en" target="_blank" title="Amazon Alexa App">Amazon Alexa App</a> 
<br> with an Amazon Account
5.	<a href="https://atlas-night-out.github.io/xdrip-Nightscout-AAPS/user-guide/xdrip/xdrip%20-%20Download/" target="_blank" title="Xdrip">Xdrip</a> 
6.	<a href="https://aiot-management.aqara.cn/config/app/aqaraHomeDeveloping" target="_blank" title="Aqara Home">Aqara Home</a>  App
<br>

## My Setup

#### Quick Setup
### Add Device
1.	First download the Aqara Home app.
Search for "Aqara Home" in the Apple App Store, or Google Play,
Xiaomi Get Apps, Huawei App Gallery, or scan the following QR code to download the Aqara Home App:<br>
<img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Aqara barcode.jpg" title="Aqara Home App"/></a><br>

2.	An Aqara Zigbee 3.0 hub is required. Please make sure
you have an <a href="https://www.amazon.co.uk/dp/B09BJCNCKM?psc=1&ref=ppx_yo2ov_dt_b_product_details" target="_blank" title="Aqara Smart Hub">Aqara Smart Hub E1</a> installed and added to
your Aqara Home App<br>

## Setting up the E1 Hub 
<img width="200" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/E1 Hub.png" title="E1 USB Hub"/></a><br>

1. Plug the hub into a USB port that can provide power, wait for the yellow indicator to flash quickly, and make sure your mobile phone is connected to a Wi-Fi network in the 2.4 GHz frequency band. <br>
You will need to make sure your home router is set to a 2.4 ghz bands until you are setup with your hub and T1 Pro, you may turn it back to Auto 5GHz after the setup, All routers will be different on how to do this process, so see your Routers Manual.<br>
<img width="600" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Virgin Riuter settings.jpg" title="Putting a Virgin Router into a 2.4Ghz"/></a><br><br>
keep the mobile phone as close to the hub as possible, and your mobile phone and hub are using the same Wi-Fi network.<br>

2. Open the Aqara Home app, click the <span style="background-color: #FFFF00">**+**</span> in the upper right corner of the home page, select <span style="background-color: #FFFF00">**Hub E1**</span>, from  <span style="background-color: #FFFF00">**Add Accessory - Gateway/Hub E1**</span> and follow the instructions of the app to operate.<br><br>
1 <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Adding Accessory.png" title="Add Accessory"/></a>2 <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Gateway_Hub E1.png" title="Gateway - Hub E1"/></a><br>
3 <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Add Hub E1.png" title="Add Hub E1"/></a>4 <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/scan the device.png" title="scan the Device"/></a><br>
5.	If the addition fails, please long press the hub button for 10s to reset the network, and then add it again in the app.<br>
6. Once the E1 Hub is connected you can now connect the T1 Pro Cube.<br>

<iframe width="392" height="397" src="https://www.youtube.com/embed/6WkQg_FvaU8" title="Connecting to Aqava E1 Hub after changing Router to a 2 4ghz" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe><br>

## Adding Battery <br>
Open the battery cover of Cube T1 Pro with the ejector tool, take out the battery, replace it with a new <span style="background-color: #FFFF00">**CR2450**</span>.
Be careful when removing the lid to know the correct  position of the cube for knowing when replacing the lid after you change the battery, that you have the correct position to avoid damage to the lid. <br>

## Reset Switch
1 <img width="500" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/T1 Pro Reset button pairing.jpg" title="Reset button"/><br>

## T1 Battery Replacement
<iframe width="883" height="509" src="https://www.youtube.com/embed/Ec3coJxT6Lw" title="T1 Pro Cube Battery Replacement Tip" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Adding Aqara Cube T1 Pro
1. Now in the Aqara Home app, click <span style="background-color: #FFFF00">**+**</span> in the upper right corner of the home page to enter the <span style="background-color: #FFFF00">**Add Accessory page**</span>, then select <span style="background-color: #FFFF00">**Remote control**</span> on the left then select <span style="background-color: #FFFF00">**Cube T1 Pro,**</span> and select the hub to be linked.<br>
use corresponding to the instructions on the app, and then long press the device reset button for 5 seconds, waiting for the hub to indicate that the connection is successful.<br>
1 <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Aqara Home app click plus.png" title="AQara Plus"/></a>2 <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/remote T1 Pro cube.png" title="Remote - Cube T1 Pro"/></a><br>
2. You should now have both the E1 Hub and T1 Pro Cube installed in your AQara Software.<br><Center>     <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Accessories.jpg" title="In Accessories"/></a></Center><br>
3. I now select which Mode Switch I wanted to use.<br><iframe width="560" height="315" src="https://www.youtube.com/embed/JZXkNemHOjM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe><br>  
4. I used the Scene Mode.<img width="400" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Mode switch scene mode.jpg" title=" I used Scene Mode"/></a><br>

## Amazon Alexa

<img width="400" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Amazon Alexa.jpg" title="Google Play Amazon Alexa"/></a><br>

1.	Now you need to install <a href="https://play.google.com/store/apps/details?id=com.amazon.dee.app&hl=en" target="_blank" title="Amazon Alexa App">Amazon Alexa App</a> with an Amazon Account on your Android Mobile device rather than it being on the Echo Show 10.<br>
2. In Alexa App, after logging in, at the bottom select, <span style="background-color: #FFFF00">**More Option**</span> and then <span style="background-color: #FFFF00">**Skill & Games**</span>.<br>

1 <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Alexa App More.jpg" title="Select More"/></a> 2 <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Skill And Games.jpg" title="Select Skill And Games"/><br>

3 <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Select Search.jpg" title="Select Search"/>4 <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/search for aqara.jpg" title="Search for aqara"/> <br>
3. Now do a Search for <span style="background-color: #FFFF00">**Aqara**</span> in the search bar.<br>
4. Select the Aqara Home for EU to enter its details page as beneath:
<img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Select Aqara Home for EU.jpg" title="Select Aqara Home for EU"/><br>

5. Select <span style="background-color: #FFFF00">**Enable**</span> and a new window will open as shown beneath. Please enter your <span style="background-color: #FFFF00">**Aqara account and password**</span> you did earlier.<br>
<img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Enable Aqara Home for EU.jpg" title="Enable Aqara Home for EU"/>   <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Aqara Login.jpg" title="Login to your Aqara Account"/><br>

6. After registering, tap <span style="background-color: #FFFF00">**Sign in**</span> and a new window will open as shown below:<br>
<img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Amazon alexa successfully linked.jpg" title="Amazon alexa successfully linked to your Aqara Account"/><br>

## Enable SugarMate in Amazon Alexa

You will again be doing something similar to what you have just done but now for Sugarmate.<br>

1.	Now we need to enable, the SugarMate skill through the Alexa app on your phone.<br>
2.	In Alexa App, after logging in, at the bottom select, <span style="background-color: #FFFF00">**More Option**</span> and then <span style="background-color: #FFFF00">**Skill & Games**</span>.<br>
3.	In the search look for Sugarmate <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/amazon sugarmate skill.jpg" title="Sugarmate Skill"/><br>
4.	Now setup a Sugarmate account if you have not already done so yet, it will give you an email address as a Follower.<br>
5.	Before you can add Routines by Launch in Alexa App, you will have needed to have added your Nightscout DataSource before hand or your Dexcom Server.<br><img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Sugarmat launch.jpg" title="Sugarmate Launch"/>  <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/goto sugarmate settings.jpg" title="sugarmate settings"/>

By going to your Sugarmate account / settings / Datasource and adding your Datasource.<br><img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Sugarmate settings.jpg" title="Settings"/>  <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Sugarmate datasource.jpg" title="Datasource"/><br>
You will need to have sign in to Sugarmate from your Browser on your mobile.<br><br> <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/sign in on mobile browser.jpg" title="Sign in to Sugarmate"/><br>
If you have not already done a Nightscout setup then you will need to have a Nightscout site please before you can do this, see [Setting up a Nightscout Account](../../Nightscout/Setting_up_Github_Account_part1.md) <br>
 

## Adding to Xdrip
1.	If you are using Dexcom Server To get the data from xDrip+ to the Dexcom Share Server you first need an account on the Dexcom site. And to add it to your Xdrip Cloud Upload / Dexcom Share Server Upload<br>
You should have already setup Xdrip and have readings coming into it from your CGM.<br>
2. This is the same place you are also going to need to add your Nightscout Datasource in to Xdrip. This is located in Nightscout Sync (REST-API) Base URL and to also make sure you are getting readings from your Dexcom One into Xdrip.<br>

<img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/xdrip readings and hamberger.jpg" title="xdrip Readings and Hamberger Menu"/>  <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/xdrip cloud upload.jpg" title="Cloud Upload"/><br>

<img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Nightscout Sync (REST-API).jpg" title="Nightscout Sync (REST-API)"/>  <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Nightscout Sync Base URL.jpg" title="Add your Nightscout Sync Base URL API Secret"/><br>

It will now be best to check your Echo Show or Echo Dot to see if it is working correctly, before you do your Routines in the Alexa App. You can see some of the things you can ask Alexa on the Amazon Site Skills, also in the Sugarmate APP.<br> <center><a href="https://www.amazon.co.uk/Wild-Village-Sugarmate/dp/B0722KNWX2" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Amazon Sugarmate.jpg" title="Amazon Site Skills"/></a><iframe width="560" height="315" src="https://www.youtube.com/embed/IKRYSBTtlJk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe></center><br> 

  If all is working and you are getting your readings read out to you, you can now setup Routines to have it read out your readings automatically from moving the cube.<br>

## Amazon Alexa Routines
<iframe width="660" height="415" src="https://www.youtube.com/embed/u9NZkSLj8ig" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


1. Sign into your Amazon Alexa.<br><img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Amazon Alexa2.jpg" title="Amazon Alexa App"/>  <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Alexa More.jpg" title="Alexa More"/>
2. Select <span style="background-color: #FFFF00">**More**</span>
3. Select <span style="background-color: #FFFF00">**Routines**</span><br><img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Select Routines.jpg" title="Select Routines"/>  <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/plus sign.jpg" title="Select The Plus Sign"/>
4.	Select the + sign at the top right. 
5.	Pick the + for  <span style="background-color: #FFFF00">**When this Happens**</span><br><img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/when this happens.jpg" title="when this happens"/>  <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Smart Home.jpg" title="Select Smart Home"/>
6. Then pick the <span style="background-color: #FFFF00">**Smart Home**</span><br><br>
Pick your T1 Pro Cube number you would like to use. In my case I want 5 on the cube (Disc) to do this task.
7. <span style="background-color: #FFFF00">**Choose your Device**</span> (Cube T1 Pro-five)<br><img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Choose Device.jpg" title="Choose Device"/>  <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/when motion is Detected.jpg" title="Select Detected then Next"/>
8.	Now select When Motion is: <span style="background-color: #FFFF00">**Detected**</span> Then <span style="background-color: #FFFF00">**Next**</span>
9.	Now Add Action: <span style="background-color: #FFFF00">**+**</span> (New Routine)<br><img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Add Action.jpg" title="Add Action"/>  <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Customised.jpg" title="Customised"/>
10.	 Select the <span style="background-color: #FFFF00">**Customised**</span> at the top.
11.	Now enter what you would ask Alexa to do.<br><img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/enter what you would ask Alexa.jpg" title="Enter what you would ask Alexa"/>  <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Alexa ask sugarmate for my latest reading.jpg" title="Alexa, ask sugarmate for my latest reading"/>
12. Add <span style="background-color: #FFFF00">**Alexa, ask sugarmate for my latest reading**</span> or you can have Alexa, ask Sugarmate what I'm at” or Alexa, ask Sugarmate to switch units
13. Save
14.	Now select your device you want your Blood reading to come out from you can select more than one device by selecting the + again and adding the device.<br><img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/from_choose Device.jpg" title="From choose Device"/>  <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Alexa/T1_Pro_Cube/Choose Device Daves Echo Dot Living room.jpg" title="Choose your Device"/>
15.	 Then <span style="background-color: #FFFF00">**Choose Device**</span>, and then select the <span style="background-color: #FFFF00">**Device  you want**</span>. In My case an Echo Dot to work in my Living room.<br><br>You should now have a fully working T1 Pro Dice (cube) 
Congratulations and my apologize for the length of this setup was a hard one for me to write up with trying to give as much details as I could.<br> 

I wish I could help more with other setups but at least you will have a clue idea to vary it to your setup, I hope!<br> 

 









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


<a>
  <img width="auto" height="auto" border="0" align="center"  src="/img/Nightscout/Time to Update Nightscout.png" title="Update Tool"/></a>	




Adding a image with link
<a href="https://www.youtube.com/watch?v=MFsbm45b6YY" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="/img/Part 1 Setting up Github 2021/Github account details.jpg" title="github account details"/>
</a><br>
******************************
just a link
***************

<a href="https://www.mongodb.com/cloud/atlas" target="_blank" title="Click Try Free">See Here</a> 

********************************
link to another page!
*************************

[Nightscout](../../Nightscout/Setting_up_Github_Account_part1.md#part-1-setting-up-the-github-for-nightscout)

********************************************

Adding Video

<iframe width="850" height="415" src="https://www.youtube.com/embed/MFsbm45b6YY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


Adding an embeded video
<iframe id="video3" width="560" height="315" src="https://www.youtube.com/embed/o7-T2IrDJ_A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


Note
**Note:** a note is something that needs to be mentioned but is apart from the context.


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



