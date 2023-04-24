# LeftClickTools

**Powershell GUI that allows troubleshooting and Remote actions on Pc's.**

• Add a computer one at a time either by hostname or IP.

• Add Multiple computers by using the "Import List" feature.  Just create a .txt document in notepad and add 1 computer per line.  

  This works on remote computers in your ORG, as well as the local machine.  All information is displayed in an output box, as well as outputting to a more verbose log on the users desktop.  It uses whoever is running the powershell applications credentials to manipulate machines, so it is in no way an incognito or "Hacking" tool.  All actions are also logged on the remote machine in the event viewer of that machine with whoever opened the tool listed as the owner of that action.  


I used Base64 to encode the images in this powershell gui to make sure it had no dependencies.


![image](https://user-images.githubusercontent.com/115837132/234049643-bef52e26-e11c-464d-ab1d-91d1a7436a91.png)




There are several actions that will not work if you do not change the name of your domain in the code. I have placed a tag of < YourDomain > in the code.  In order to use all of the features, do a ctrl+F and replace all the <YourDomain> tags with your actual domain.  

U:or Z: Is a generic mapping for a company network share.  You will also need to modify this for your org.  Ive also included the < SharedDrive> tag to help you find this and change it to reflect your network share in the code.  


LOCAL TOOLS SECTION:
Current Registry Tweaks:

Button 1. DISM Repair: Deployment imaging and service management Tool Generally for Windows images and VHD files, but has the ability to find problems with a local windows image as well. It will copy down critical core files required to run from Microsoft and gather information, then upgrade or repairs any files that are corrupted or out-of-date.

Button 2. Run SFC - Runs the System File Checker tool is best to run this after running the DISM Repair Tool. This finds corrupt files or incorrect windows files by checking the hash of the file, then repairs them.

Hiberboot Disable - Disables deep hibernation. This can help resolve a computer not going to sleep when closing the lid. Or extremely slow shutdown times

Hiberboot Enable - Runs the reverse of the previous action.

Disable WSUS - Allows your computer to check for online windows updates, and not just use your companies WSUS server. If you have a Group policy in place that allows your computer to only point to your local server for windows updates, this will only work until the GPO kicks back in. (Depending on your heartbeat, around 15 minutes.)

Enable WSUS - Runs the reverse of the previous action.

Disable Search Highlights - Disables the ads in the search bar.

Enable Highlights - Runs the reverse of the previous action.

AllowUpgrades - Allows getting the Windows 11 Upgrade natively through Microsoft Windows Updates, even if the CPU and TPM is not listed as compatible or recommended. This is a built in Registry key from Microsoft and is not considered a "Hack" to make it work.

Dissallow Upgrades - Runs the reverse of the previous action.

Disable Bing - Disables Bing in the search Bar.

Enable Bing - Runs the reverse of the previous action.

Get Serial Number - Gets the serial number (Service Tag) of the current machine.
  
  --------------------------------------------------------------------------------
  Local Machine Registry Tweaks
  --------------------------------------------------------------------------------
  
  Current Registry Tweaks:

Button 1. DISM Repair: Deployment imaging and service management Tool Generally for Windows images and VHD files, but has the ability to find problems with a local windows image as well. It will copy down critical core files required to run from Microsoft and gather information, then upgrade or repairs any files that are corrupted or out-of-date.

Button 2. Run SFC - Runs the System File Checker tool is best to run this after running the DISM Repair Tool. This finds corrupt files or incorrect windows files by checking the hash of the file, then repairs them.

Hiberboot Disable - Disables deep hibernation. This can help resolve a computer not going to sleep when closing the lid. Or extremely slow shutdown times

Hiberboot Enable - Runs the reverse of the previous action.

Disable WSUS - Allows your computer to check for online windows updates, and not just use your companies WSUS server. If you have a Group policy in place that allows your computer to only point to your local server for windows updates, this will only work until the GPO kicks back in. (Depending on your heartbeat, around 15 minutes.)

Enable WSUS - Runs the reverse of the previous action.

Disable Search Highlights - Disables the ads in the search bar.

Enable Highlights - Runs the reverse of the previous action.

AllowUpgrades - Allows getting the Windows 11 Upgrade natively through Microsoft Windows Updates, even if the CPU and TPM is not listed as compatible or recommended. This is a built in Registry key from Microsoft and is not considered a "Hack" to make it work.

Dissallow Upgrades - Runs the reverse of the previous action.

Disable Bing - Disables Bing in the search Bar.

Enable Bing - Runs the reverse of the previous action.

Get Serial Number - Gets the serial number (Service Tag) of the current machine.
