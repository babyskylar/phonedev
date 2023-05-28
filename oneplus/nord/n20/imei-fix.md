get the file for your version and phone [here](https://github.com/babyskylar/phonedev/releases/tag/modem)

1. put those files into the folder where your adb.exe and fastboot.exe happen to be.
2. get your phone into fastboot mode "adb fastboot reboot" or by holding the volume down button while rebooting
Now the key is to erase the partitions before flashing them. erase in any order you want, but when flashing, the way it is listed must be followed.
commands as follows:

3. fastboot erase mdm1m9kefs1
4. fastboot erase mdm1m9kefs2
5. fastboot erase mdm1m9kefs3
6. fastboot erase mdm1m9kefsc
7. fastboot erase modem_a
8. fastboot erase modem_b
9. fastboot erase modemst1
10. fastboot erase modemst2
11. fastboot erase modemdump
12. fastboot flash modem_a modem_a.img
13. fastboot flash modem_b modem_b.img
14. fastboot flash modemdump modemdump.img
15. fastboot flash modemst1 modemst1.img
16. fastboot flash modemst2 modemst2.img
17. fastboot flash mdm1m9kefs1 mdm1m9kefs1.img
18. fastboot flash mdm1m9kefs2 mdm1m9kefs2.img
19. fastboot flash mdm1m9kefs3 mdm1m9kefs3.img
20. fastboot flash mdm1m9kefsc mdm1m9kefsc.img
