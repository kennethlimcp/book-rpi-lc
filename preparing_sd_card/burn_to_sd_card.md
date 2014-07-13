# Burn to SD card

The Raspberry Pi website has great documentation to setup the SD card properly.

1. [Linux](http://www.raspberrypi.org/documentation/installation/installing-images/linux.md)
2. [Mac OSx](http://www.raspberrypi.org/documentation/installation/installing-images/mac.md)
3. [Windows](http://www.raspberrypi.org/documentation/installation/installing-images/windows.md)

<br><br>
**Tips for mac:**

To speed up the copying, we should use the raw disk drive instead. Some have gotten **10x improved performance** by doing the following:

*adding `r` to `/dev/disknumber` to become `/dev/rdisknumber` which will use it as a raw disk

The full command will look like:
```
New:
sudo dd bs=1m if=path_of_your_image.img of=/dev/rdisknumber

Old:

sudo dd bs=1m if=path_of_your_image.img of=/dev/disknumber

```

It was indeed faster (the previous took forever)

```
2825+0 records in
2825+0 records out
2962227200 bytes transferred in 257.177468 secs (11518222 bytes/sec)
```

<br>
<br>
*Licensed under: Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)*
