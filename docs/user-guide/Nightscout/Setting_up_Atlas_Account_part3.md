<!-- this is on github live server !
docs made by D.Galloway 2019- 2021-->

# Welcome to The Diabetic way
For full Website content visit [The Diabetic Way](https://www.thediabeticway.co.uk/index.php/en/).
<br>
<br>

<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/a1a2f138-e0aa-4cd7-ad22-1738fd6206f8" title="Setting up Atlas Part 3"/></a><br><br>


## **Part 3 Setting up a Atlas Account for Nightscout**<br><br>


###1. **Now Open another tab**  to make a Mongodb Atlas Account: <a href="https://www.mongodb.com/cloud/atlas" target="_blank" title="Click Try Free">See Here</a> 

  and **click** <span style="background-color:#26AF06">**Start Free**</span><br>


<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/62e08cd7-4986-4016-983d-064b189a52bc" title="Sign up a Atlas Account"/></a><br><br>

###2. Enter your Account Details like I have and then click <span style="background-color:#26AF06">**get started free**</span> 

<img width="Auto" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/1dd69af5-8f4d-40a3-9f69-2867c8e34646" title="Setting Up a Free  Atlas Account"/></a><br><br>

###3. Atlas will send you an email, if you don't receive it check your Spam folder.<br>

###4. Now verify your email<br>

<img width="400" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/6e940771-e52c-45d0-88b2-fb2514ba7e21" title="Verify your email"/></a>


###5. Enter some information like I have below and then Finish <br>

  <img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/d2c8cd18-bc37-4a8f-9f1d-d152843c4496" title="Welcome to Atlas"/></a>

###6. Select Create a cluster in <span style="background-color:#26AF06">**Shared Clusters (FREE)**</span><br>

<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/de418612-4427-4fe7-868a-671ddc06c85a" title="Deploy a Cloud Database Free"/></a>

  

###7. Leave all default values and click <span style="background-color:#26AF06">**Create Cluster**</span><br>

<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/1aaa6216-a095-4422-a622-c1061cde541d" title="Create Shared Cluster"/></a><br><br>

  Atlas will create your default cluster, wait until it is complete... (can take more than 3 minutes) If not sure after a while click on the leaf icon in the top left!<br><br>


###8.  Click on <span style="background-color:#26AF06">**CONNECT**</span><br>

<img width="Auto" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/990d1930-9f54-4bef-81cd-ba62b6b5db92" title="click on connect"/></a><br>

    

    
###9. Click on <span style="background-color:#26AF06">**Allow Access from Anywhere**</span><br>

<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/8ad830dc-a35a-445c-b2b6-85072a44e3cd" title="Allow Access from Anywhere"/></a><br><br>


!!!warning "Allow Access Risks"  
    If you don't allow access from anywhere (IP 0.0.0.0/0) Nightscout will not be able to access your database.!

   <br>

###10. Click on <span style="background-color:#26AF06">**Add IP Address**</span><br>

<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/bea43786-1fee-4d5c-a9d9-b43fa80d567d" title="Add IP Address"/></a><br><br>

   
!!!warning "Database Details Risk"  
    Make sure not use your Atlas account Account details. <br>Do not use special characters: only letters and numbers. No spaces.

   <br><br> 

###11. Add a database username (In my example <span style="background-color:#26AF06">**nightkai**</span>) and a database user password (In my examples below <span style="background-color:#26AF06">**Madeuppassword7**</span>) but please change it later, see both images below!!<br><br>


<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/e174366f-429e-476d-b87b-6fe171e0df6e" title="Add IP Address"/></a><br><br>


###12. Then click <span style="background-color:#26AF06">**Create Database User**</span>.<br>


<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/4ee208b4-54e5-418d-aa58-6cd1ee0630fd" title="create database user"/></a><br><br>


!!!warning "Keep Safe"  
    Make sure you write these details down in a safe place, you are going to need them later in the boxes below to make your <span style="background-color:#26AF06">**Connection string**</span> Which I will explain further down, on this process!<br> <span style="background-color:#26AF06">**db user**</span> and <span style="background-color:#26AF06">**db user password!**</span><br><br>


###13. Click on  <span style="background-color:#26AF06">**Choose a Connection Method**</span><br>

<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/1db2e288-a627-4507-ad7d-ff49d734cd86" title="connection method"/></a><br><br>

###14.  Now Select <span style="background-color:#26AF06">**Connect your application**</span><br>

<img width="600" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/4e884808-a9f9-44fa-b127-022b559f03b1" title="Connect your application"/></a><br><br>

###15. Copy the <span style="background-color:#26AF06">**Connection string**</span> click Copy icon and paste it somewhere to edit it later(like Notepad, or Notepad++).<br>

<img width="Auto" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/231f132f-4179-445d-a9e0-6545bf0dd0f5" title="connection string"/></a><br><br>


!!!Note "Note! It should be similar to this - cluster0 (xxxxx) yours will be different"  
    mongodb+srv://nightkai:password@cluster0.xxxxx.mongodb.net/myFirstDatabase?retryWrites=true&w=majority<br><br>

    
``` { .yaml .copy }
mongodb+srv://nightkai:password@cluster0.xxxxx.mongodb.net/myFirstDatabase?retryWrites=true&w=majority
```
<br><br>

###16. Make up a name for your database, this is not  important information (just an example kdatabase ), note that default is <span style="background-color:#26AF06">**myFirstDatabase**</span><br>

###17. I will try to give you an example about the way to do this in the boxe's belows with my explanations on how to do it.<br>

####A. In the boxes below I have made for you to use.<br> 1st is your Atlas Account, you gave yourself a <span style="background-color:#26AF06">**User Name**</span> add it to the box below User Name on the left side!<br>

####B. You also made a <span style="background-color:#26AF06">**Database user Password**</span> so add your Password you created for your database in the box below, in the box on the left side removing mine I have put there to show you has an example!.<br>

####C. For the Cluster0 xxxxx where everyones will be unique when making a cluster when it is made so yours needs to be added into the Connection string part after it says Cluster0<br>

####D. And lastly you made up a <span style="background-color:#26AF06">**Database Name**</span> , also add this in to the last box, on the left side and click the <span style="background-color:#26AF06">**Generate button**</span>  which will then generate your <span style="background-color:#26AF06">**Connection String Code**</span>, that you will  need to add it in to your Heroku settings reveal Config Vars Mongo URI Section after you make it in the boxes below.
<br><br>


!!!Note "Note! Example Method for you to use! To make your Mongo URI Connection String"  
    I have given you my examples below on the right side of the  boxes so just ignore them they are my examples to show you how the connection string is made up! <br>
     You need to had your own details into the left side Boxes making sure to remove mine (click in the box's below, delete and put your own in place of mine!)first, and click on Generate.<br><br>



</font>
<br><p>
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


<br>
####E. After you have generated your code, it should be looking somthing similar to the one below.<br> Mine might be a little different to what yours should be so do check it carefully, and make sure to copy and paste it into notepad like I will explain and show you in the video below for you<br>

### **My Connection String results**

``` { .yaml .copy }
mongodb+srv://nightkai:Madeuppassword7@cluster0.j2iil.mongodb.net/kdatabase?retryWrites=true&w=majority
```
<br>
!!!warning "Warning"  
    Keep this Connection String in a safe place, it is called your MONGODB_URI and you will need it for your Heroku Account Config Vars<br><br>

The Diagram below, explains a little more  on how to do it yourself. <br>

<img width="Auto" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/3ae9b9fa-7ee2-4a44-a06c-2576e1ed9a01" title="how to make connection string"/></a>
<br>



<script>
function myFunction() {
  document.getElementById("field3").value = document.getElementById("username").value;
  document.getElementById("field4").value = document.getElementById("dbpassword").value;
  document.getElementById("field5").value = document.getElementById("dbname").value;
  document.getElementById("field6").value = document.getElementById("@cluster").value;
  
}
</script><br><br>


<table width="1166" Height="485 border="1" style="border-color: #000000; background-color: #ffffff;" cellpadding="1" cellspacing="1" height="98">
<tbody>
<tr style="height: 16px;">
<td style="width: 1158px; border-color: #000000; background-color: #5B9BD5;" fff="" ><span style="font-size: 14pt;"><span style="color: #ffffff; ">video demo of getting connection string,</span></span></td>
</tr>
<tr style="height: 56.4063px;">
<td style="width: 1158px; border-color: #000000;"><span style="font-family: tahoma, arial, helvetica, sans-serif; font-size: 14pt;">
 <iframe id="video3" width="860" height="615" src="https://www.youtube.com/embed/iYnNddVSbzY?start=19" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</tr>
</tbody>
</table><br>


****************************************************************************************
   
####A. If you want to do it manually: replace <password> with your database password as noted previously (in the example below **Madeuppassword7** ) and <dbname> by any text you want to add as your **database name**, say kdatabase in my example. The result will be like this:<br>

 <img width="Auto" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/3ae9b9fa-7ee2-4a44-a06c-2576e1ed9a01" title="how to make connection string"/></a>


###  Another example for you below!

<img width="Auto" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/c070ebe4-9e5e-46aa-be43-60059ffe84ec" title="connecting to cluster"/></a><br><br>

!!!Note "Note! "  
    There are no < and > characters in the final string, neither for password nor for the database name. You need to remove them!<br><br>

<br>

## <center>Now we need to do <br></center>
<br>
# <center>Part 4: <a href="https://atlas-night-out.github.io/xdrip-Nightscout-AAPS/user-guide/Nightscout/Part%204%20-%20Fork%20and%20Deploy%20cgm%20remote%20monitory/" target="_blank" title="Fork and Deploy cgm remote monitory Part 4">Fork and Deploy cgm remote monitory</a> </center>

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
  ****************************************************************************************************************
  
  
   
</font>
 

Check what version you are upto on your Nightscout site. In my example I'm on version  14.06 (Liquorice)

<table width="1166" border="1" style="border-color: #000000; background-color: #ffffff;" cellpadding="1" cellspacing="1" height="98">
<tbody>
<tr style="height: 16px;">
<td style="width: 1158px; border-color: #000000; background-color: #5B9BD5;" fff=""><span style="font-size: 14pt;"><span style="color: #ffffff;">Note! video, see below</span></span></td>
</tr>
<tr style="height: 56.4063px;">
<td style="width: 1158px; border-color: #000000;"><span style="font-family: tahoma, arial, helvetica, sans-serif; font-size: 14pt;">
<iframe width="850" height="415" src="https://www.youtube.com/embed/MFsbm45b6YY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>  </span></td>
</tr>
</tbody>
</table>



Updating your website to the latest version
 <a href="https://github.com/nightscout/cgm-remote-monitor/releases" target="_blank" title="Nightscout Release Versions">See Here</a> for the 
 current released version at moment) is easy with the update tool linked below. 
  
  
  
  
  
  
  
  
  
  ********************************************************************************************************************************
  mkdocs.yml    # The configuration file.
    docs/
    index.md  # The documentation homepage.
       ...       # Other markdown pages, images and other files.
		
		
	**************************
  Links
  ******************************	
<a href="http://nightscout.github.io/pages/update-fork/" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="/img/Nightscout/Time to Update Nightscout.png" title="Update Tool"/></a>		
		

*******************		
external link
******************

# <center>Part 4: <a href="https://atlas-night-out.github.io/xdrip-Nightscout-AAPS/user-guide/Fork_and_Deploy_cgm_remote_monitory_part4/" target="_blank" title="Fork and Deploy cgm remote monitory Part 4">Fork and Deploy cgm remote monitory</a> </center>


*****************************************************************

adding 	Yellow Hightligher!!!!!!!!	
<span style="background-color: #FFFF00">**Marked text**</span>


adding 	Green Hightligher!!!!!!!!	with bold too

<span style="background-color:#26AF06">**Later**</span>


****************************************************************
adding an image
***********************

  <a><img width="auto" height="auto" border="0" align="center"  src="/img/Nightscout/Time to Update Nightscout.png" title="Update Tool"/></a>	




<a href="https://www.youtube.com/watch?v=MFsbm45b6YY" target="_blank">
  <img width="auto" height="auto" border="0" align="center"  src="/img/Nightscout/nightscout version_14.06.jpg" title="Version of Nightscout Video"/>
</a>

*******************************************************************************
Adding Video

<iframe width="850" height="415" src="https://www.youtube.com/embed/MFsbm45b6YY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Note
**Note:** a note is something that needs to be mentioned but is apart from the context.

***************************************************************************************
Adding a copy code block

``` { .yaml .copy }
mongodb+srv://nightkai:password@cluster0.xxxxx.mongodb.net/myFirstDatabase?retryWrites=true&w=majority
```


**********************************************************************************************

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




*******************************
Table
| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |


************************************************************
adding a space

&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;

******************************************************************


-->

