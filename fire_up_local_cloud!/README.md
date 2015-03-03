# Fire up Local Cloud!


1.) fire up the server, baby!

`node main.js` in the `spark-server` folder

This will have some lag for the first time when the Rpi creates a new key.

```
pi@raspberrypi ~/spark-server $ node main.js
-------
No users exist, you should create some users!
-------
connect.multipart() will be removed in connect 3.0
visit https://github.com/senchalabs/connect/wiki/Connect-3.0 for alternatives
connect.limit() will be removed in connect 3.0
Starting server, listening on 8080
static class init!
Loading server key from default_key.pem
set server key
server public key is:  -----BEGIN PUBLIC KEY-----
MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEA0Gv5evNQCYusK+TnLy2B
lt7WLkSMcjKDzf/JQIkA7azKpJ8iYo8/W2ZTVQYHGxzglvPThkAkwjINpEEKHmQg
199tUDFMo46+FpYFa4A4pOVgF765Uhr84eKSMqCkJ4vzcV7mmrDUTFcmq8ERAOee
802deTBRBRoA7vey1ZjOBrP5WBzTfRAsnmX/ysWBAEe+ikE/4dtIeNlGmp1Z12ne
S1BTomc7d2LJZisJjQ3IszOguvW7DpwovMWxXIJjUy6Uh02zHaEth6ljjUaAeTPU
FZyt6FxWKnNubv8fFM59Ma9eFxKHvIZxCoVabYrilvXNqmraG2rHmrvaqE4lM2eN
3QIDAQAB
-----END PUBLIC KEY-----

Your server IP address is: 192.168.1.200
server started { host: 'localhost', port: 5683 }
```

<br>
<br>
The next tutorial to help you connect Spark Cores to your local cloud can be found at:

https://community.spark.io/t/tutorial-local-cloud-1st-time-instructions/5589

<br><br>
Have fun!

k

<br>
<br>
*Licensed under: Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)*
