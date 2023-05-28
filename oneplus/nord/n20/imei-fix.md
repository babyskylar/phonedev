get the file for your version and phone [here](https://github.com/babyskylar/phonedev/releases/tag/modem)

1. put those files into the folder where your adb.exe and fastboot.exe happen to be.
2. get your phone into fastboot mode "adb fastboot reboot" or by holding the volume down button while rebooting
Now the key is to erase the partitions before flashing them. erase in any order you want, but when flashing, the way it is listed must be followed.
commands as follows:

fastboot erase mdm1m9kefs1
fastboot erase mdm1m9kefs2
fastboot erase mdm1m9kefs3
fastboot erase mdm1m9kefsc
fastboot erase modem_a
fastboot erase modem_b
fastboot erase modemst1
fastboot erase modemst2
fastboot erase modemdump
fastboot flash modem_a
fastboot flash modem_b
fastboot flash modemdump
fastboot flash modemst1
fastboot flash modemst2
fastboot flash mdm1m9kefs1
fastboot flash mdm1m9kefs2
fastboot flash mdm1m9kefs3
fastboot flash mdm1m9kefsc
