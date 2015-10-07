#### Preparation

1) Toolchain

Follow [Toolchain](https://github.com/esp8266/esp8266-wiki/wiki/Toolchain) page

You should install, 
* Toolchain
* Espressif SDK
* Xtensa libraries and headers
* ESP image tool
* ESP upload tool

2) Test writing with Blinky example

`Build` and `Flashing` is documented in two pages

2-1) compile

Read [Building](https://github.com/esp8266/esp8266-wiki/wiki/Building)

```
cd /opt/Espressif
git clone https://github.com/esp8266/source-code-examples.git
cd source-code-examples/blinky
make
```

2-2) Flashing

Read [Uploading](https://github.com/esp8266/esp8266-wiki/wiki/Uploading)

* Power off ESP8266 board
* Connect GPIO0 to GND
* Connect GPIO2 to VCC
* Power on

Flash with `make`,
```
make ESPPORT=/dev/ttyUSB0 flash
```
After flashing is successfully finished, 
* Power off
* Disconnect GPIO0 so that it is floating
* Connect GPIO2 with serial of 470 Ohm + LED and to GND
* Power On

LED should blink on and off every second.

#### Working with ESP8266

Will be documented in Wiki pages...
