# Install Node.js & npm

Original reference from: https://learn.adafruit.com/raspberry-pi-hosting-node-red/setting-up-node-dot-js

1.) Download the package made compatible for Pi with:

`sudo wget http://node-arm.herokuapp.com/node_latest_armhf.deb`

2.) Install the debian package:

`sudo dpkg -i node_latest_armhf.deb`

3.) Check the node.js version for a success install!

```
pi@raspberrypi ~ $ node -v

v0.10.29
```

4.) the package manager for Node.js will also be required.

So: `sudo apt-get install npm

```
pi@raspberrypi ~ $ sudo apt-get install npm
Reading package lists... Done
Building dependency tree
Reading state information... Done
```

<br>
<br>
*Licensed under: Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)*
