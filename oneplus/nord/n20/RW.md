this applies to both devices (GN2200/CHP2459}

<br><b>NOTE:</b> RW files can be found [here](https://github.com/babyskylar/phonedev/releases/tag/RW). use the ones for your current build and device (if they are available).

To see RW in action, please watch this video linked [here](https://youtu.be/fNp9pZUJXmE?si=rS0YNHv42p6V_iWb).

i noticed with trying to use the magisk modules to enable RW was not allowing me to delete or edit files properly. this is the reason i created the RW

as with root, and the others, any images will go into the root of the "adb_fastboot" or "images" folder. you will also need command open and directed to that folder
use the files that only pertain to you device. failure to do so will result in bricked device

to see if your phone is compatible with the RW, it needs to be on a certain slot for it to work, which is listed below
<br>CPH2459_11_C.13 slot B
<br>CPH2459_11_C.14 slot A
<br>CPH2459_11_C.15 slot B
<br>CPH2459_11_C.16 slot A
<br><br>GN2200_11_C.12 slot B
<br>GN2200_11_C.13 slot A
<br>GN2200_11_C.14 slot B
<br>GN2200_11_C.15 slot A
<br>GN2200_11_C.16 slot B

windows "adb_fastboot" folder: 
1. "adb devices" if it shows as device, you are good, otherwise allow it to be used
2. "adb reboot fastboot"
3. "fastboot flash --disable-verity --disable-verification vendor_boot vendor_boot-zeroed-rw.img"
4. "fastboot flash super super-rw.img"
5. wipe the device using devices own recovery
6. reboot and setup as normal.
7. download and install magisk canary from [here](https://github.com/babyskylar/phonedev/releases/download/files-needed/magisk-canary.apk).
8. go into magisk and let it update and reboot the phone.
9. enable zygisk
10. reboot and prosper

<br><br>N20AIO:
**always choose the option for your device for best compatibility**
1. watch video for RW and follow the directions found in this video [here](https://youtu.be/Sa7nrsNlccw?si=i4CY9vmhQulLKu1w)
2. wipe the device using devices own recovery
3. reboot and setup as normal.
4. download and install magisk canary from [here](https://github.com/babyskylar/phonedev/releases/download/files-needed/magisk-canary.apk).
5. go into magisk and let it update and reboot the phone.
6. enable zygisk
7. reboot and prosper
