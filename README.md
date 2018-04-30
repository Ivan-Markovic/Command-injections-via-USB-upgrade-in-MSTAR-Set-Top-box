# Command-injections-via-USB-upgrade-in-MSTAR-Set-Top-box

While I was working on diagnostic device for some of my clients I found command injections in MSTAR Set-Top box products. Diagnostic device is not specially target this vendor but we used it in development phase and for testing. Vulnerable functionality is in automatic USB upgrade process. It is possible to inject additional commands via malicious files names. 

For example, to upgrade your Set-Top box, you just need to put firmware file on USB drive with filename "auto_upgrade.bin" and after you insert it and restart device, it will be automaticaly upgraded. This fuctionality can be also exploited by inserting additional commands in filename.

Full advisory: https://security-net.biz/set-top-box-command-injection-mstar-uboot-usb-upgrade.html
