# RPi_nodejs_npm_DHT11
Install Node.js, npm, and DHT11 driver on RPi

### Update
```
sudo apt-get update
sudo apt-get dist-upgrade
```
### Install nodejs [optional]
```
curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
sudo apt-get install -y nodejs
node -v
```

### Install npm
```
sudo apt-get install npm
sudo npm install -g npm
sudo npm install -g npm
sudo npm install -g npm
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
### REBOOT

```
node-red-start
```
Open a browser and visit 127.0.0.1:1880. Click the "triple bars" button on the top right corner. Select "Manage palette". Select the "Install" Tag. Use DHT as keyword, select "node-red-contrib-dht-sensor" and click the install button.

### References
[1] http://www.airspayce.com/mikem/bcm2835/index.html 
