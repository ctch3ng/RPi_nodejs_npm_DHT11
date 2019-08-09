# RPi_nodejs_npm_DHT11
Install Node.js, npm, and DHT11 driver on RPi

### Update
```
sudo apt-get update
sudo apt-get dist-upgrade
```
### Install nodejs
```
curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
sudo apt-get install -y nodejs
node -v
```

### Install npm
```
sudo apt-get install npm
```

### Install DHT11 driver[1]
```
wget http://www.airspayce.com/mikem/bcm2835/bcm2835-1.60.tar.gz
tar zxvf bcm2835-1.60.tar.gz
cd bcm2835-1.60
./configure
make
sudo make check
sudo make install
```
### Install the node-dht-sensor dependency[2]
```
sudo npm install --unsafe-perm -g node-dht-sensor
```
### Install node-red-contrib-dht-sensor node[2]
```
sudo npm install --unsafe-perm -g node-red-contrib-dht-sensor
```

### References
[1] http://www.airspayce.com/mikem/bcm2835/index.html
[2] https://flows.nodered.org/node/node-red-contrib-dht-sensor
