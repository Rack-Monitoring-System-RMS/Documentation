<placeholder>

# RMS (Rack Monitoring System)

<br>

## Index

1. What? Why?<br>

2. Bus<br>
    2.1. Protocol<br>
    2.2. Physical implementation<br>
3. Master Device / Dongle<br>
    3.1. Master<br>
    3.2. Dongle<br>
4. Slave device

<br>

## 1. What? Why?

### What?
An open-source, out-of-the-box and plug-&-play system for rack cabinets monitoring.

<br>

### Why?
The other open-source project are not as modular as we need it to be.

<br>

## 2. Bus

### 2.1. Physic Layer

Total power: 60W (if USB-PD connected) or 12W (if only PoE present)<br>
Voltage: 12V<br>

<br>

Poles number: 4<br>
- 2 poles for Power
- 2 poles for Data (RS-485)

<br>

Single Master, Multi Slave (**SMMS**)

Master know where power is coming from and can decide which slave can be powered and which not.

<br>

Number of slaves: **TBD** (probably **256**)<br>

Types of slaves:
- Powered by only by the Master
    - Always powered: few milliWatt sensor
    - Power check needed: tens of Watt actuator (power budget must be checked by the master) <br>
- Powered by External Power Source (Fallback to Master power if external power fail)

<br>

Connectors: Pluggable screw terminal block
Modulation: None (DC)

<br>

### 2.2. Protocol

- ModBus RTU
- Device type pattern (e.g.: coil 0x69 identify sensors)
- Physical set of the slave address (address factory set, reconfigurable via software)
    - ! Suggest user to change default address !

<br>

## 3. Master / Dongle

- Power from PoE (Power over Ethernet) or wall adapter (i.e.: USB-PD)
    - PoE max 12W
    - USB-PD max 60W
- No external service needed
- Configure & Go

<br>

## 4. Slave device

- Configurable address (via software)
- Power itself with a external power source or with the bus if the other is not present
