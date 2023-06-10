how to properly update the nord N20. 

1. boot into standard fastboot "adb reboot bootloader"
2. flash unrooted boot from current build "fastboot flash boot boot.img"
3. disable developer options. bootloader unlocked is fine. no need to get rid of magisk, or rooted apps
4. update device using standard method in settings. let it reboot
5. boot back into standard fastboot "adb reboot bootloader".
6. flash rooted boot for new build "fastboot flash boot boot-magisk.img"
7. reboot and enable developer options, and you are good.
