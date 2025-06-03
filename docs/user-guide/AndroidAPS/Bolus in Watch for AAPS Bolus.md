<!-- this is  on github server!
docs made by D.Galloway 2019- 2021-->

# AAPS on Wear OS smartwatch 
## Ticwatch Pro 5 Watch with AAPS Watch faces



<img width="400" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/AAPS/Ticwatch Pro 5.jpg" title="(BG) Blood Readings Icon"/><br>

### Watch wear version of AAPS allows you to: 
•	show data on your watch: by providing custom watchfaces or in standard watchfaces with use of complications. <br>

•	control AAPS on mobile phone: to bolus, set a temporary target etc.


### Summary

• To be able to bolus from your watch, you are first going to have installed xdrip+ and have it setup and working on your Phone.<br>

• You will also have to make your own WearOS.APK file and installed that onto your watch by sideloading it. You do this at your own risk. There is no warrenty on this  I have made a video showing how to do this and I will also  add a document to help you setup when I get time too! So stay tuned! (Grammer corrected by Berni Warren Thank you!)

## Step 1 What you will already needed to have done before you go any further! 

1. You will need to installed xdrip+ onto your Phone and working, so its getting reading from your CGM. See <br>
[Install xdrip±](../xdrip/xdrip%20-%20install.md#install-xdrip_1) <br>

2. Important notes Please use Android Studio Version 2020.3.1 or newer to build the apk.
Windows 10 32-bit systems are not supported by Android Studio 2020.3.1 <br>

3. Make your own copy of AAPS_3.1.0.3.APK file in Android Studio. And then have it AAPS 3.1.0.3.APk file installed onto your Phone and working with xdrip+,  then within the ConfigBuilder you need to enable the Wear plugin. <br>
<img width="500" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/AAPS/AndroidAPS_3.2.0.3_main.jpg" title="Android_3.2.0.3 APP.Main"/> <Br><br>

4. You can copy the Repo code from Github into Android Studio from  <a href=" https://github.com/nightscout/AndroidAPS   " target="_blank" title="Git Hub Repository">AAPS     </a>    Or go to https://github.com/nightscout/AndroidAPS  to make your own AAPS.APK file to install onto your phone.<br>

5. See my video on how to do this process of making your own Wear APK file from <a href=" https://youtu.be/VwG-rOolBDM   " target="_blank" title="UTUBE">Utube     </a> or go to  https://youtu.be/VwG-rOolBDM  but you will need to choose Android_3.1.0.5 APP.Main instead of wear when Generate a signed Bundle! For the Software version, later you will make a wear.APK file for your watch Faces.<br>
<table width="1166" height="515" border="1" style="border-color: #000000; background-color: #ffffff;" cellpadding="1" cellspacing="1" height="98">
<tbody>
<tr style="height: 16px;">
<td style="width: 1158px; border-color: #000000; background-color: #5B9BD5;" fff=""><span style="font-size: 14pt;"><span style="color: #ffffff;">Generate Signed Bundle or APK for Wear AAPS watchfaces</span></span></td>
</tr>
<tr style="height: 56.4063px;">
<td style="width: 1158px; border-color: #000000;"><span style="font-family: tahoma, arial, helvetica, sans-serif; font-size: 14pt;">
<iframe width="860" height="415" src="https://www.youtube.com/embed/VwG-rOolBDM?si=B7Pr92kJUqqp0t3g" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>  </span></td>
</tr>
</tbody>
</table> <br>
6. You will need to make sure Wear is enabled in AAPS, by going to the Config Builder and scrolling down to Wear. And select it and then click the gear icon to select your setting for it. E.g BG COB<br>

<img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/AAPS/config_wear settings.jpg" title="Config Builder - Wear"/> <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/AAPS/Config Builder wear wear settings.jpg" title=" Wear Setting"/> <br><br>
7. And also, Settings added into xdrip+ for you to get readings onto your watch. By going to Setting/Smart Watch Features/Android Wear Integration <br>

<img width="300" height="auto" border="0" align="left"  src="/xdrip-Nightscout-AAPS/img/Medtronic/xdrip Smart Watch Features.jpg" title="xdrip Smart Watch Features"/>

<img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Medtronic/Android Wear Intergration.jpg" title="Android Wear Intergration"/>

<img width="300" height="auto" border="0" align="left"  src="/xdrip-Nightscout-AAPS/img/Medtronic/Android Wear Intergration settings.jpg" title="Wear Intergration Settings"/>

<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
8. Your AAPS .APK file you have just created in Android Studio will now need to be sideloaded onto your Watch. You do this in a similar way as you will have done with xdrip+ onto your watch with sideloading it, but AAPS is done a little different as its not already installed onto your watch and needs to be added. Big Thank you to  (By Malcolm Bryant) for doing the wear 2 Installer! <br><br>
9. I'm not very good at making videos with me speaking but thought until I have time to write up more docs to do this process, I thought best to just add it so then this will give me more time to try to write some docs up for it, but until then you will still be able to setup. So here is the video to help you sideload wear onto your watch!<br>

<table width="1166" height="515" border="1" style="border-color: #000000; background-color: #ffffff;" cellpadding="1" cellspacing="1" height="98">
<tbody>
<tr style="height: 16px;">
<td style="width: 1158px; border-color: #000000; background-color: #5B9BD5;" fff=""><span style="font-size: 14pt;"><span style="color: #ffffff;">Generate Signed Bundle or APK for Wear AAPS watchfaces</span></span></td>
</tr>
<tr style="height: 56.4063px;">
<td style="width: 1158px; border-color: #000000;"><span style="font-family: tahoma, arial, helvetica, sans-serif; font-size: 14pt;">
<iframe width="860" height="415" src="https://www.youtube.com/embed/d3lI4Wp1N6E?si=TxOUSm7sfWissl4O" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</span></td>
</tr>
</tbody>
</table>
   
# (not fully finished on this page yet! will be back soon to finish it)






## *Step 2 Instructions*
1. First  double Click on BG Readings icon on which ever Watch Face you are using for AASP. There are a few to choose from. <br>
## Watchfaces available <br>
<img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/AAPS/AAPS(v2).png" title="AAPS(v2)"/>    <img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/AAPS/AAPS (Digital Style).png" title="AAPS (Digital Style)"/><br>
<br>AAPS(v2)  AAPS (Digital Style)

<img width="300" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/AAPS/AAPS (Large).png" title="AAPS (Large)"/>AAPS (Large)



















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

<table width="1166" height="600" border="1" style="border-color: #000000; background-color: #ffffff;" cellpadding="1" cellspacing="1" height="98">
<tbody>
<tr style="height: 16px;">
<td style="width: 1158px; border-color: #000000; background-color: #5B9BD5;" fff=""><span style="font-size: 14pt;"><span style="color: #ffffff;">Version of Nightscout Video</span></span></td>
</tr>
<tr style="height: 56.4063px;">
<td style="width: 1158px; border-color: #000000;"><span style="font-family: tahoma, arial, helvetica, sans-serif; font-size: 14pt;">
<iframe width="850" height="415" src="https://www.youtube.com/embed/MFsbm45b6YY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>  </span></td>
</tr>
</tbody>
</table>





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

