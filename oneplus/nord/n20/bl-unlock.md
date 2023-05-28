This is for both GN2200 and for CPH2459 

i will have a note next to which device it applies

make sure you are on C.12 for the. you may have to update using wifi, but maake sure you enable oem unlocking before you get on your wifi network to update.

For the gn2200, do not allow them to stick the sim in. it will disable the oem unlock. you may get it back by doing a factoy data reset, but no guarentees. 
when you do the factory reset, keep sim and SD card out if the phone and just do a generic setup (no accounts).

make sure you have usb debugging enabled, and that oem unlock also on.

anything with  "" is the commands to run.

1. (both) download adb_fastboot.zip from [here](https://github.com/babyskylar/phonedev/tree/8af41ba02d6a3fd9281c83210cd055e22444c42e/oneplus/needed-files) and put in in a location that is easilly accessable (i.e. C:\adb_fastboot).
2.  (both) using the cord that is included with the phone, connect it to the computer and make sure driver is properly installed. If it isn't, use the included driver from the adb_fastboot.zip and manually install it.
3. (GN2200) "fastboot oem get_unlock_code"
4. (GN2200) submit the information [here](http://www.oneplus.com/unlock_token?_ga=2.234988545.1689870803.1684785181-943976437.1681291978) and aslo write an email similar to the attached image to support@oneplus.com. you should get your key in about 48 business hours directly to your email![support](https://github.com/babyskylar/phonedev/assets/66063174/243eaf3e-3d01-45bf-aa5c-aca220f169d0)

5. (GN2200) once you have your unlock token, copy it to the extracted adb_fastboot folder and rename it to unlock.bin
6. (GN2200) "fastboot flash cust-unlock unlock.bin"
7. (both) "fastboot flashing unlock"
8. (both) if done properly, it should pop up with a menu that says 'unlocking the bootloader.....' using volume keys select 'unlock the bootloader'.
9. hit the power key, let phone do it's thing.

now if you goal was to just unlock the bootloader, then setup the device as normal, but if you want root go [here](https://github.com/babyskylar/phonedev/releases/tag/GN2200_11_C.12-root)
