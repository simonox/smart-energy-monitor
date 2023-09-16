# Hardware

We are using HelTec Automation Wirelsess Sticks ESP32 Dev-Boards.

## PinOut

The PinOut of our version 3 modules can be found here: https://docs.heltec.org/en/node/esp32/dev-board/hardware_update_log.html#wifi-lora-32-hardware-update-logs

![PinOut](../images/HTIT-WS_V3.png "PinOut")

## License

For some parts of the Heltec board you need a ["license"](https://docs.heltec.org/general/view_limited_technical_data.html#esp32-lora-series).

## USB-C

Our HelTec Automation Wirelsess Sticks ESP32 Dev-Boards already have USB-C. But they do not support Power Deliver (PD). If your computer tries to do PD, just plug a cheap USB hub between the board and your computer.

## Arduino IDE

HelTecs GitHub repo can be found here: https://github.com/HelTecAutomation/Heltec_ESP32

I had to install VCP Drivers, first: https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers?tab=downloads

You can add their Board Manager to the boards managers URLs: https://github.com/HelTecAutomation/Heltec_ESP32/blob/master/library.json and find their libraries in the IDE (Sketch -> Include Library -> Manage Libraries... Search for "heltec esp32").

> These boards are already _V3_ boards, so be careful selecting the right board and port (VCP).

![Arduino IDE](../images/flash-with-arduino.png "select the right board and port")

## Install esptool

Esptool is a Pyhton program to flash ESP32. As it's a Pyhton tool you can install it using `pip`:

```sh
pip install esptool
```

## Find the port

Usually you can find the used port using `esptool.py`:

```sh
esptool.py write_flash_status --non-volatile 0
```

### Using MicroPython

Download the firmware: https://micropython.org/download/

Flash it using `esptool`: https://micropython.org/download/GENERIC_S3/

```sh
esptool.py --chip esp32s3  write_flash -z 0  ~/Desktop/GENERIC_S3-20220117-v1.18.bin
```
