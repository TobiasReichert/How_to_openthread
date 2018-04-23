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

## Setup a Network
https://codelabs.developers.google.com/codelabs/openthread-simulation/#3

https://github.com/openthread/openthread/tree/master/examples/platforms/samr21#run-the-example-with-sam-r21-xplained-pro-boards

## RIOT
https://github.com/RIOT-OS/RIOT/tree/master/tests/openthread

### SAMR21
Gets in Leader state but cc2650 with orginal openthread can't connect.
