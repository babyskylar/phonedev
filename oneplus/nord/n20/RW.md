as with root, and the others, any images will go into the adb_fastboot folder. you will also need command open and directed to that folder
use the files that only pertain to you device. failure to do so will result in bricked device

1. "adb devices" if it shows as device, you are good, otherwise allow it to be used
2. "adb reboot fastboot"
3. "fastboot flash --disable-verity --disable-verification odm odm-rw.img"
4. "fastboot reboot booloader"
5. "fastboot flash super super-rw.img"
6. wipe the device using devices own recovery
7. reboot and setup as normal.
8. do gpay fix
