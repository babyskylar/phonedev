this applies to both devices (GN2200/CHP2459}

<br><b>NOTE:</b> disable verity files can be found [here](https://github.com/babyskylar/phonedev/releases/tag/verity). use the ones for your current build and device (if they are available).

follow these directions to a tee


<br><br>windows "adb_fastboot" folder:
<br>Any areas that have the quotation marks are the commands
1. put the verity images into root of folder with "adb.exe" and "fastboot.exe".
2. start command window and type command "adb devices" if it shows as device, you are good, otherwise allow it to be used, and driver is installed
3. "adb reboot bootloader"
4. "fastboot flash --disable-verity --disable-verification dtbo dtbo.img"
5. "fastboot flash --disable-verity --disable-verification vbmeta vbmeta.img"
6. "fastboot flash --disable-verity --disable-verification vbmeta_system vbmeta_system.img"
7. "fastboot flash --disable-verity --disable-verification vbmeta_vendor vbmeta_vendor.img"
8. "fastboot flash --disable-verity --disable-verification vendor_boot vendor_boot.img"
9. using phones volume keys make sure it says start and hit the power button. let phone boot.
10. get back into fastboot "adb reboot bootloader".
11. "fastboot flash --disable-verity --disable-verification dtbo dtbo-zeroed.img"
12. "fastboot flash --disable-verity --disable-verification vbmeta vbmeta-zeroed.img"
13. "fastboot flash --disable-verity --disable-verification vbmeta_system vbmeta_system-zeroed.img"
14. "fastboot flash --disable-verity --disable-verification vbmeta_vendor vbmeta_vendor-zeroed.img"
15. "fastboot flash --disable-verity --disable-verification vendor_boot vendor_boot-zeroed.img"
16. if it is included with the verity files, "fastboot flash boot boot-magisk-zeroed.img"
17. select recovery from the current menu and wipe the device.


N20AIO: **always choose the option for your device for best compatibility**
1. watch video for disable verity and follow the directions found in this video [here](https://youtu.be/sIJ_IcVUjts?si=i-uMwKIZ0Cxuif8P). if it hangs up on not flashing, close bat, install driver, and try again 
2. make sure it boots both times and then factory reset the device after second boot


if all you are wanting is verity disabled. then setup phone as normal,
if you would like to get RW, then setup phone without signing into anything, or internet. Also get usb debugging working. directions for RW can be found [here](https://github.com/babyskylar/phonedev/blob/main/oneplus/nord/n20/RW.md).
