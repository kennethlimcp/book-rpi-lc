# Change password & assign static IP

1.) Enter the command: `passwd`

You should see:

```
Changing password for pi.
(current) UNIX password:
Enter new UNIX password:
Retype new UNIX password:
passwd: password updated successfully
```

<br><br>
2.) Next up, we will modify assign a **static IP** address.

Enter the command: `ifconfig`

We will need to note down the following:

INSERT Screenshot

- inet addr – 192.168.1.100 (current IP Address)
- Bcast –  192.168.1.255 (broadcast IP Range)
- Mask –  255.255.255.0 (subnet Mask Address)

<br><br>
3.) Now, we will grab the Gateway info with `netstat -nr`

Write down:

 - Gateway Address
 - Destination Address

Great! We can now modify the settings with:

`sudo nano /etc/network/interfaces
`

Change the following line:

`iface eth0 inet dhcp` to `iface eth0 inet static`

The mappings are as such:
```
`address` --> the_ip_you_prefer
`netmask` --> Mask
`network` --> Destination
broadcast --> Bcast
gateway ----> Gateway
```

What you will see after adding is like:


```
auto lo

iface lo inet loopback
iface eth0 inet static

address 192.168.1.200
netmask 255.255.255.0
network 192.168.1.0
broadcast 192.168.1.255
gateway 192.168.1.1

allow-hotplug wlan0
iface wlan0 inet manual
wpa-roam /etc/wpa_supplicant/wpa_supplicant.conf
iface default inet dhcp
sui
```

**Double-check** the parameters and save! <kbd>(CTRL+X)</kbd>


<br><br>
To make sure things are working ok, let's restart the machine with `sudo reboot`

If you managed to connect to the Rpi with the **new IP address**, congratulations!

Let's make sure things are indeed loading correctly:

`ifconfig`

To be super-sure things are ok, we will perform a ping to the gateway!

`ping gateway_ip_add -c 4`

<br>
<br>
*Licensed under: Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)*
