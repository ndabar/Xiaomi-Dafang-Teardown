## Xiaomi Dafang Teardown

This repository is a collection of Informations about the Dafang Camera

![Dafang](/dafang.png)

## Teardown

![Teardown](/teardown/mainboard_teardown.jpg)

Can be found in the "teardown"-folder

## Usage

[Getting Root-Access using Serial](/mod_getroot/getroot.md)

[Dumping-Firmware](/mod_getroot/firmware-dump.md)


## Contribution

Any contribution to the development is highly welcome. The best possibility to provide any change is to open a pull request on GitHub.


## Hardware infos 
Main Processor:
[Ingenic T20](ftp://ftp.ingenic.com/SOC/T20/T20_PB.PDF)

Wifi:
[Realtek 8192](http://www.realtek.com.tw/products/productsView.aspx?Langid=1&PFid=48&Level=5&Conn=4&ProdID=277)

LED Driver:
[ULN2803](http://www.ti.com/lit/ds/symlink/uln2803a.pdf)



The Hardware should be similar to [Icamera Keep](https://www.ismartalarm.com/devices/cameras/icamera-keep/ISA00008.html)

Source of this Information: [Source](https://xiaomi.eu/community/threads/cant-open-camera-plugin-xiaomi-mijia-dafang-home-1080p-hd.41855/#post-391171)

## Software Infos:

Opened Ports:
1. Port 80: Probably "Boa HTTPd 0.94.13" according to Nmap
2. Port 10002 : No Clue yet, but it responds with the following Sequence if you send a simple
"GET"-Request:

ICAM�������������ÿ����s���àÖÑv�����TÑv

The complete portscan can be found in portscan.txt

## Testpoints on Board:

![Headers](/teardown/headers_sample.jpg)

have a look at mod_serial folder for a example setup of the serial-console

## Hardware required for debugging:
FTDI-Adapter with 3.3V




## List of sources:
A Hack of a similar Device(Camera using the Ingenico T10):

[Part1](http://nm-projects.de/2016/12/hacking-digoo-bb-m2-mini-wifi-part-1-identify-the-serial-interface/)
[Part2](http://nm-projects.de/2017/01/hacking-ip-camera-digoo-bb-m2-part-2-analyzing-the-boot-process/)
[Part3](http://nm-projects.de/2017/01/hacking-ip-camera-digoo-bb-m2-part-3-getting-root-access/)

Linux on Ingenic Devices:

[Linus Mips](https://www.linux-mips.org/wiki/Ingenic)


