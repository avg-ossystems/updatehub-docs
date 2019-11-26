# Step-3

---> talvez aqui seja interessante colocar um passo antes deste explicando como usar minicom.

Now we have to enable the network in order to have internet access to connect the device to  **UpdateHub**.
Then run the command:  

`$ ifconfig` (Using ifconfig includes setting an IP Address and netmask on an interface, and enabling and disabling a given interface).

For example if in your case the network interface is `eth0` then you would type:

`$ ifup eth0`

If by chance ifconfig doesn't work and you need to enable `DHCP` then run the command below:

`$ dhcpc` (this should work and enable your network for internet access)
