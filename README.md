# pi-bluetooth
Loads BCM43430A1 firmware on boot
Originally forked from https://github.com/RPi-DISTRO.
Bring nicer support of Raspberry 3B+ on-board bluetooth device for ubuntu
18.04-arm.

## Getting prepared
On ubuntu 16.04.5 LTS
```
$ sudo apt-get install build-essential
$ sudo apt-get install dh-systemd
```

## Build the package
```
$ mkdir deb-build-dir && cd deb-build-dir
$ git clone git@github.com:ascentai/pi-bluetooth.git && cd pi-bluetooth
$ dpkg-buildpackage -us -uc
$ cd ../ && ls -la | grep *.deb
```
