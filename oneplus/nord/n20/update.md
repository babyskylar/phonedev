how to properly update the nord N20. keep the images for your curent build in their apropriate folders until you have sucsessfully updated. then overwrite them with the new build.

Windows adb_fastboot folder:
<br>**make sure all images are in the root of the folder with adb.exe**
1. update phone using stock methods
2. get into bootloader and root new build using the new build boot files found [here](https://github.com/babyskylar/phonedev/releases/tag/boot) the command is "fastboot flash boot boot-magisk.img"

if your phone errors out during update install
<br>1. get into bootloader and unroot using the boot for your curent build included in my boot files zip. "fastboot flash boot boot.img"
<br>2. update phone as normal
<br>3. get into bootloader and root new build using the new build boot files found [here](https://github.com/babyskylar/phonedev/releases/tag/boot) the command is "fastboot flash boot boot-magisk.img"
<br><br>N20AIO:
<br>**always choose the option for your device for best compatibility**
1. update as normal
2. put boot inages for the new build into the "images" folder
3. start aio
4. choose your device
5. choose root.

if your phone errors out during update install
1. start AIO
2. choose device
3. select back to stock
4. choose stock rooted
5. let the AIO finish and leave program open
6. unplug phone from pc and update using the standard methods
7. download and overwrite the boot files in the "images" folder with ones for the new build.
8. plug phone back in and make sure it is in file transfer mode.
9. choose root. let it finish.
10. once it has sucefully flashed, exit out and enjoy.
