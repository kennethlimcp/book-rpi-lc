# Misc Instructions

1.) Copy server public key to own machine

`scp pi@192.168.1.200:spark-server/default_key.pub.pem Desktop`

2.) Send core public key to server

`scp core_keys/55ff6e065075555329461687.pub.pem pi@192.168.1.200:spark-server/core_keys`
