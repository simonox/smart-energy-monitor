# Smart Energy Monitoring

Smart Energy Monitoring is an open-source hardware project designed to empower individuals to monitor their energy consumption easily and efficiently. With the versatility of two different integrations - a DIY kit and a finished product - users can make informed decisions to manage and reduce their energy footprint.

The project seamlessly integrates with the [IoT Prototyping Backend](https://code.curious.bio/curious.bio/iot-backend/) and serves as an exemplary application for the comprehensive integration of sensor systems, through the manipulation of data streams and visualization on a dashboard.

## Features

- Real-time energy monitoring
- Historical data logging
- MQTT Support
- Open-Source firmware

## Integrations

### DIY Kit

The DIY Kit includes an [ESP microcontroller](https://www.espressif.com/en/products/socs) and comes with appropriate measurement terminals. The firmware is open-source, based on the [Arduino framework](https://www.arduino.cc/reference/), allowing enthusiasts to extend or customize features according to their needs.

#### Hardware Requirements

- [Bill of Material](./hardware/BOM.md)
- Soldering iron

### Shelly Plus Plug S

For users looking for a ready-made solution, we support the [Shelly Plus Plug S](https://kb.shelly.cloud/knowledge-base/shelly-plus-plug-s) / [Shelly Plug](https://kb.shelly.cloud/knowledge-base/shelly-plug) or any other ESP based Power Plug with measurement functions. We use the device with the open-source firmware [Tasmota](https://tasmota.github.io/), making integration into your existing smart home systems a breeze. The following page gives an overview of the [devices supported by Tasmota](https://templates.blakadder.com/plug.html).

## Safety Note

> ⚠️ Handling High Voltage
> Working with electrical systems can be dangerous if not handled carefully.

Always make sure to:

- Turn off the power supply before making any electrical connections.
- Use insulated tools.
- Work in a dry environment.
- If you are not confident or experienced in working with electricity, please contact a professional to assist you.

## Installation

- [DIY Kit Installation](./docs/energy-monitor/README.md)
- [Shelly Plus Plug S](./docs/shelly-monitor/README.md)

## Contribution

Feel free to open an issue for bugs, feature requests, or questions. Contributions are welcome.

## License

This project follows the [REUSE Specification](https://reuse.software/spec/) and is licensed under the following:

- [Documentation: Creative Commons Attribution-ShareAlike 4.0 Licence](./LICENSES/CC-BY-SA-4.0.txt)
- [Hardware: CERN Open Hardware strongly reciprocal Licence](./LICENSES/CERN-OHL-S-2.0.txt)
- [Software: The GNU General Public License v3.0 Licence](./LICENSES/GPL-3.0-or-later.txt)
