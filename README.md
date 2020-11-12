# wlan_renaming
re-naming wlan0 to the old school style 

sudo nano /etc/default/grub  

Look for `GRUB_CMDLINE_LINUX` and add the following `net.ifnames=0 biosdevname=0`  

Change From:

 `GRUB_CMDLINE_LINUX=""`  

To:  

 `GRUB_CMDLINE_LINUX="net.ifnames=0 biosdevname=0"`  
 
 the run `sudo update-grub2`
