You will need drivers, for most of the modes for our devices (adb, fastboot) can be found [here](https://github.com/babyskylar/phonedev/releases/download/files-needed/Universal_Naked_Driver_0.73.7z.001).  not needed if linux/mac.
<br>The drivers for EDL mode can be found [here](https://github.com/babyskylar/phonedev/releases/download/files-needed/Qualcomm.drivers.7z). not needed if linux/mac.
<br>A slimmed down adb/fastboot that is specific to our devices can be found [here](https://github.com/babyskylar/phonedev/releases/download/files-needed/adb_fastboot.zip). not needed if linux/mac.
<br>My N20 AIO file can be found [here](https://github.com/babyskylar/phonedev/releases/download/files-needed/N20AIOGH.7z.001). my AIO can be used to get and do most everything as long as you follow the directions. made with windows and bash in mind
<br>**NOTE: Use original red cord and backup all your data to another oneplus phone or to PC using a program like wondershare mobilego. all data must be unencrypted**
<br><br>directions for setup of device/computer
<br>1a. For GN2200 setup device without sim. if they(tmobile/metro) put one in, then remove it and leave it removed until instructed to do so. Factory reset device and set it up without accounts.
<br>1b. For both go into "settings", "about phone", "version", and repeatedly click on "build number" until it says you are a developer.
<br>2. Back out until you are at the settings main page and the go into "additional settings", then select "developer mode"
<br>3. Click on "OEM unlock" and a menu should pop up. hit enable on it.
<br>4. While still in "developer options", scroll down until you see "usb debugging". Enable it.
<br>5. Reboot device
<br>6. Extract out either the adb-fastboot or the N20AIO zip to it's own folder.
<br>7. Extract the "naked drivers" to just the inside of either the N20AIO or the adb_fastboot folder and have it sit in it's own folder inside there.
<br>8. Once device is rebooted and you are in the main screen, plug the device into you computer using the original red cord the device came with.
<br>9. An option on the phone will pop up, choose "transfer files/android auto".
<br>10a. For windows, if you see the device in "my computer, you are good (if not, install driver from the "naked drivers" folder make sure to select the "ADB" as the option.
<br>10b. For linux/mac just install the ADB/fastboot for your respective OS. the phone should automatically recognize the device without fiddling with drivers/kexts.
<br>11a. if using the AIO, there is a windows and bash folder respectively. bash folder is for linux/mac, and the windows folder is for windows.
<br>11b. On windows go to either "N20AIO/windows", or the root of "adb_fastboot" where you will see "fastboot.exe", and "adb.exe".
<br>12a. On windows -with the device unlocked and the screen on- in the folder start a command propnt window and type in it "adb devices" without the quotation marks. you should see an option on the device to allow usb debugging. check the check box and click "enable".
<br>**note: if command does not work, install driver manually. if windows complains about driver signature and won't install it, disable driver signature permanently using your OS's specific guide**
<br>12b. For Linux/Mac start a terminal window, type "adb devices" without the quotation marks. If it says something about root/sudo try "sudo adb devices" without the quotation marks.
