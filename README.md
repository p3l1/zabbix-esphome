# Zabbix Integration for ESPHome Devices

This project aims to integrate sensor data from [ESPHome](https://esphome.io/) Devices into [Zabbix](https://zabbix.com) via an MQTT-Broker.

## Structure

The project uses ESPHome, which provides a simple Webinterface to manage all sensors and ESP devices. The given nodes are then configured to use an MQTT for communication with Zabbix. The `docker-compose.yml` comes with a basic MQTT broker (mosquitto), but any other broker can also be used.

To get the published data from the MQTT broker the [Zabbix Agent2 MQTT plugin](https://git.zabbix.com/projects/ZBX/repos/zabbix/browse/src/go/plugins/mqtt?at=release/6.2) is used.

## Installation

The `docker-compose.yml` provides a basic setup including mosquitto and esphome.
