## Physical & Electrical
BUS: **RS485**<br>
Poles number: **4 -> RS485_A RS485_B VCC GND**<br>
Voltage: **12V to 15V with tollerance of +-10%**<br>
Max devices: **128**<br>

## Protocol 
The protocol is implemented over Modbus RTU. <br>

### Inherited properties:
Single Master, Multi Slave (SMMS) <br>
Request response <br>

### Device type at ReadHoldingRegister 0xTBD, 0xTBD, 0xTBD:
These three 16 bits variables are fixed (address and value) inside the devices and if a master finds it recognise the device as standard of this protocol.

### Device type at ReadHoldingRegister 0xTBD:
This 16 bits variable defines the protocol version.

### Device type at ReadHoldingRegister 0xTBD (Multiple type per device):
This 16 bits variable is an index that should identify the type of the device connected to the bus.
The standard of indexes that this protocol aim to define, map a predefined data structure of addresses inside of the device.

#### Device type Temp 0xTBD
Has value of temp in °C in the 0xTBD register