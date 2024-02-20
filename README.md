
# PLD Bypass
*updated 20/2/2024*

A guide on how to bypass restrictions on Singapore Personal Learning Devices (PLD) for Secondary schools. This only works for iPads and not Chromebooks or Microsoft Surface devices. (Though for Surface you can use a windows2go drive or any other bootable OS!)

## Note
I'm not responsible if you get your ass beat. Don't get caught. If they do a class where they check your iPads, power it off and say you have no battery, or just don't bring it at all.

This process factory resets your iPad, meaning everything you have on there will be gone. You can of course back your files up if you want to.

## Requirements
1. A relatively modern Apple Computer running Big Sur or higher with SIP disabled. [How to check your macOS version](https://support.apple.com/en-sg/109033) & [How to disable SIP.](https://developer.apple.com/documentation/security/disabling_and_enabling_system_integrity_protection)


2. Lightning cable, aka the cable that came with your iPad

3. Basic computer literacy


## Prerequisites

(This is only for my school, your school may be similar, may be not.)
1. Make sure you can login to your school Microsoft account (OneNote, OneDrive, Teams etc) for your schoolwork. [Check your ability to log in.](https://www.onenote.com/hrd)

2. Know your MIMS password. This is needed for WiFi in school. [Check your ability to log in.](https://idp.mims.moe.gov.sg/nidp/app/login) Of course you can just use your phone's hotspot too.

3. (Optional) Backup your files, such as photos and homework. There are two ways to do this, via AirDrop or the aforementioned cloud storage. With AirDrop, you can simply transfer the files and photos you want to keep to your Mac or another Apple device then AirDrop it back once this process is finished. You do not need to backup your OneNote notebooks, as they are stored with in the cloud and not locally.

4. Have the [MDM patcher downloaded and installed.](https://github.com/j4nf4b3l/MDMPatcher-Universal/releases/download/v1.0/MDMPatcher_Universal_v1.dmg) To fix "This app cannot be opened as it is from an unidentified developer" go into System Settings, Security & Privacy and click open anyway. (You may need to scroll down, if you do not see it, close the popup first.)

5. A IPSW (iOS firmware file) downloaded. [Choose your device and download the latest version.](https://ipsw.me/product/iPad)

6. Your personal Apple ID. Do not use your school one.


## Bypassing

1. Plug your iPad into your computer via the lightning cable and hold both the power button and home button until you see [this screen.](https://cdsassets.apple.com/live/7WUAS350/images/ipad/ipad/recovery-mode-ipad-pro-face-id.png)

2. Finder should open with a popup saying that your iPad has a [problem and needs to be restored or updated.](https://cdsassets.apple.com/live/7WUAS350/images/mac-os/monterey/macos-monterey-finder-update-restore-ipad-finder.png) Close this popup.

3. Hold down Option (Alt on Windows keyboards) and click Restore. Select the IPSW file you downloaded.

4. Wait. Restoring takes a while.

5. Once your iPad shows the [hello screen](https://help.apple.com/assets/65691320E7FC42EA3F02A1D8/6569132237A5D113A9082F2E/en_US/b3e222b3c922318d01364ad0cd4cfbfb.png), open finder and find your iPad and make sure that you see somthing similar to [this screen.](https://www.cnet.com/a/img/resize/af53a594388baea1a341940f63091ad62fcf48a9/hub/2017/08/30/a4096c4b-d91f-4177-a798-88e1c7c6d991/itunes-restore-from-backup.jpg?auto=webp&width=1200)

6. Open MDMPatcherUniversal and click patch. 

7. You're done!

## Post-requisites
 1. Apps for school
   1. Microsoft OneNote
   2. Microsoft Teams
   3. Microsoft OneDrive
   4. Microsoft Word
   5. Microsoft PowerPoint
   6. Microsoft Excel
   7. Kahoot (Optional)
   8. Padlet (Optional)
 2. Connecting to school WiFi
      Connect to SWN@SSOE and use your MIMS account to log in.

## Troubleshooting
If your device keeps blinking in the sidebar and is just acting glitchy in general, open Terminal and put in this command `sudo killall -STOP -c usbd` and type in your account password. Note that your password will not appear, and it is normal.
