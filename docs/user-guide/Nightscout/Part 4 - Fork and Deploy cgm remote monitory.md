<!-- this is not on github server its local only and run my mkdocs server!
docs made by D.Galloway 2019- 2021-->
# Welcome to The Diabetic way
For full Website content visit [The Diabetic Way](https://www.thediabeticway.co.uk/index.php/en/).
<br><br><br>


<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/9e91983d-cde2-4a54-988c-73cdb72c3ea2" title="Fork and Deploy cgm remote monitory Part 4"/></a>
<img width="auto" height="auto" border="0" align="center"  src="/xdrip-Nightscout-AAPS/img/Fork and Deploy cgm remote monitory Part 4/Fork_and_Deploy_cgm_remote_monitory_Part_4t_860x462.jpg" Setting up Atlas Part 3"/>

## **Part 4 - Fork and Deploy cgm remote monitory  **<br><br>
## If you would like to follow these instructions with video then see below other wise continue step by step below<br>
<br>

<table width="1166" height="560" border="1" style="border-color: #000000; background-color: #ffffff;" cellpadding="1" cellspacing="1" height="98">
<tbody>
<tr style="height: 16px;">
<td style="width: 1158px; border-color: #000000; background-color: #5B9BD5;" fff=""><span style="font-size: 14pt;"><span style="color: #ffffff;">video Instructions,</span></span></td>
</tr>
<tr style="height: 56.4063px;">
<td style="width: 1158px; border-color: #000000;"><span style="font-family: tahoma, arial, helvetica, sans-serif; font-size: 14pt;">
 <iframe id="video3" width="860" height="615" src="https://www.youtube.com/embed/mEilmCDz1pc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> </span></td>
</tr>
</tbody>
</table><br>
!!!Note "Note! "  
    If you have already forked your  cgm-remote-monitor, before reaching this stage, you should delete the existing cgm-remote-monitor repository before proceeding.<br>
    Delete your current cgm-remote-monitor fork using <a href="  https://youtu.be/tUoWQ7ns2sA" target="_blank" title="Video showing you how to delete your cgm-remote-monitor">Video STEP</a>
    

 
<br>  

###1. Hopfully you should now have 3 pages opened in your browser: <span style="background-color:#26AF06">**Heroku, Atlas, and Github,**</span> Make sure you are logged-in on each one of them <span style="background-color:#26AF06">**i.e. important**</span> before you continue.

###2.  <a href="https://github.com/nightscout/cgm-remote-monitor" target="_blank" title="Nightscout Release Versions">Click Here</a> to go to Nightscout Repository  or copy the link below to go to open a new GitHub Nightscout Repo<br>

``` { .yaml .copy }
https://github.com/nightscout/cgm-remote-monitor
```
<br>

###Click the on fork icon in the top right, making sure your not in your own Repository and in Nightscouts! <br>

<img width="Auto" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/132c949e-b716-41fe-b249-f570eddae052" title="Nightscout Repository"/></a>
   

###3. Wait for a moment

<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/cdcbec57-62fb-4765-99a1-11cfe50338a6" title="forking"/></a>
  
   
###3.1. Scroll down the page and click <span style="background-color:#26AF06">**Deploy to Heroku**</span>


<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/291ec0c5-f12f-4ad8-8916-d0ba5238643b" title="Deploy to Heroku"/></a><br>

  
   
###4. Enter in your Heroku account a site name: invent a name you would like to use or see your BG in on the internet. Confirm that the name is available.

<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/af544cd3-beca-4c04-8ffe-0e81aa5c6320" title="site name"/></a><br>
 
 
###5.  Don’t change the region.

###6. <span style="background-color:#26AF06">**Scroll down**</span> and setup the following variables: You can come back to these later later by going to settings and config Vars Enable in Heroku!<br>

<img width="400" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/50a85cb1-faa2-4ec1-a0d1-85f260a62c02" title="API SECRET Required2"/></a>
     <iframe width="800" height="415" src="https://www.youtube.com/embed/65KI5-3E_XM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe><br>
	 
!!!Note "Note! "  
    The API_SECRET is the main password allowing full access to your Nightscout site. Make sure its secure (mix upper and lowercase letters, plus digits) and do no not share it publicly. If you think you exposed it by mistake, it is recommended that you change it.</a><br>


###7. <span style="background-color:#26AF06">**API_SECRET**</span> is your Nightscout site password; it must be at least 12 characters.  <span style="background-color:#26AF06">**Avoid spaces when using @ or ! symbols,**</span> as you may need to use Percent encoding in uploader and downloader apps.<br>
###If unsure, it's best to use only <span style="background-color:#26AF06">** letters (uppercase and lowercase)**</span>and digits.<br>


<img width="600Auto" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/43446774-5b75-4971-8fda-f7bd56a302e3" title="API SECRET Required"/></a><br><br>



###8. If you <span style="background-color:#26AF06">**want to link your Dexcom Share account**</span> as a data source, complete the following 3 lines:<br>

<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/d3c6473c-3a2e-4e7f-9982-84fa991139b1" title="bridge for Dexcom share"/></a><br>
<br>

!!!warning "Warning Common Errors"  
    The BRIDGE_PASSWORD and BRIDGE_USER_NAME are NOT visible from within your Dexcom app or online account. These values are what you entered into your Dexcom mobile app when you logged into that app for the VERY FIRST time. The BRIDGE_USER_NAME is not an email address. The most common error on initial Nightscout setups is that people incorrectly use an old account or an old password.<br> To test your username and password, go to Dexcom's Clarity page (check here <a href="https://clarity.dexcom.com/" target="_blank" title="Dexcom USA Account">See Here</a> for USA accounts and <a href="https://clarity.dexcom.eu/" target="_blank" title="Dexcom EU Account"> Here</a> here for the others) and try logging in to your Dexcom account. If your account info isn't valid, or you don't see any data in your Clarity account... you need to figure out your actual credentials before moving ahead.<br><br>



###9. If you want to link your <span style="background-color:#26AF06">**Care Link account**</span> as a data source (currently not functional with Heroku), complete the following lines:<br>

<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/bc1f4432-9664-49d3-adba-8666a14e077f" title="mmconnect"/></a><br>

###10. Select the units you’re using in <span style="background-color:#26AF06">**DISPLAY_UNITS**</span> the acceptable choices are <span style="background-color:#26AF06">**mg/dl or mmol/L**</span> (or just <span style="background-color:#26AF06">**mmol**</span> when entering it).<br>

<img width="500s" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/0008938a-fddd-4027-be89-b4fded2c0cb2" title="display units"/></a><br>

<br>
In <span style="background-color:#26AF06">**my case I used mmol**</span> >br>

<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/1ce85144-7af3-4155-bb52-4439d6f800b3" title="display unit EU"/></a>



## Plugins <br>

###11.    In <span style="background-color:#26AF06">**ENABLE**</span> copy and paste the following Plugins below <span style="background-color:#26AF06">**(separated by a space)**</span> so that won't have to think about which you want now and learn the rest later!<br><br>
**Plugins I added to config var Enable**<br>

<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/b0e19115-de96-430c-9ec0-465fdbb076b8" title="enable"/></a>
><br>

 **Plugins I added**<br>

``` { .yaml .copy }
careportal boluscalc food  rawbg iob cob bwp cage sage iage bage treatmentnotify basal (Basal Profile) bolus connect pump openaps loop override xdripjs alexa googlehome speech cors
```

careportal boluscalc food  rawbg iob cob bwp cage sage iage bage treatmentnotify basal (Basal Profile) bolus connect pump openaps loop override xdripjs alexa googlehome speech cors <br><br>

!!!Note "Note! "  
    If you are using your Dexcom share account as a data source add a bridge at the end of your plugins, after a space like this: careportal basal dbsize rawbg iob maker cob bwp cage iage sage boluscalc pushover treatmentnotify loop pump profile food openaps bage alexa override speech cors <span style="background-color:#26AF06">**bridge**</span><br>



<br>
###12. Now you need the <span style="background-color:#26AF06">**connection string**</span> you defined during the <span style="background-color:#26AF06">**Atlas cluster creation - Part 3**</span> (as the example below, but not the string below). Copy and paste your results into the MONGODB_URI variable field in Heroku Config vars.<br><br>

<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/3051a0b5-d174-482f-b62a-09355247937c" title="mongo uri"/></a><br>
	
###13. I will try to give you an example about the way to do it again below, you can also see my video if you get stuck!


<br>
####A. In the boxes below 1st is your Atlas Account you gave yourself a <span style="background-color:#26AF06">**User Name**</span> add it to the box below User Name on the left side!<br>

####B. Then you also made a <span style="background-color:#26AF06">**Database user Password add your Password**</span>you  created for your database add this too into the box on the left side.<br>

####C. And lastly you made up a <span style="background-color:#26AF06">**Database Name**</span>, also add this to the last box on the left and click the <span style="background-color:#26AF06">**Generate button**</span>  which will generate your <span style="background-color:#26AF06">**connection string code**</span> that you will  need to add to your Heroku API<br><br>


  
####	I have given you my examples below on the right side of the  boxes so just ignore them they are my examples to show you how the connection string is made up!

<span style="background-color:#26AF06">**username:**</span> <input type="text" id="username" value="click here, delete and put your own! " size="32">  Eg: username: <input type="text" id="egusername" value="nightkai" size="32"><br>
<br>
<span style="background-color:#26AF06">**Database password:**</span> <input type="text" id="dbpassword" value="click here,delete and put your own!" size="31">Eg: Database password: <input type="text" id="egdbpassword" value="   Madeuppassword7" size="20"><br>
<br>
<span style="background-color:#26AF06">**@cluster0:xxxxx**</span> <input type="text" id="@cluster" value="click here, delete and put your own! " size="32"> E.g: cluster0.xxxxx <input type="text" id="egdbname" value=" j2iil " size="20><br>output: <input type="text" id="output" value="click here, delete and put your own " size="32"><br>
<br>
<span style="background-color:#26AF06">**Database Name:**</span> <input type="text" id="dbname" value="click here, delete and put your own! " size="32"> E.g: Database Name: <input type="text" id="egdbname" value=" kdatabase " size="20><br>output: <input type="text" id="output" value="click here, delete and put your own " size="32"><br>
<br><br>
Now click on the <span style="background-color:#26AF06">**Generate**</span>,below! And see the boxes generate your Connection String Code for you!<br>

<button onclick="myFunction()">Generate</button><br><br><br><br>
<span style="background-color:#26AF06">**mongodb+srv://**</span> <input type="text" id="field3"value="User Name">
: <input type="text" id="field4"value="Database Password">
@cluster0.<input type="text" id="field6"value="cluster0.xxxxx ">.mongodb.net/ <input type="text" id="field5"value="Database Name">?retryWrites=true&w=majority<br><br>




### My Connection String results

``` { .yaml .copy }
mongodb+srv://nightkai:Madeuppassword7@cluster0.j2iil.mongodb.net/kdatabase?retryWrites=true&w=majority
```
<br>

<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/3ae9b9fa-7ee2-4a44-a06c-2576e1ed9a01" title="how to make connection string"/></a>


!!!warning "Warning"  
    Keep this Connection String in a safe place, it is called your MONGODB_URI and you will need it for your Heroku Account Config Vars - called your MONGODB_URI<br><br>


<br>
<script>
function myFunction() {
  document.getElementById("field3").value = document.getElementById("username").value;
  document.getElementById("field4").value = document.getElementById("dbpassword").value;
  document.getElementById("field5").value = document.getElementById("dbname").value;
  document.getElementById("field6").value = document.getElementById("@cluster").value;
  
}
</script><br><br>


<table width="1166" height="560" border="1" style="border-color: #000000; background-color: #ffffff;" cellpadding="1" cellspacing="1" height="98">
<tbody>
<tr style="height: 16px;">
<td style="width: 1158px; border-color: #000000; background-color: #5B9BD5;" fff="" ><span style="font-size: 14pt;"><span style="color: #ffffff; ">video demo of getting connection string,</span></span></td>
</tr>
<tr style="height: 56.4063px;">
<td style="width: 1158px; border-color: #000000;"><span style="font-family: tahoma, arial, helvetica, sans-serif; font-size: 14pt;">
 <iframe id="video3" width="860" height="615" src="https://www.youtube.com/embed/iYnNddVSbzY?start=19" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>  </span></td>
</tr>
</tbody>
</table><br>

###14. Once you have added your Connection string into the MongoDB_Uri. Scroll down to the bottom of the Config var list and click the <span style="background-color:#26AF06">**Deploy APP**</span><br>

### You will wait for a while for them completion. Do not stop  the process until it's complete.
<img width="500" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/ca4ed1ac-e22d-4904-9594-f20f95d1b2ac" title="select deploy app"/></a>	<br>

###15.  click the  <span style="background-color:#26AF06">**View button** </span>and it should come up (if not, then click the Manage App -> Open App, in the top right corner)<br>

<img width="500" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/b4b8831b-f068-4269-8710-9d06d9aa0ee3" title="click view"/></a>	<br>

###16. Your Nightscout site  should open and direct you to fill in profile editor for Nightscout.<br>
<img width="500" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/de9b5f8e-c349-4faa-8b7e-72f3a77598ce" title="profile editor"/></a>	<br>

###17. All you need to fill in at this moment in time is your <span style="background-color:#26AF06">**Time zone**</span> and eventually all the other fields e.g. Insulin to carbs. Make sure to not leave any fields empty. If you don't understand which value to use, just use the <span style="background-color:#26AF06">**default value**</span>.<br>

###a. You can come back and change these values later at any time by going to your  Nightscout URL selecting the <span style="background-color:#26AF06">**Hamberger icon**</span> on the right and selecting <span style="background-color:#26AF06">**profile editor**</span>.<br>

<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/83a3ca49-6a35-4a81-97af-6a82142c1f52" title="getting to nightscout profile editor"/></a>	<br>

###18. You will then need to go down to <span style="background-color:#26AF06">**Authentication Status**</span> on the left and click Authentication.  And enter your <span style="background-color:#26AF06">**Heroku API secret**</span> you made earlier. Then click <span style="background-color:#26AF06">**Time zone**</span> <span style="background-color:#26AF06">**Authenticate button**</span>, Then <span style="background-color:#26AF06">**save**</span>.<br>

<img width="400" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/82464ee5-0936-4abf-8d20-a305bca8cfc8" title="Authentication"/></a><br>

<img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/5a40fd30-c368-413e-a199-a99d23bad4a8" title="Api secret image"/>     </a><img width="150" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/944107ce-9305-4f6c-910c-c305138299de" title="save"/></a><br><br>


!!!warning "Warning"  
    Anyone with your URL of your Nightscout site, can view your values and run reports of your data. It is recommended that you enable <a href="http://127.0.0.1:8000/user-guide/Nightscout%20Safety%20Check/" target="_blank" title="Best to set security to your nightscout">security</a> to your site once you're done this setup.<br><br>


###19. Dexcom Share and CareLink users should see data working after a few minutes. <br>

Other uploaders like <span style="background-color:#26AF06">**xDrip+**</span>, <span style="background-color:#26AF06">**Gluroo**</span>, xDrip4iOS, Sugarmate,Jade, GlucoDataHandler etc will need to be setup with a Nightscout address and API secret in each Apps settings (<a href=" https://github.com/pachi81/GlucoDataHandler" target="_blank" title="see uploaders ">See Uploaders (Data Sources)</a><br><br>

##  Example:
## Nightscout Address for your Uploader Apps (Data Sources)<br>

<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/ae07b79c-c5f6-440f-89a2-38bc7d474cf7" title="Nightscout Address"/></a>><br>
## PAPERTRAIL<br>

####A. Lastly, you might want to change the PAPERTRAIL_API_TOKEN line. Heroku gives you a free, tiny amount of Papertrail service (this is like a logging service for how the site is running), but this generates a lot of confusion to most people later on.<br>

 when they get a message that their "Free Papertrail Service has run out of room". Papertrail is not needed at all, edit the line with the pensil icon and add <span style="background-color:#26AF06">**DISABLED**</span> at the end, so that you can recover the function if you need it later.<br><br>

 <img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/ecd60aa2-53cd-4e07-a8e7-5608b45615b7" title="PAPERTRAIL DISABLED"/></a><br>
<br><br>
<img width="Auto" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/ef33c5e3-afe7-4f04-bca6-6533afbada32" title="Nightscout"/></a><br><br>

<font size="6"> <center>**Congratulations Nightscout is now setup!**</center><br></font><br>

## Enable Auto Deploys in Heroku <br><br>
Automatic deploys will allow you to update routinely your Heroku apps when you renew the GitHub repository.
You will then not need to login into Heroku and execute Manual Deploy, as soon as do a new version of the repo be merged into GitHub an automatic deploy will trigger in all enabled Heroku apps.

a)	To allow automatic deploy, log in Heroku and select your app, in my case diabeticway and then selecting the <span style="background-color:#26AF06">**Deploy section**</span>.<br>

<img width="500" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/1e4c6c88-016c-40b8-9755-abcaaf4ebffb" title="Deploy heroku"/></a>

b)	 Select <span style="background-color:#26AF06">**Connect to Github**</span><br>

