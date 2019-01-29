# Realtek RTL8188EUS v5.3.9 (2018)

Driver support for rtl8188eu, rtl8188eus and rtl8188etv chipsets.<br>
Linux & Android 8 is supported and various boards/architectures.

[![Monitor mode](https://img.shields.io/badge/monitor%20mode-supported-green.svg)](#)
[![Frame Injection](https://img.shields.io/badge/frame%20injection-not%20supported-red.svg)](#)
[![GitHub version](https://badge.fury.io/gh/kimocoder%2Frtl8188eus.svg)](https://badge.fury.io/gh/kimocoder%2Frtl8188eus)
[![GitHub issues](https://img.shields.io/github/issues/kimocoder/rtl8188eus.svg)](https://github.com/kimocoder/rtl8188eus/issues)
[![GitHub forks](https://img.shields.io/github/forks/kimocoder/rtl8188eus.svg)](https://github.com/kimocoder/rtl8188eus/network)
[![GitHub stars](https://img.shields.io/github/stars/kimocoder/rtl8188eus.svg)](https://github.com/kimocoder/rtl8188eus/stargazers)
[![GitHub license](https://img.shields.io/github/license/kimocoder/rtl8188eus.svg)](https://github.com/kimocoder/rtl8188eus/blob/master/LICENSE)
<br>
[![Kali](https://img.shields.io/badge/Kali-supported-blue.svg)](https://www.kali.org)
[![aircrack-ng](https://img.shields.io/badge/aircrack--ng-supported-blue.svg)](https://github.com/aircrack-ng/aircrack-ng)
[![wifite2](https://img.shields.io/badge/wifite2-supported-blue.svg)](https://github.com/derv82/wifite2)

## This driver supports:
```
* Android 8 (checking Android 9 soon)
* MESH mode operation
* Monitor mode
```

## TODO
```
* Add more VHT capabilities (HT Greenfield will be added)
* Add frame injection (packet injection)
* Fix the USB3 quirk (and modeswitch).
* Add old/new kernel support (up to kernel v5.0)
* Add support for kernels with backported cfg80211 API
* Add the 8812/8814 & 8821 HAL (and make them all supported in 1 module)
* Move the 8192EU HAL onto this base (not sure of this one yet)
```
++++ lots to walkthrough over here..


We'll check the posiblities to move our rtl8812au driver onto this base.<br>
This looks like a clean, better Realtek base! More information coming.

## Android users
This driver supports Android 8 (and below), 
For more information on how-to get started, look inside the "Android" folder for help.


## NetworkManager options
Newer versions of NetworkManager has some options you might find usefull.<br>
Simply add these lines into the NetworkManager.conf

[device]
```
[device]
wifi.scan-rand-mac-address=no

[ifupdown]
managed=false

[connection]
wifi.powersave=2
```

## Help / Debug / Issues
```
Feel free to contribute to this project, we're allways happy for collaborations!
Got questions/suggestions or maybe you'd encountered issues/bugs, open a "issue" report.
```
<b>Check the "documents" folder for internal schematics</b><br>
<b>And in the "tools" folder there's a Realtek Android application for different tests/debug</b>

![https://github.com/kimocoder/rtl8812au/blob/v5.2.20/documents/Screenshot_20190129-002101-01.jpeg](https://github.com/kimocoder/rtl8812au/blob/v5.2.20/documents/Screenshot_20190129-002101-01.jpeg)
<br><br>
![https://github.com/kimocoder/rtl8812au/blob/v5.2.20/documents/Screenshot_20190129-025608-01.jpeg](https://github.com/kimocoder/rtl8812au/blob/v5.2.20/documents/Screenshot_20190129-025608-01.jpeg)

<br><br><br>
## best regards<br>
## Christian aka kimocoder
christian@aircrack-ng.org
