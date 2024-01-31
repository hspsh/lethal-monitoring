# Getting started

git gud.

The image from google drive doesn't work correctly - no SSH, busybox is ancient, videostream is borked too

# Chaotic list of stuff todo

## spawn ubuntu docker for SDK compilation
docker run -it -v $(pwd):/app ubuntu

TODO: push docker image with preinstalled stuff

## upgrade stuff
Use flasher from: 

`luckfox-pico-sdk/tools/linux/Linux_Upgrade_Tool`

NEVER run this crap with sudo - just apply the udev rules, it will work sudoless.

## connect

adb shell works

to connect through usb networking, set static IP on host PC
`sudo ip address add 172.32.0.90/24 dev enp0s20f0u2`

now you can ssh via `ssh root@172.32.0.93` # passwd: luckfox

## view camera

VLC doesn't work reliably.

`mpv rtsp://192.168.0.146/live/1`

or

`mpv rtsp://172.32.0.93/live/0`

The camera lags as hell.

## NN research

https://github.com/rockchip-linux/rknn-toolkit2

## USB host

Need soldering iron. Saving progress here.

## Links

https://wiki.luckfox.com/Luckfox-Pico/Luckfox-Pico-USB
https://forums.luckfox.com/viewforum.php?f=13&start=25
https://wiki.luckfox.com/Luckfox-Pico/Luckfox-Pico-SDK
https://github.com/rockchip-linux/rknn-toolkit2