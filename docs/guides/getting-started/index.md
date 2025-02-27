---
title: Getting Started with Meshtastic
tags:
  - Info
  - Getting Started
---

# Getting Started with Meshtastic (915MHz, US)
Meshtastic is a mesh networking project that utilizes affordable, long-range, and low-power radio hardware to create ad-hoc mesh networks. This guide will help you set up a Meshtastic node and join the network.

## Hardware Requirements
- **[Meshtastic-compatible device](https://meshtastic.org/docs/hardware/devices/)**: Popular vendors include RAKWireless, Heltec, and SenseCap. There are several other ESP32 boards with LoRa radios that are compatible as well.
- **Antenna**: An antenna with 903MHz minimum and 928MHz maximum frequency range. Typically, best performance is achieved with a 3dBi gain. For detailed information on all antennas and their usage, refer to [Meshtastic antenna reports](https://github.com/meshtastic/antenna-reports).
- **USB-C PD 15V 20W**: Power adaptor and USB-C to USB-C cable.

!!! warning "Important Note"

    Never power on your Meshtastic device without an antenna connected. This could permanently damage the radio.

## Software Setup and Flashing the Firmware
1. Browse to [Meshtastic Web Flasher](https://flasher.meshtastic.org).
2. Follow the instructions to flash the latest firmware.

!!! tip "Next Steps"

    Check out our [Meshtastic Node Configuration Guide](https://iowamesh.org/guides/getting-started/configure).

## Legal Considerations
- Meshtastic operates in the 915MHz ISM band under FCC regulations in the United States.
- Meshtastic does not require a HAM radio license to operate.
- All communications on Meshtastic LoRa are encrypted by default.