<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/57dbc9ab-f9da-468a-9a9b-6ac12bdeb7cd" title="connect to github"/></a>
	<br>

c) Authenticate GitHub and your cgm-remote-monitor app are now connected.
	<br>

d) Click on <span style="background-color:#26AF06">**search**</span> and add your repo name, it will then connect to Github<br>

<img width="500" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/425d0237-859e-42df-9a18-a2c8c2fb6919" title="search"/></a><br>

<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/c80919c0-e499-41cc-b15d-3b52554b8e29" title="repo name"/></a><br>


e) Verify the master branch is selected and click <span style="background-color:#26AF06">**Enable Automatic Deploys**</span>.<br>

<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/35b6c82a-19c8-46ab-af60-028619ed4c01" title="Verify the master branch"/></a>	<br>

f) Your site will <span style="background-color:#26AF06">**update automatically**</span> every time you update the GitHub repository now.<br><br>
<img width="500" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/da862108-3827-4c30-b798-855f801e0478" title="Verify the master branch"/></a>	<br><br>


**********************************************************************************************


## <center> If you have any issues or concerns please visit: </center> 
<font size="4"><center>
:simple-discord:<a href=" https://discord.gg/Gb5SF7jR" target="_blank" title="Discord"> Discord</a>&emsp; :simple-facebook: <a href=" https://www.facebook.com/groups/cgminthecloud" target="_blank" title="CGM in the Cloud on Facebook"> CGM in the Cloud</a> 🩸 <a href=" https://github.com/nightscout/AndroidAPS/issues" target="_blank" title="Nightscout "> Nightscout</a>&emsp; :simple-github:<a href=" https://github.com/nightscout/AndroidAPS?tab=readme-ov-file" target="_blank" title="Github AAPS"> Github AAPS</a> </center></font>
<br><br>


