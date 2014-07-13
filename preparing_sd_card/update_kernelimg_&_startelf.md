# Update kernel.img & start.elf

The `.img` file from the **raspbian** image does not contain the latest files and upgrading this files before powering up will save us some updating time later.

Go to:

1. Download the latest Rpi firmware from:
https://github.com/raspberrypi/firmware/blob/master/boot/start.elf


2. Download the latest Rpi kernel from: https://github.com/raspberrypi/firmware/tree/master/boot/kernel.img

Overwrite the files on the SD and eject the card!
