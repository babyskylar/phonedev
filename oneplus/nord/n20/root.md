this applies to both devices (GN2200/CHP2459}

<br><b>NOTE:</b> rooted and non-rooted boot files can be found [here](https://github.com/babyskylar/phonedev/releases/tag/boot)
<br><b>NOTE:</b> if all you intend is to root, then setup device as normal, with sim installed. if you intend to disable verity, then only setup device with no accounts, no sim, no internet.
<br><br>windows "adb_fastboot" folder:
1. put both images into root of folder with "adb.exe" and "fastboot.exe".
2. start command window and type command "adb devices" if it shows as device, you are good, otherwise allow it to be used
3. "adb reboot bootloader"
4. "fastboot flash boot boot-magisk.img"
5. download and install magisk canary from [here}(https://github.com/babyskylar/phonedev/releases/download/files-needed/magisk-canary.apk).
6. go into magisk and let it update and reboot the phone.
7. enable zygisk
8. reboot and prosper


<br><br>N20AIO:
**always choose the option for your device for best compatibility**
1. watch video for root and follow the directions found in this video [here](https://youtu.be/qKDdd8h7R_o?si=YVLzJwFzTbYlW38S)
2. download and install magisk canary from [here}(https://github.com/babyskylar/phonedev/releases/download/files-needed/magisk-canary.apk).
3. go into magisk and let it update and reboot the phone.
4. enable zygisk
5. reboot and prosper

<br><br>**if you intend on disabling verity, please follow disable verity instructions found [here](https://github.com/babyskylar/phonedev/blob/main/oneplus/nord/n20/verity.md)**
