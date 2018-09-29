# How_to_openthread
How to get openthread running

Orginal Repro: https://github.com/TobiasReichert/How_to_openthread

Last edit: 23.04.2018

## cc2650
Can only be a child.

https://github.com/openthread/openthread/tree/master/examples/platforms/cc2650

Flash with Uniflash: 
http://www.ti.com/tool/UNIFLASH


## SAMR21
Can be a leader too.

https://github.com/openthread/openthread/tree/master/examples/platforms/samr21

Flash with:
https://github.com/openthread/openthread/tree/master/examples/platforms/samr21#flash-binaries

Port:
EDBG USB

COAP:
```bash
make -f examples/Makefile-samr21 clean
make -f examples/Makefile-samr21 COMMISSIONER=1 COAP=1 JOINER=1 DHCP6_CLIENT=1 DHCP6_SERVER=1
```
https://github.com/openthread/openthread/issues/2717

## Setup a Network
https://codelabs.developers.google.com/codelabs/openthread-simulation/#3

https://github.com/openthread/openthread/tree/master/examples/platforms/samr21#run-the-example-with-sam-r21-xplained-pro-boards

## RIOT
https://github.com/RIOT-OS/RIOT/tree/master/tests/openthread

fatal error: libudev.h: No such file or directory
```bash
sudo apt-get install libudev-dev
```
### SAMR21
~~Gets in Leader state but cc2650 with orginal openthread can't connect.~~
befor starting openthread you must change the channel to the same number
