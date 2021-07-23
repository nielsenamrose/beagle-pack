# beagle-pack

## Configure BeagleBone

Updated image to Debian 10.3 using eMMC IoT Flasher from https://beagleboard.org/latest-images

Power up the BeagleBone Green Wireless while holding down the small button near the SD slot. You need to keep it pressed until the blue LEDs start flashing wildly.

Set static IP address
```
$ sudo connmanctl config ethernet_689e19a7b79c_cable --ipv4 manual 192.168.1.10 255.255.255.0 192.168.1.1
```
