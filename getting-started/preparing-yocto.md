# Preparing the Yocto environment

After create the access key, the next step is initialize the environment to
build a Linux image using **Yocto Project**. So go to the directory that you
want to work run:

`$: git clone https://git.yoctoproject.org/git/poky -b zeus`

Start the `poky` build environment.

`$: source poky/oe-init-build-env build`

The easiest way to fetch all layer that is needed to build an image for
`Raspberry Pi` with `UpdateHub` support use [bitbake-layers](https://www.yoctoproject.org/docs/current/dev-manual/dev-manual.html#adding-a-layer-using-the-bitbake-layers-script)
command like shown bellow.

`$: bitbake-layers layerindex-fetch meta-updatehub-raspberrypi -b zeus`
