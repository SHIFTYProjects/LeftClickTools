# LeftClickTools

**Powershell GUI that allows troubleshooting and Remote actions on Pc's.**

• Add a computer one at a time either by hostname or IP.

• Add Multiple computers by using the "Import List" feature.  Just create a .txt document in notepad and add 1 computer per line.  

  This works on remote computers in your ORG, as well as the local machine.  All information is displayed in an output box, as well as outputting to a more verbose log on the users desktop.  It uses whoever is running the powershell applications credentials to manipulate machines, so it is in no way an incognito or "Hacking" tool.  All actions are also logged on the remote machine in the event viewer of that machine with whoever opened the tool listed as the owner of that action.  


I used Base64 to encode the images in this powershell gui to make sure it had no dependencies.


![image](https://user-images.githubusercontent.com/115837132/229212873-5bcc06c8-475c-4edc-8d33-604625aa7ab3.png)


There are several actions that will not work if you do not change the name of your domain in the code. I have placed a tag of < YourDomain > in the code.  In order to use all of the features, do a ctrl+F and replace all the <YourDomain> tags with your actual domain.  

U:or Z: Is a generic mapping for a company network share.  You will also need to modify this for your org.  Ive also included the < SharedDrive> tag to help you find this and change it to reflect your network share in the code.  
