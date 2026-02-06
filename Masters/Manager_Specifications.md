# Master specifications

## RMS-Bus

### Interfaces

The master has 2 RMS-Bus (TODO Add link here) interfaces.

### Total power capabilities:
Power budget divided by two interfaces

#### Powered over USB-C
>This path has priority over PoE

Total power: **60W**<br>
Voltage: **15V**<br>
Current: **4A**<br>


#### Powered over PoE

Total power: **12W**<br>
Voltage: **12V**<br>
Current: **1A**<br>
Type: **TBD**<br>
Type: **Class**<br>

## Electrical protections

## Features 

## Configuration
The device should be configured once and work standalone and has the capability to expose the data requested when you want (Sensor value, alarms flags)

The device should be configured with the principle of the following logic:

Aggregate sensors with some operator (mean, max, min, sum, average)
Map the aggregated data inside a user-defined map
Actuate multiple device with the result

## Mechanical
Can be mounted Standalone or Rack monted