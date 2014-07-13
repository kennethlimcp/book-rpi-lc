# Update Packages

1.) Run `sudo apt-get update` to ensure we have all the latest packages

```
pi@raspberrypi ~ $ sudo apt-get update
Get:1 http://raspberrypi.collabora.com wheezy Release.gpg [836 B]
Hit http://repository.wolfram.com stable Release.gpg
Get:2 http://archive.raspberrypi.org wheezy Release.gpg [490 B]
Hit http://repository.wolfram.com stable Release
```
<br>
2.) Next will be upgrading with `sudo apt-get upgrade`

```
pi@raspberrypi ~ $ sudo apt-get upgrade
Reading package lists... Done
Building dependency tree
Reading state information... Done
The following packages will be upgraded:
  dbus dbus-x11 gnupg gpgv libdbus-1-3 libsmbclient libwbclient0 libxml2
  rpi-update samba-common smbclient
11 upgraded, 0 newly installed, 0 to remove and 0 not upgraded.
Need to get 9673 kB of archives.
After this operation, 42.0 kB of additional disk space will be used.
Do you want to continue [Y/n]? y
```

<br>
<br>
*Licensed under: Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)*
