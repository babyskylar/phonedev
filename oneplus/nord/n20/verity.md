To disable verity for the your device, you need to follow a few steps to do that

WARNING: your userdata will be wiped during this process. Also make sure your phone is updated to C.12 for the GN2200 and C.13 for the CHP2459, rooted using magisk-canary, your bootloader is unlocked, and that usb debugging is enabled.

I would highly suggest backing up your data in a way that is unencrypted so it can go back on the phone without issue. i would also recommend unhiding any pics you have until you are back with verity-disabled, or you could wait until you have RW to hide them.

After your data is backed up using unencrypted methods, remove your SIM and SD card from the phone and set to the side (this is to ensure you don't lose your data on there).

you will need the adb_fastboot.zip from the "files-needed.7z" which can be found in my releases area (beware, you will need a password from me) downloaded and extracted out to a location of your choosing (i.e. C:/adb_fastboot) with the images listed here in that same folder.

Any areas that have the quotation marks are the commands

Also of note. use the files that pertain to your device , or you will brick it

with the device connected to PC, run command line in the adb_fastboot folder (does not need to be administrator).
type "adb devices" if it shows as device., your good, otherwise authorize it.
  <br><br>"adb reboot bootloader" wait for device to reboot
<br>"fastboot devices" if you see fastboot, you are good. If not install driver included with adb_fastboot.zip manually
<br>"fastboot reboot fastboot" this gets you into fastbootd. wait for device to reboot
<br>"fastboot getvar is-userspace" if it says yes, continue, if not, try the previous command, or check drivers.
<br>"fastboot getvar current-slot" if it is a, flash to a, if it is b, flash to b
the * from this point on will stand for either a or b depending on the current slot command
<br><br>"fastboot flash --disable-verity --disable-verification dtbo dtbo.img"
<br>"fastboot flash --disable-verity --disable-verification vbmeta vbmeta.img"
<br>"fastboot flash --disable-verity --disable-verification vbmeta_system vbmeta_system.img"
<br>"fastboot flash --disable-verity --disable-verification vbmeta_vendor vbmeta_vendor.img"
<br>"fastboot flash --disable-verity --disable-verification vendor_boot vendor_boot.img"
<br><br>setup phone without internet and accounts
<br><br>"fastboot flash --disable-verity --disable-verification dtbo dtbo-zeroed.img"
<br>"fastboot flash --disable-verity --disable-verification vbmeta vbmeta-zeroed.img"
<br>"fastboot flash --disable-verity --disable-verification vbmeta_system vbmeta_system-zeroed.img"
<br>"fastboot flash --disable-verity --disable-verification vbmeta_vendor vbmeta_vendor-zeroed.img"
<br>"fastboot flash --disable-verity --disable-verification vendor_boot vendor_boot-zeroed.img"
<br><br>the next 2 commands are dealers choice
<br><br>if you want root
<br>"fastboot flash boot boot-magisk-zeroed.img"
<br>just verity disabled and no root
<br>"fastboot flash boot boot-zeroed.img"
<br><br>using the menu in the phone, go to recovery, wipe all data(factory reset).

if all you are wanting is verity disabled. then setup phone as normal,
if you would like to get RW, then setup phone without signing into anything.then download the files for RW
