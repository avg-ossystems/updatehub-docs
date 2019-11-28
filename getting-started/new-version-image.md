# New Version Image

Now open the `local.conf` file and change the   

Before:   

`UPDATEHUB_PACKAGE_VERSION_SUFFIX = "-test-image-1.0"`   

New:   

`UPDATEHUB_PACKAGE_VERSION_SUFFIX = "-test-image-2.0"`     

Save the `local.conf` file and go to your build directory and type:  

`$: bitbake updatehub-image-minimal -c uhuarchive`   

And now send it to the ???????     type:    

`$: bitbake updatehub-image-minimal -c uhupush`   

> If you want a detailed explanation about this topic go to the [INTEGRATION section](../integration/pushing-and-update-package.md).
