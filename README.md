```
#include <std_disclaimer.h>
/*
* Your warranty is void.
*
* I am not responsible for bricked devices, dead SD cards,
* thermonuclear war, or you getting fired because the alarm app failed. Please
* do some research if you have any concerns about features included in this Recovery
* before flashing it! YOU are choosing to make these modifications, and if
* you point the finger at me for messing up your device, I will laugh at you.
*/
```

If you didn't understand that:  

THIS IS NOT FOR DAILY USE. DO NOT COMPLAIN ABOUT BUGS OR BROKEN FEATURES, OR ANY FAILURES.  

Keep in mind:  

 • This build is not for use. It is a development build, for experimental purposes.  
 
 • Only use the provided images.  
 
# How to flash:  

 • Make sure your device's bootloader is unlocked.  
 
 • Power off the device and boot to download mode (Plug in USB cable and then hold both volume buttons until the blue download screen shows up)  
 
 • Download the recovery.tar for the phone (releases page)  
 
 • Download Samsung Odin and run it (If the device is not recognized, make sure Samsung USB Drivers are properly installed)  
 
 • Put the recovery.tar file in Odin's AP slot and flash it  
 
 • At the exact moment the screen goes off, boot to recovery mode with the key combo (Vol Up +  Power)  
 
 • Download the rootfs and boot image from the releases page and unzip the rootfs.
 
 • Enter fastboot mode  
 
 • Run the following:  
 
 • fastboot erase boot  
 
 • fastboot erase userdata  
 
 • fastboot flash boot /path/to/bootimage.img  
 
  eg: fastboot flash boot /home/schoosh/releases-mainline/4GB-boot-uniLoader-20260929-postmarketOS-a135f.img  
  
 • fastboot flash userdata /path/to/rootfs.img 
 
  eg: fastboot flash userdata /home/schoosh/releases-mainline/postmarketOS-plasma-mobile-6-20260929-rootfs-a135f.img  
  
 • Wait for it to finish flashing, then reboot to system. You will end up at the lockscreen.  
 
 The password for the lockscreen is 1234.