[&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;]()
[Please Subscribe to our UTUBE Channel](https://www.youtube.com/channel/UC9TwtBefjjKw_uKHiIWMkBA?sub_confirmation=1){ .md-button }

<br>
<a href="https://maundyrelief.org.uk/" target="_blank">
  <center><img width="300" height="auto" border="0" align=""  src="https://github.com/user-attachments/assets/585dd221-4f22-4e83-978d-3eedb39d3ca9" title="Maundy Relief"/></center></a>
<br><br>

<a href="https://www.diabetes.org.uk/" target="_blank">
<img width="auto" height="auto" border="0" align="center"  src="https://github.com/user-attachments/assets/21b87537-f1fa-4e01-904c-132085884544" title="Diabetes UK"/> </a>Why Not take visit <a href="https://www.diabetes.org.uk/support-us/fundraise/fundraising-events/pedal-for-progress" target="_blank"> :man_biking_tone1: UK Wide Cycle Ride - Diabetes.uk :woman_biking_tone5:</a> **or** <a href="https://swim22.diabetes.org.uk/?fbclid=IwAR3XSygKTkbU7l_Xgu88WU3Q3EYFrFoAj1STvQTVz_6X-xthmjqOUWMTiww" target="_blank">Diabetes.UK Swim22 :man_swimming_tone5:</a> **or** <a href="https://www.diabetes.org.uk/support-us/fundraise/fundraising-events/60-miles-challenge" target="_blank">:man_walking_tone5: Diabetes UK Month of Miles Challenge :woman_running:</a> for all of your Diabetes Needs!

  



   
   

 








  <!--  
  ******************************************************************************************************************
  mkdocs.yml    # The configuration file.
    docs/
    index.md  # The documentation homepage.
       ...       # Other markdown pages, images and other files.
		
		
		
<a href="http://nightscout.github.io/pages/update-fork/" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="/img/Nightscout/Time to Update Nightscout.png" title="Update Tool"/></a>		
		
		
*****************************************************************

adding 	Yellow Hightligher!!!!!!!!	
<span style="background-color: #FFFF00">**Marked text**</span>


adding 	Green Hightligher!!!!!!!!	with bold too

<span style="background-color:#26AF06">**Later**</span>


****************************************************************

link
<a href=" https://github.com/" target="_blank" title="First create a user account by going to">Click Here</a>

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

<table width="auto" border="1" style="border-color: #000000; background-color: #ffffff;" cellpadding="1" cellspacing="1" height="98">
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


***************************************************************************************
Adding a copy code block

``` { .yaml .copy }
mongodb+srv://nightkai:password@cluster0.xxxxx.mongodb.net/myFirstDatabase?retryWrites=true&w=majority
```


**********************************************************************************************



-->

