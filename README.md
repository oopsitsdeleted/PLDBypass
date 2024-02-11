# PLDBypass
how to bypass Singapore's Personal learning devices (ipad 7th gen to 9th gen)

^(this is for educational purposes only dont sue)

# Requirements:

A Mac , a Hackintosh or a Virtual Machine in Linux with SIP disabled (How to disable SIP in [OpenCore](https://dortania.github.io/OpenCore-Install-Guide/troubleshooting/extended/post-issues.html#disabling-sip) and a [Genuine Mac](https://developer.apple.com/documentation/security/disabling_and_enabling_system_integrity_protection)) running macOS 10.13 or higher.

A genuine lightning cable

[A IPSW](https://ipsw.me/product/iPad) (Select your device and download a signed IPSW)

A iPad 9th gen or lower (Go into Settings > General > About if you do not know yours)

&#x200B;

I used a Intel ThinkPad running macOS Big Sur.

# Note:

Your PLD will be restored, basically all your data will be wiped. So you will need to know your passwords to your Microsoft OneNote etc. You will also probably not be able to connect to the school Wi-Fi (edit, you can use SWN@MOE (or something along those lines) and use your MIMS password.). You are also unable to restore this iPad via settings, as you will get the restrictions again. Updating should be fine though, as I updated from 17.0.1 to 17.2 Beta, but I recommend backing up your data first before attempting to.

# Instructions:

Firstly, you need to put your iPad into recovery mode. This can be done by plugging your device into your computer and powering it off. Once it is fully shut off, hold down the home button and power button together until you see the [recovery screen](https://support.apple.com/library/content/dam/edam/applecare/images/en_US/ipad/ipad/recovery-mode-ipad-pro-face-id.png). Finder should now appear saying that your iPad needs to be updated or restored. Just click 'Cancel'. Hold down the Option key (Alt if you're using a hackintosh or a Windows keyboard), click on Restore and select the IPSW you downloaded. Your iPad should now be restoring. Do not unplug it.

Open MDMPatcher Universal and wait for your iPad to finish. Once your iPad is at the Hello screen, click 'Patch'. Do not touch the iPad at all. Wait a while and your iPad should be bypassed and you can set it up like a normal iPad.

# Troubleshooting:

If you get an error while patching, redo all the steps, try another USB cable or USB port and try it with another PC if possible.

If your device keeps blinking in the sidebar and is just acting glitchy in general, open Terminal and put in this command `sudo killall -STOP -c usbd` and type in your account password. Note that your password will not appear, and it is normal.

If your device does not show up in the VM, try passing through the device twice.
