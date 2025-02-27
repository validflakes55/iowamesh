---
title: Meshtastic Node Configuration
tags:
  - Info
  - Getting Started
---

### Initial Setup
   - Power on your node.
   - Connect to a laptop via USB or phone via Bluetooth.
      - **Bluetooth:** Enable Bluetooth on your device (if not already enabled).
      - **Wi-Fi:** Use Wi-Fi if your node has a Wi-Fi chip.
      - **USB Serial:** Use Meshtastic Web Client `https://client.meshtastic.org/`

### Settings Configuration
   - Connect to your node.
   - Setup basic information:
     - Set your device name.
     - Choose the correct region (United States/915MHz).
     - Set other preferences such as GPS settings, screen brightness, etc.
     - View our [recommended settings](#other-recommended-settings).

#### Device Role is an important step for configuring Meshtastic.
- `Client` Recommened for most nodes. This is the default role.
- `Client_Mute` Ideal for additional nodes in close proximity (e.g., a single home or apartment) or areas with high mesh coverage. These nodes can send and recieve messages but do not participate in routing other nodes' messages. THey help reduce network congestion in dense areas.
!!! warning **`Router` or `Repeater` should only be used for devices that have an excellent line of sight to the surrounding area. (e.g., mounted to radio towers)**
- Other roles exist for nodes that serve a purpose other than messaging.
  -  For detailed information on all roles and their usage, refer to [Choosing The Right Device Role](https://meshtastic.org/blog/choosing-the-right-device-role/) and the [Meshtastic Documentation](https://meshtastic.org/docs/configuration/radio/device/#roles)

### Recommended Settings
- Broadcast Node Info Interval: `10800 seconds` (3 hours)
- GPS for Mobile Nodes: `Enabled`
- GPS for Fixed Nodes: `Fixed Location`
- Power Saving Mode:
    - Non-Solar Nodes: `Disabled`
    - Solar Nodes: `Enabled`
- Lora Region: `US`
- Hop Count: `7`
- Frequency Slot: `20`
- Waveform Settings: `LongFast`
- Radio Transmit: `Enabled`
- Max Transmit Power: `30dBm`
- Override Duty Cycle: `Enabled`
- Boosted RX Gain: `Enabled`
- Store and Forward:
    - Mobile Nodes: `Disabled`
    - Router and Fixed Nodes: `Enabled`
- Heartbeat: `Enabled`
- Number of Records: `100`
- History Return Max: `100`
- History Return Window: `7200 seconds` (2 hours)
- Update Interval: `900 seconds` (15 minutes)