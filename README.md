# beagle-pack
![Photo of the hardware](beagle-pack.JPG)
## Configure BeagleBone

Updated image to Debian 10.3 using eMMC IoT Flasher from https://beagleboard.org/latest-images

Power up the BeagleBone Green Wireless while holding down the small button near the SD slot. You need to keep it pressed until the blue LEDs start flashing wildly.

### Set static IP address

Connect BBG via USB. Connect to `192.168.7.2`

```
$ connmanctl services
*AR Wired                ethernet_88c2556c93d9_cable
$ sudo connmanctl config ethernet_88c2556c93d9_cable --ipv4 manual 192.168.1.10 255.255.255.0 192.168.1.1
```
