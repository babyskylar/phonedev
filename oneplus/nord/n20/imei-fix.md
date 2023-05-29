get the file for your version and phone [here](https://github.com/babyskylar/phonedev/releases/tag/modem)
and you must use the adb-fastboot contained in this zip located [here](https://github.com/babyskylar/phonedev/releases/tag/files-needed)
using any other adb or fastboot will not allow it to work.

<br><br><b>NOTE:</b> if this does not work for you, then you will unfortunately have to get a new device.


<br>get your phone into fastboot mode "adb fastboot reboot" or by holding the volume down button while rebooting
Now the key is to erase the partitions before flashing them. erase in any order you want, but when flashing, the way it is listed must be followed.
commands as follows:

<br>fastboot erase mdm1m9kefs1
<br>fastboot erase mdm1m9kefs2
<br>fastboot erase mdm1m9kefs3
<br>fastboot erase mdm1m9kefsc
<br>fastboot erase modem_a
<br>fastboot erase modem_b
<br>fastboot erase modemst1
<br>fastboot erase modemst2
<br>fastboot erase modemdump
<br>fastboot flash modem_a modem_a.img
<br>fastboot flash modem_b modem_b.img
<br>fastboot flash modemdump modemdump.img
<br>fastboot flash modemst1 modemst1.img
<br>fastboot flash modemst2 modemst2.img
<br>fastboot flash mdm1m9kefs1 mdm1m9kefs1.img
<br>fastboot flash mdm1m9kefs2 mdm1m9kefs2.img
<br>fastboot flash mdm1m9kefs3 mdm1m9kefs3.img
<br>fastboot flash mdm1m9kefsc mdm1m9kefsc.img
