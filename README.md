# Windows-Tricks-and-Tips
Windows Tricks and Tips

Windows Tricks and Tips
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**To check if your windows is legit or pirated version:**
•	Run Cmd as administrator.
•	Type slmgr /xpr 
  if result shows permanently activated: Its good
   If it shows some date and time: its pirated version.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**To Scan for viruses:**
•	Windows + r
•	Type mrt
•	Ok
•	Then follow instructions. 

**To refresh screen and drivers (If screen turning black)**
•	Press these at once: Windows + Shift + Ctrl + B
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**If your computer is running slow and you want to make  Faster:**
  Step 1:
    •	Press windows + r
    •	Type msconfig
    •	Go to Boot option.
    •	Go to Advanced 
    •	Check the Number of Processors option.
    •	Select 8 from the drop-down list. 
    •	Apply
  Step 2:
    •	Run Cmd as Administrator
    •	Type wmic
    •	If statis is OK  Hard disk is fine
    •	If any error:
      	Type exit
      	Type chkdsk
    •	This scans and fix any errors that could have been on hard disk. 
  Step 3:
    •	Press win + r
    •	Search for %TEMP%
    •	Delete all those appeared junky files. 
    •	This will clear unwanted files to assist in making computer faster. 
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**To check full specs of a Computer:**
•	Press Win + r
•	Search for msinfo32

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**To Activate Windows 11 pro for free:**
  Run Cmd as Administrator 
  Type slmgr.vbs /upk
    Now it will give a message, click on OK      
  Type slmgr.vbs /cpky
  	It will give an message once again, and click on OK again
  Type slmgr.vbs /ckms
  	Once again click on OK when you get a message.
   
  Now we will check if edition is supported to upgrade to Pro, run the following command to check this: DISM /online /Get-TargetEditions If you see "Professional" in the list, then you can upgrade your Windows edition to Pro for free!
  
  Now type these commands one after the other followed by enter key on Cmd prompt: 
  
  sc config LicenseManager start= auto & net start LicenseManager
  
  sc config wuauserv start= auto & net start wuauserv
  
  changepk.exe /productkey VK7JG-NPHTM-C97JM-9MPGT-3V66T
  
  exit
  
  This will run an installer that shows % complete. Let it complete and restart. If you encounter any error, that’s normal too, just click exit and restart the computer. 
  
  But we are not done, You will see that it isn't activated and that you can't change some settings, now we are gonna fix that!
  
  Once it restarts, Run Command prompt as Administrator again.
  
  Type these commands one after the other followed by enter key. 
  
  slmgr /ipk W269N-WFGWX-YVC9B-4J6C9-T83GX
  
  slmgr /skms kms8.msguides.com
  
  slmgr /ato
  
  Congratulations. You have finally activated Windows 11 pro. You can check it at: Settings//Systems//Activation. (Activation can be found under Updates and security in Windows 10)
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Activate Microsoft Office using Microsoft Activation Scripts(MAS)
Method 1 - PowerShell (Recommended)
•	Open Powershell (Not CMD). To do that, right-click on the start menu and select PowerShell or Terminal.
•	Copy and paste the code below and press enter
irm https://get.activated.win | iex

or (deprecated, will be retired on Dec 31 2024, use above instead)
irm https://massgrave.dev/get | iex

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

