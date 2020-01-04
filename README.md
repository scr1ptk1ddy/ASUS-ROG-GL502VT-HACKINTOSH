**NOTE: THE FILES AND THE TUTORIAL ARE A MODIFIED FROM [CremBluRay's Original Guide](https://github.com/CremBluRay/ASUS-ROG-GL552VW-HACKINTOSH).**

# Asus ROG GL502VT Hackintosh MacOS Mojave 10.14.6 

### MAKE BOOTABLE MOJAVE USB GUIDE

**DOWNLOAD OR CLONE MY REPO BEFORE STARTING**

01. You need access to a macbook.
02. Go to the appstore and type 'mojave' now download the installer.
03. After the installer is downloaded go into Finder > Applications and verify that its there.
04. Plug a usb in your macbook and erase it as a "Mac OS Extended (Journaled)" partition and rename your usb to "USB"
05. Copy paste the `sudo /Applications/Install\ macOS\ Mojave.app/Contents/Resources/createinstallmedia --volume /Volumes/USB --applicationpath /Applications/Install\ macOS\ Mojave.app --nointeraction`
06. After the usb has been successfully completed go to the files u got from my repo and open "Clover_v2.5k_r5102.pkg"
07. Click "Continue" 2 times then click "Change Install Location" and select the "Install macOS Mojave" usb which is the usb you just created.
08. Click "Continue" then click "Customize" and check the "Clover for UEFI booting only" then click "Install".
09. After the clover installation finishes on your usb go to the files u got from my repo and replace your "BOOT" and "CLOVER" files in the usb on "EFI" partition with mine.
10. Now you are ready to install the macOS Mojave on your hackintosh machine.

### INSTALLATION OF MOJAVE

**CHANGE YOUR BOOT ORDER IN BIOS AND SELECT USB AS FIRST**

01. Boot into your usb which you created earlier.
02. You will see Clover with many options use your mouse to click on "BOOT OS X INSTALL FROM INSTALL macOS Mojave".
03. It will take some time to load so be patient after it loads click on "Disk Utility".
04. From the left panel select the disk drive on which you want to install the macOS on.
05. Format the disk drive as "APFS" then go back to the main options.
06. Click on "Install macOS" from the main menu and select your disk drive which you formatted earlier and then click "Install".
07. During the installation the system will reboot many times so be patient and don't freak out.
08. After the installtation has been done setup your system by following the onscreen prompts.

### POST INSTALLATION STEPS

01. At this point your hackintosh machine should be up and running.
02. Now go to the files u got from my repo and open "Clover_v2.5k_r5102.pkg".
03. Click "Continue" 2 times then click "Change Install Location" and select the disk drive on which you have installed your macOS Mojave.
04. Click "Continue" then click "Customize" and check the "Clover for UEFI booting only" then click "Install".
05. After the clover installation finishes on your disk drive go to the files u got from my repo and replace your "BOOT" and "CLOVER" files in the "EFI" partition with mine.
06. You don't need your usb anymore so unplug it and change your boot order to the drive on which you have your macOS Mojave installed.
07. When you turn on your computer you will see a clover screen again now select "BOOT macOS" and your machine should boot up into your hackintosh OS.

---

### WHAT WORKS :)

- Intel HD Graphics
- HDMI
- USB ports
- Keyboard
- Function Keys
- Ethernet
- Wifi (use ac1200 usb-ac53 nano)
- Battery Status
- UVC HD Webcam
- Speaker and Microphone
- Touchpad

### WHAT DOESN'T WORK :(

- NVIDIA Optimus
- SD Card Reader

---

### Thanks to:

- [CremBluRay](https://github.com/CremBluRay) for his ASUS-ROG-GL552VW-HACKINTOSH guide
- [fidele007](https://github.com/fidele007) for the original project and guide
- [RehabMan](https://www.tonymacx86.com/members/rehabman.429483/) for all the amazing guides and kexts
- [toleda](https://www.tonymacx86.com/members/toleda.2393/) for his [Broadcom WiFi/Bluetooth [Guide]](https://www.tonymacx86.com/threads/broadcom-wifi-bluetooth-guide.242423/)
- [u/corpnewt](https://www.reddit.com/user/corpnewt) for the [vanilla guide](https://hackintosh.gitbook.io/-r-hackintosh-vanilla-desktop-guide/) which walks you through the steps in making a Hackintosh happen for each CPU architecture
- [alexandred](https://github.com/alexandred) and other contributors to the project [VoodooI2C](https://github.com/alexandred/VoodooI2C) who made the support for ASUS's ELAN touchpad possible
- [acidanthera](https://github.com/acidanthera) for their work on [AppleALC](https://github.com/acidanthera/AppleALC) and [Lilu](https://github.com/acidanthera/Lilu)
- Everyone else on the tonymacx86 forums
