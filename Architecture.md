<placeholder>

# RMS (Rack Monitoring System)

<br>
<br>
<br>
<br>
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
<br>
<br>
<br>
<br>

## 1. What? Why?

### What?
An open-source, out-of-the-box and plug-&-play system for rack cabinets monitoring.

<br>

### Why?
The other open-source project are not as modular as we need it to be.

<br>
<br>
<br>
<br>
<br>

## 2. Bus

### 2.1. Physic Layer

Total power: 10W<br>
Voltage: 24V<br>

<br>

Poles number: 2<br>
**Power over Bus**

<br>

RS-485 like

<br>

Single Master, Multi Slave (SMMS)

<br>

Number of slaves: 32
Maximum power per slave: 100mW (Typical) / 200mW (Max)

<br>


Connectors: ? **TBD**<br>
Modulation: ? **TBD**<br>


<br>
<br>

### 2.2. Protocol

- CRC
- Variable lenght
- Versioning
- Functional code (ModBus like)
- Addressing
- Request-Response / Polling
- Standard register set
    - Common Registers: UID, Version, Type, ...
    - Type specific registers
    - Auxiliary Registers (e.g. Vendor-Specific Registers)

<br>
<br>
<br>
<br>
<br>

## 3. Master / Dongle

- Power from PoE (Power over Ethernet) or wall adapter
- 

<br>
<br>
<br>
<br>
<br>

## 4. Slave device

- UID 32 bit, from factory or user-programmed
- Logic domain receive power from bus (for mitigating power domain issues)
- Other domains receive power externally
- 
