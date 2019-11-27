# Configuring the local.conf file


After fetch the bitbake layers is important change some variables in the local.conf file

Look for the variable    

>`MACHINE ??= "qemux86-64"`       

and change to    

>`MACHINE ?= 'raspberrypi3'`

It's necessary to add the variables below:

Contains the IP address where updatehub-ce is running:
>`UPDATEHUB_SERVER_URL = "https://api.updatehub.io"`   

Used to add a suffix in the version of the image being generated and at this time you should put in a version number:
>`UPDATEHUB_PACKAGE_VERSION_SUFFIX = "-test-image-1.0"`   

The RSA key bellow you can generate [here](../integration/generating-a-rsa-key.md)
>`UPDATEHUB_UHUPKG_PRIVATE_KEY = "/home/username/updatehub-keys/private_key.pem"`
>`UPDATEHUB_UHUPKG_PUBLIC_KEY = "/home/username/updatehub-keys/public_key.pem"`   

The two variables below you learn how to create in the [DASHBOARD section](../dashboard/access-key.md)
>`UPDATEHUB_ACCESS_ID = "your-email@gmail.com-8bc21121049af..."`    
>`UPDATEHUB_ACCESS_SECRET = "9b1fcee96795fa5dea5cd04cb1d2..."`   

And finally you need inform the `local.conf` file the product UID that you can see [here](../integration/create-a-product.md)
>`UPDATEHUB_PRODUCT_UID = "db1b4f82911468d800569d33d55d5162557..."`   
