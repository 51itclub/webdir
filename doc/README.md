## wadir.php 

### USAGE

#### Aria2

Debian


install Aria2 


```
apt-get install -y aria2
```

install screen

```
apt-get install -y screen
```

Aria2 config

```
mkdir /root/.aria2


wget http://webdir.cc/aria2.config /root/.aria2/aria2.config


wget http://webdir.cc/dht.dat /root/.aria2/dht.dat


echo '' > /root/aria2.session 

```

start up Aria2 

```
screen -dmS aria2 aria2c --enable-rpc --rpc-listen-all=true --rpc-allow-origin-all -c 
```

#### wadir.php

upload *wadir.php* on your WWW directory

set passworfd
```
define("PASS","Password");
```
set forbidden access directory [notdir] and extension [notex]
```
$this->notdir=array("a","phpmyadmin");
$this->notex=array("php","js","tgz");
```

visit http://yourdomain/wadir.php by your browser




