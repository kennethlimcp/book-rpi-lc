# Install Local Cloud Repo

With the basic setup ready, we are now ready to install Spark-server!

<br>
1.) run `cd` just to be sure we are in the base directory. Otherwise, you can choose where you want to `git clone` the repo.

<br>
2.) Download the `spark-server` repo:

`git clone https://github.com/spark/spark-server.git`


<br>
```
pi@raspberrypi ~ $ git clone https://github.com/spark/spark-server.git
Cloning into 'spark-server'...
remote: Reusing existing pack: 272, done.
remote: Total 272 (delta 0), reused 0 (delta 0)
Receiving objects: 100% (272/272), 61.07 KiB | 80 KiB/s, done.
Resolving deltas: 100% (155/155), done.
```
<br>
3.) go to the `spark-server/js` folder

`cd spark-server/js`

<br>
4) Install the module!

    `npm install --verbose`

You usually won't need `--verbose` but things are a little slow on the Rpi and it would be nice to see what's going on.


**ALERT:**

The `URSA` node module is not installing correctly with the `install.js` script from `spark-server`.

I am not sure why but it managed to build from source when i tried to find out the issue.

So we have to manually build it instead by:

```
cd node_modules
git clone https://github.com/Medium/ursa.git
cd ursa
npm install -verbose
```
<br>
Another issue came up with the `express` module so...

```
cd
cd spark-server/js
npm install express -verbose`
```


<br><br>
WOOHOO! We now have a shiny new server which talks **COAP protocol** and responses to `API calls`!!


<br><br><br><br>
Commands summary list:

```
git clone git@github.com:spark/spark-server.git
cd spark-server/js
npm install
node main.js
```

<br>
<br>
*Licensed under: Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)*
