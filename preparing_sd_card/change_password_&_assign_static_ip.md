# Change password & assign static IP

Enter the command: `passwd`

You should see:

```
Changing password for pi.
(current) UNIX password:
Enter new UNIX password:
Retype new UNIX password:
passwd: password updated successfully
```

Next up, we will modify assign a static IP address.

Enter the command: `ifconfig`

We will need to note down the following:

INSERT Screenshot

- inet addr – 192.168.1.100 (current IP Address)
- Bcast –  192.168.1.255 (broadcast IP Range)
- Mask –  255.255.255.0 (subnet Mask Address)

Now, we will grab the Gateway info with `netstat -nr`

Write down:

 - Gateway Address
 - Destination Address

Great! We can now modify the settings with:

`sudo nano /etc/network/interfaces
`

Change the following line:

`iface eth0 inet dhcp` to `iface eth0 inet static`

Below the line, we will add in the information manually:

```
address the_ip_you_prefer
netmask 255.255.255.0
network 192.168.1.0
broadcast 192.168.1.255
gateway 192.168.1.254
```

**Double-check** the parameters and save! <kbd>(CTRL+X)</kbd>

<br>
<br>
To make sure things are working ok, let's restart the machine with `sudo reboot`

If you managed to connect to the Rpi with the **new IP address**, congratulations!

Let's make sure things are indeed loading correctly:

`ifconfig`

To be super-sure things are ok, we will perform a ping to the gateway!

`ping gateway_ip_add -c 4`

