Raspberry Pi Tales of Interest
==============================

Monday, November 17, 2016
-------------------------

Got the PiCan 2 working. The newer version of the Debian Jessie kernel required
a few changes to the boot time options.

```
# /boot/config.txt

dtparam=spi=on 
dtoverlay=mcp2515-can0,oscillator=16000000,interrupt=25 
dtoverlay=spi-bcm2835-overlay
```

Resources:

[General information](http://skpang.co.uk/catalog/pican2-canbus-board-for-raspberry-pi-23-p-1475.html)  
[Setup information](http://skpang.co.uk/catalog/images/raspberrypi/pi_2/PICAN2_jessie_2016-05-10.pdf)
