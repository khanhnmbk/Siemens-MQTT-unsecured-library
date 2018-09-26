# Siemens-MQTT-unsecured-library
This is the offical MQTT library for PLC S7-1500, S7-1200 published by Siemens

## Getting Started
MQTT is a light-weight protocol for M2M communication. This library enable Siemens'PLCs 
(S7-1200, S7-1500) to connect to unsecured MQTT broker.

## Requirement
- PLC S7-1200 with firmware 4.0 or above, PLC S7-1500 (any firmware)
- Available MQTT broker (for test purpose, [Mosquitto](test.mosquitto.org) is a good choice)
- Internet connection (cable)

## Deployment
In TIA Portal, add this library as a global library. Copy all blocks to Program blocks
(of your PLC). Call the Publisher_FB in a cyclic OB (such as OB1). Edit the generated DB
with your own broker information.

## Note
This is only a publisher client. For subscriber function, consult this library: 
