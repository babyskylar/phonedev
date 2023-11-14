This is for both GN2200 and for CPH2459 

**note: BACKUP your data. And it is highly recommended to use my AIO script for windows and mac**

Here is the methods for bot windows and mac

i will have a note next to which device it applies
<br>note: both=CPH2459/GN2200


Windows adb_fastboot folder:
1. (both) open folder and start a command window inside of it.
2. (both) if phone is pluged in from following the steps from setup, then skip step 3 and 4.
3. (both) plug in device using original red cord
4. (both) in the command window type "adb devices" without the quotation marks. if it says device, continue on. Otherwise enable it using the steps found [here](https://github.com/babyskylar/phonedev/blob/main/oneplus/nord/n20/setup.md)
5. (both) type in "adb reboot bootloader" without the quotation marks. let phone reboot.
6a. (GN2200) "fastboot oem get_unlock_code". if command doesn't pull the unlock token or other data, install driver as bootloader device for phone and try command again.
6b. (GN2200) submit the information [here](http://www.oneplus.com/unlock_token?_ga=2.234988545.1689870803.1684785181-943976437.1681291978) and aslo write an email similar to the attached image to support@oneplus.com. you should get your key in about 48 business hours directly to your email![support](https://github.com/babyskylar/phonedev/assets/66063174/243eaf3e-3d01-45bf-aa5c-aca220f169d0). if they don't send it, call their tech support and give them the case number they sent to you.
6c. (GN2200) once you have your unlock token, copy it to the extracted adb_fastboot folder and rename it to unlock.bin.
6d. (GN2200) "fastboot flash cust-unlock unlock.bin" without the quotation marks.
7. (both) "fastboot flashing unlock"
8. (both) if done properly, it should pop up with a menu that says 'unlocking the bootloader.....' using volume keys select 'unlock the bootloader'.
9. (both) hit the power key, let phone do it's thing.


<br><br>N20AIO:
**always choose the option for your device for best compatibility**
1. (GN2200)watch video for unlock token and follow the directions found in this video [here](https://youtu.be/o-ochdop1Gg?si=DR8rIS-ZdKMiwO2X).
<br>1a. (GN2200) submit the information [here](http://www.oneplus.com/unlock_token?_ga=2.234988545.1689870803.1684785181-943976437.1681291978) and aslo write an email similar to the attached image to support@oneplus.com. you should get your key in about 48 business hours directly to your email![support](https://github.com/babyskylar/phonedev/assets/66063174/243eaf3e-3d01-45bf-aa5c-aca220f169d0). if they don't send it, call their tech support and give them the case number they sent to you.
2. (both)follow the directions found in the video found [here](https://youtu.be/vUz-rS50Ho4?si=GyFSNmLIQd5IE0mj).
3. (both) if done properly, it should pop up with a menu that says 'unlocking the bootloader.....' using volume keys select 'unlock the bootloader'.
4. (both) hit the power key, let phone do it's thing.
<br><br>**If all you wish is to unlock bootloader and not root, then setup device as normal. if you intend on rooting, please follow rooting instructions found [here](https://github.com/babyskylar/phonedev/blob/main/oneplus/nord/n20/root.md)**
<br><br>**Note:**if you want to lock the bootloader use the command "fastboot flashing lock". just beware, your phone has to be bone stock in order for it to boot properly.
