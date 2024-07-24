
# PLD Bypass
*updated 25/7/2024*

A guide on bypassing MDM and all other restrictions on Singapore Secondary School Personal Learning Devices (iPads).

## DISCLAIMER
### I am not responsible for any dead iPads, discipline cases, angry teachers/parents. This guide is purely for educational purposes only. 

### This process *FACTORY RESETS* your iPad, meaning that *ALL* local data will be irreversibly deleted.

### FOLLOW EVERY STEP, NONE OF IT IS OPTIONAL. YOUR IPAD WILL NOT BE BYPASSED IF YOU SKIP STEPS.

## Requirements
1. A relatively modern computer running MacOS 11 or higher with SIP disabled. [How to check your macOS version](https://support.apple.com/en-sg/109033) & [How to disable SIP.](https://developer.apple.com/documentation/security/disabling_and_enabling_system_integrity_protection) Hackintoshes and Virtual Machines with USB passthrough are supported if you do not have a Mac.


2. A USB-C or Lightning cable (depends on your iPad model) that supports data transfer 

3. Basic computer literacy
## Prerequisites


1. Make sure you can login to your school Microsoft account (OneNote, OneDrive, Teams etc) or any other account your school uses (Google Classrooms etc) for your schoolwork. If you are unable to, ask your form teacher to reset your password.

2. Know your MIMS password. This is needed for WiFi in school. [Check your ability to log in.](https://idp.mims.moe.gov.sg/nidp/app/login) Of course you can just use your phone's hotspot as an alternative. Do not connect to any other networks in your school as it may reinstall the restrictions

3. (Optional) Backup your files, such as photos and documents. There are two ways to do this, via AirDrop or cloud storage. Basically you just need to backup any local data that you still want.

4. Have the [MDM patcher downloaded and installed.](https://github.com/j4nf4b3l/MDMPatcher-Universal/releases/download/v1.0/MDMPatcher_Universal_v1.dmg) To fix "This app cannot be opened as it is from an unidentified developer" go into System Settings, Security & Privacy and click open anyway. (You may need to scroll down, if you do not see it, close the popup first.)

5. A IPSW (iOS firmware file) downloaded. [Choose your device and download the latest version.](https://ipsw.me/product/iPad)

6. A personal Apple ID. Do not use your school one.


## Bypassing

1. Boot your iPad into recovery mode. 
	1. Connect your iPad to your computer using a USB cable.
	
	For an iPad without a home button, press and quickly release the volume button closest to the power button. Press and quickly release the volume button furthest from the top button. Press and hold the top button.
	
	![](https://github.com/oopsitsdeleted/PLDBypass/blob/main/Assets/recovery-mode-ipad-face-id-ipad-mini-animation.gif?raw=true 1-1.png?raw=true)
	
	For iPads with a home button, press and hold both the Home and power button at the same time
	![](https://github.com/oopsitsdeleted/PLDBypass/blob/main/Assets/ipad-home-button-force-restart.png?raw=true?raw=true)
	
	Keep holding the button (or buttons) until you see the recovery mode screen:
	![](https://github.com/oopsitsdeleted/PLDBypass/blob/main/Assets/recovery-mode-ipad-pro-face-id.png?raw=true)
2. Finder should open with a popup, press cancel.

	![](https://github.com/oopsitsdeleted/PLDBypass/blob/main/Assets/Problem%20with%20this%20iPad.png?raw=true)
	

3. Hold down Option (Alt on Windows keyboards) and click Restore. Select the IPSW file you downloaded.

	![](https://github.com/oopsitsdeleted/PLDBypass/blob/main/Assets/iPad%20Finder%20page.png?raw=true)
	
	![](https://github.com/oopsitsdeleted/PLDBypass/blob/main/Assets/File%20Picker.png?raw=true)

4. Wait. Restoring takes a while.

	![](https://github.com/oopsitsdeleted/PLDBypass/blob/main/Assets/Restoring.png?raw=true)

5. Close the successfull iPad restore popup, leave it plugged in.
	
	![](https://github.com/oopsitsdeleted/PLDBypass/blob/main/Assets/Successfull%20restore.png?raw=true)
	

6. Go into iPad in the sidebar, if it's not there, wait. Wait for it to activate.

	![](https://github.com/oopsitsdeleted/PLDBypass/blob/main/Assets/iPad%20Activation.png?raw=true)
	
	![](https://github.com/oopsitsdeleted/PLDBypass/blob/main/Assets/iPad%20Activated.png?raw=true)

7. Open MDMPatcher Universal and click patch. Unplug your iPad after there's a success popup.
	
	![](https://github.com/oopsitsdeleted/PLDBypass/blob/main/Assets/MDMPatcher.png?raw=true)
	
	![](https://github.com/oopsitsdeleted/PLDBypass/blob/main/Assets/MDMPatcher%20success.png?raw=true)

8. Setup your iPad.

## Post-requisites
1. Install apps for school, such as:
	 1. Microsoft OneNote
 	2. Microsoft Teams
 	3. Microsoft OneDrive
 	4. Microsoft Word
 	5. Microsoft PowerPoint
 	6. Microsoft Excel
 	7. Google Classroom
 	8. Kahoot (Optional)
 	9. Padlet (Optional)
 	10. Connecting to school WiFi
      		Connect to SWN@SSOE and use your MIMS account to log in.

## Troubleshooting
If your device keeps blinking in the sidebar and is just acting glitchy in general, open Terminal and put in this command `sudo killall -STOP -c usbd` and type in your account password. Note that your password will not appear, and it is normal. Also, Google what errors you get, use sites like Reddit or other forums.
