# Initializing the Yocto


After create an access key the next step is initialize the Yocto Project. So go to the folder where you want to store your project and run this:

`$: git clone https://git.yoctoproject.org/git/poky -b zeus`

Start the poky build environment.

`$: source poky/oe-init-build-env build`

Fetch the bitbake layers with the same version of poky zeus.

`$: bitbake-layers layerindex-fetch meta-updatehub-raspberrypi -b zeus`
