# RMS Documentation

<br>
<br>
<br>


## Project Tree Structure

Where better place to start then a map? 🗺️

<br>

```
Remote-Monitoring-System/
│
│
│── Documentation/
│   │
│   │── README.md   ⬅   You're here 🚩
│   │
│   │── LICENSE (Apache 2.0)
│   │
│   │── Architecture.md 📐
│   │
│   │── Interfaces Definitions/ 📡
│   │   │
│   │   │── RMS-Bus/
│   │   │   │── Protocol.md
│   │   │   └── Transport.md
│   │   │
│   │   └── Ethernet/
│   │       └── TCP.md
│   │       └── PoE.md
│   │ 
│   │── Masters
│   │   │── Rack-Manager.md
│   │   └── Debug-Dongle.md
│   │
│   └── Devices
│       │── Temperature sensor.md
│       │── Fan Manager.md
│       └── Coming soon... 🚧
│
│
│
├── Masters/ 🖥️
│   │
│   ├── Rack-Manager/
│   │   └── Board/
│   │   └── Firmware/
│   │   └── Mechanical/
│   │
│   └── Debug-Dongle/
│       └── Board/
│       └── Firmware/
│       └── Mechanical/
│
│
│
└── Devices/
    │
    │── Temperature-Sensor/ 🌡️
    │   └── Board/
    │   └── Firmware/
    │   └── Mechanical/
    │
    ├── Fan-Manager/ 🌪️
    │   └── Board/
    │   └── Firmware/
    │   └── Mechanical/
    │
    └── Coming soon... 🚧
```

<br>
<br>
<br>

## What? Why?

### What?
> An open-source, out-of-the-box and plug-&-play system for rack cabinets monitoring.

<br>

### Why?
> The other open-source project are not as modular as we need it to be.
