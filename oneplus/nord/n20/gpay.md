wait until your device has transfered all its data from the backup you made earlier.
do not access any apps that you want to put on the deny list.

1. put the MagiskHideProps found [here](https://github.com/Magisk-Modules-Repo/MagiskHidePropsConf), safetynet-fix found [here](https://github.com/kdrag0n/safetynet-fix), and Shamiko found [here](https://github.com/LSPosed/LSPosed.github.io/releases) on the root of the internal storage
2. install via magisk
3. go to the gear icon, and put gpay, authenticators, healthcare, and banking apps on the deny list.
3a. also enable force deny
4. reboot phone.
open a command window in adb_fastboot folder
5. "adb devices" if it shows as device, you are good, otherwise allow it to be used
6. "adb shell" allows access to the device via command line on the PC
7. "su" make sure you say yes to magisk, if it doesn't work, go to magisk and enable root for sh.
<br>7a. if you see "#" in the command prompt, continue on
8. "props"
9. "1"
10. "f"
11. "21"
12. make your selection. i chose "21"
13. when OS choice pop up, select the one that is closest to the N20s current build version
22. "Y" twice.
23. phone will reboot, if you can add a virtual card from your banking app to gpay, then you are all set.
