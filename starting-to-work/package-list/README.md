# Packages

To send an update package first you need create one, so...

Open the `local.conf` file and change the variable  


>`UPDATEHUB_PACKAGE_VERSION_SUFFIX = "-test-image-1"`

to

>`"-test-image-2"`.  

Save and close the file and run     

> `$ updatehub-image-minimal-raspberrypi3.uhupkg`  

and after     

>`$ updatehub-image-minimal-raspberrypi3.uhupush`.  

Then you go to the product screen into the **UpdateHub** and in some seconds you will see your package there.  

![creating a package](/../../.gitbook/assets/package1.png)  
