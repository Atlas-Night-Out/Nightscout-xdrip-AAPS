<!-- this is  on github server!
docs made by D.Galloway 2019- 2021-->


<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/fd599896-1918-4933-ac8d-a5e4a298abbc" title="AAPS logo"/></a>

# **Intro into AAPS** <br>

!!! Question - what is AAPS
What is AAPS

!!! note "Info"


AAPS (Android Artificial Pancreas System) is a do-it-yourself (DIY), open-source automated insulin delivery (AID) system designed for people with Type 1 diabetes or insulin-dependent Type 2 diabetes.<br>

 It transforms an Android smartphone, a compatible insulin pump, and a CGM (Continuous Glucose Monitor) into a closed-loop system that automatically adjusts insulin delivery to keep blood glucose in range.<br>

!!! Question - what is AAPS
🔄 How Does AAPS Work?<br>

!!! note "Info"

1. Receives CGM Data (e.g., Dexcom G6, Libre 3)
• Continuously monitors glucose levels.
2. Predicts Future Glucose
• Uses the OpenAPS algorithm to forecast highs/lows.
3. Adjusts Insulin Automatically<br>
• Sends commands to your insulin pump (e.g., Omnipod DASH, Dana RS) to:<br>
• ⏫ Increase basal insulin if glucose is rising.<br>
• ⏬ Reduce/suspend insulin if glucose is dropping.<br>
• 💉 Give micro-boluses to correct highs.<br>
🔄 Updates every 5 minutes, 24/7 – mimicking a healthy pancreas!<br>
<br>

📋 Key Features <br>
✅ Open-source & free (no corporate lock-in).<br>
✅ Works offline (no internet required for looping).<br>
✅ Highly customizable (adjust targets, insulin sensitivity, etc.).<br>
✅ Supports multiple pumps & CGMs (unlike commercial systems).<br>
✅ Integrates with Nightscout (cloud monitoring for caregivers).<br>
<br>

!!! Warning "Important Considerations"

❗ Not FDA-approved – DIY project (use at your own risk).<br>
❗ Requires technical setup (must build the app yourself).<br>
❗ Medical supervision essential (always consult your doctor).<br>
❗ Backup plan needed (carry glucose & spare insulin).<br>
<br>

!!! note "What You Need to Use AAPS"

| Component    | Examples                         |
| ----------- | ------------------------------------ |
| `Android Phone`       | Android 9+ with Bluetooth   :material-check:      |
| `CGM`       | Dexcom G6/G7, Libre 2+/3+, Medtronic Guardian :material-check: |
| `Insulin PumpTE`    | Omnipod DASH, Dana RS/i, Accu-Chek Combo :material-check:  |
| `AAPS App APK`    | Self-built from <a href="https://github.com/nightscout/AndroidAPS" target="_blank"> Github</a> repo  |

<br>

!!! Tip "AAPS vs. Commercial Systems"

| Feature    | AAPS|Tandem Control-IQ / Omnipod 5|
| ----------- | ------------------------------|-------------|
| `Cost`       | Free        |££££ - Funded (pump + supplies)
|
| `Customization`       |Fully adjustable |Limited by FDA rules|
| `Pump Choice`    | Multiple options  |Brand-locked|
| `Approval`    | DIY (community-supported)  |FDA-approved|

<br>

!!! Note "🚀 Getting Started" 


1. Read the <a href="https://androidaps.readthedocs.io/en/latest/" target="_blank"> Official Docs</a>  – Understand risks & requirements. This site will be trying to help on video setups rather than the Official Docs already made for to use.
2. <a href="https://androidaps.readthedocs.io/en/latest/Getting-Started/CompatiblePumps.html" target="_blank"> Check Compatibility</a> – Ensure your devices work with AAPS.
3. Join Support Groups (Facebook: <a href="https://www.facebook.com/groups/androidapsusersuk" target="_blank"> "AndroidAPS Users UK"</a> -<a href="https://www.facebook.com/groups/AndroidAPSUsers" target="_blank"> "AndroidAPS Users"</a> - <a href="https://discord.com/invite/4fQUWHZ4Mw" target="_blank"> "Discord"</a> - <a href="https://www.facebook.com/groups/TheLoopedGroup" target="_blank"> "Looped"</a>.<br>
4. Build & Install – Follow the <a href="https://androidaps.readthedocs.io/en/latest/SettingUpAaps/BuildingAaps.html" target="_blank"> step-by-step guide</a>.

<br>

=== "🔄 AAPS in Action"
``` mermaid
graph LR
  A[CGM] --> |Bluetooth| B[AAPS App];
  B -->|Commands| C[Insulin Pump];
  C --> D[Adjust Insulin];
  B --> E[Nightscout Cloud];
  E --> F[Caregiver/Monitor];
```


<br> 



<br> <br>

!!! Question  "FAQ"

Q: Is AAPS safe?
A: Many users report improved glucose control, but errors can happen – always monitor and have backup supplies.<br>

Q: Can I use an iPhone?<br>
A: No, AAPS is Android-only. iOS users can try Loop.<br>

Q: How hard is setup?<br>
A: Requires effort (~2-10 hours), but no coding knowledge is needed.<br>

Q: Will it prevent all hypos/hypers?<br>
A: No – it reduces extremes but isn’t perfect. User input (meals, exercise) still matters.<br>

<br><br>

!!! note "💡 Final Thoughts"
AAPS is a powerful, customizable alternative to commercial systems, but it demands technical effort, caution, and medical oversight. If you're comfortable with tech and want full control over your diabetes management, it could be life-changing!


<br><br>








<a href="https://maundyrelief.org.uk/" target="_blank">
 <center> <img width="300" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/585dd221-4f22-4e83-978d-3eedb39d3ca9" title="Maundy Relief"/>

<br>
<a href="https://www.diabetes.org.uk/" target="_blank">
 <center> <img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/21b87537-f1fa-4e01-904c-132085884544" title="Diabetes UK"/>
</a>               Why Not take visit <a href="https://www.diabetes.org.uk/support-us/fundraise/fundraising-events/pedal-for-progress" target="_blank"> UK Wide Cycle Ride - Diabetes.uk</a> **or** <a href="https://swim22.diabetes.org.uk/?fbclid=IwAR3XSygKTkbU7l_Xgu88WU3Q3EYFrFoAj1STvQTVz_6X-xthmjqOUWMTiww" target="_blank">Diabetes.UK Swim22:</a> **or** <a href="https://www.diabetes.org.uk/support-us/fundraise/fundraising-events/60-miles-challenge" target="_blank"> Diabetes UK Month of Miles Challenge</a> for all of your Diabetes Needs!
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
		

Adding a Green Highlighter with Bold too:
<span style="background-color:rgb(88, 121, 72)">**(Settings - Apps - xDrip+)**</span>


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

*******************		
external link
******************

# <center>Part 4: <a href="https://atlas-night-out.github.io/xdrip-Nightscout-AAPS/user-guide/Fork_and_Deploy_cgm_remote_monitory_part4/" target="_blank" title="Fork and Deploy cgm remote monitory Part 4">Fork and Deploy cgm remote monitory</a> </center>

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




Adding white space:

&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#26AF06">**Gear**</span> &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#26AF06">**Settings**</span>

-->

