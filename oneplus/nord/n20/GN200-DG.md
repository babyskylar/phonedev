this will only work if you have fastboot available to you. if all you have is EDL, then this method will not work.

to get rid of RW and get back into the stock stream, follow these steps.
NOTE: you must also do this if you wish to get out of RW.
WARNING: your slot must be slot A in order for the phone to boot properly
if you get reboots, or it goes into fastboot, check active slot, if slot B, switch to A.

file can be found [here](https://github.com/babyskylar/phonedev/releases/tag/N20_downgrade)

this works for all updates, but must be used from C.13 onwards.

to use:
P.1 flash OFP and boot
1. get phone into fastboot mode "adb reboot bootloader"
2. run "1runme" 
  2a. select option 2
  2b. select option 0
  2c. let it do it's thing errors and all.
3. using phones menu, reboot back into bootloader
4. get phone into fastbootd "fastboot reboot fastboot"
5. re-run "1runme"
  5a. select option 2
  5b. select option 0
  5c. let it do it's thing errors and all.
6. setup phone without accounts to make sure it boots properly

P.2 run "2downgrade-fix"
STEP 1 NOTES: this flashes all the files for A.05 so you can update to A.08 properly using stock methods.
STEP 2 NOTES: this step puts the device on slot A for A.08 so all other updates fall where thy need to properly.
