# Generating an Image

After you configure the `local.conf` follow the next steps.

Open a terminal and go to your build directory and type:  

`$: bitbake updatehub-image-minimal`

Now it's time to record the image in the SD card. Then in a terminal go to this directory:   

 `build/tmp/deploy/images/raspberrypi2/`   

 and type this:    
> Pay attention!!! Check the name of the SD card device before executing the command below!   

 `$: zcat updatehub-image-minimal-raspberrypi3.wic.gz | sudo dd of=/dev/sdX`


 With the SD card ready, you can already insert it into the target and connect it to RaspberryPi. The image is with the network configured to obtain an IP address using DHCP. To access the console the user is set to “root” and does not need to enter a password.

 You can confirm the version of the image that is running on the target with the command `cat /etc/os-release` and you will see the version that you put in the `local.conf` file.

>`UPDATEHUB_PACKAGE_VERSION_SUFFIX = "-test-image-1.0"`  

![image instaled](../../.gitbook/assets/raspberry-zeus2.png)
