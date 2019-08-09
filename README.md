# RPi_nodejs_npm_DHT11
Install Node.js, npm, and DHT11 driver on RPi

### Install nodejs

### Install npm

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

### References
[1] http://www.airspayce.com/mikem/bcm2835/index.html
