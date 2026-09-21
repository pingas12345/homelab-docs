# Home Automation

Home automation stack centered on Home Assistant, with Zigbee support and MQTT messaging.

## Core Components

- **Home Assistant** - Central home automation platform
- **Zigbee2MQTT** - Zigbee device integration
- **Mosquitto** - MQTT broker
- **SLZB-06M** - Zigbee coordinator (Ethernet/PoE capable)

## Design Notes

- Zigbee coordinator is network-attached for flexible placement
- MQTT is used as the messaging layer between Zigbee2MQTT and Home Assistant
- All components run as Docker containers where possible

## Skills Demonstrated

- Integration of multiple home automation components
- Zigbee network management
- MQTT-based service communication
- Containerized deployment of automation workloads
