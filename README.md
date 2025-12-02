# DIY Battery Spot Welder

![Project Banner](Images/DIY%20Spot%20Welder.png)
![Build Status](https://img.shields.io/badge/build-passing-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)

A professional-grade DIY battery spot welder for assembling custom battery packs. Features precise pulse control, high-current MOSFET switching, and safe operation for lithium battery assembly.

## ⚡ Features

- **Precise Pulse Control**: NE555 timer-based 10ms welding pulse
- **High Current Capacity**: Parallel IRLB4132 MOSFETs (6x configuration)
- **Safe Operation**: Two-hand trigger system & isolated probes
- **Easy Assembly**: Through-hole components for DIY-friendly construction
- **Professional PCB**: Manufacturable via JLCPCB or similar services

## 📸 Project Images

| Schematic | PCB Design | Final Build |
|-----------|------------|-------------|
| [Schematic](https://github.com/BEEMB/DIY-Battery-Spot-Welder/blob/main/Images/Circuit%20Schematic.png) | [PCB](https://github.com/BEEMB/DIY-Battery-Spot-Welder/blob/main/Images/PCB%203D%20Render.png) | [Build](https://github.com/BEEMB/DIY-Battery-Spot-Welder/blob/main/Images/Final%20Assembly%20view.JPG) |

## 📋 Bill of Materials (BOM)

| Component | Quantity | Specification | Notes |
|-----------|----------|---------------|-------|
| NE555 Timer | 1 | DIP-8 package | Pulse generator |
| IRLB4132 MOSFET | 6 | TO-220 package | Parallel configuration |
| 10kΩ Resistor | 2 | 1/4W | Timing circuit |
| 100nF Capacitor | 1 | Ceramic | Timing capacitor |
| 100μF Capacitor | 1 | Electrolytic, 25V | Power stabilization |
| LED | 1 | 5mm, any color | Pulse indicator |
| 220Ω Resistor | 1 | 1/4W | LED current limit |
| Push Button | 1 | Momentary switch | Trigger |
| Terminal Blocks | 3 | 2-pin, 5mm | Probes & power input |
| PCB | 1 | 2oz copper recommended | |

## 🛠️ Assembly Instructions

### 1. PCB Preparation
- Order PCB from [JLCPCB](https://jlcpcb.com/?from=TIP) using Gerber files in `/Fab Files/`
- Select 2oz copper thickness for better current handling
- Black solder mask recommended (all colors same price)

### 2. Component Soldering
1. Start with small components (resistors, capacitors, IC socket)
2. Solder terminal blocks
3. Install MOSFETs with thermal consideration
4. Add probe connectors last

### 3. Probe Construction
- Use 4mm copper rods for welding tips
- Solder thick AWG cables (8-10 gauge recommended)
- Insulate with heat shrink tubing
- Mount push button on negative probe handle

### 4. Power Connection
- Connect 12V battery (7Ah minimum, higher recommended)
- Ensure polarity is correct
- Add fuse for additional safety

## ⚙️ Technical Specifications

| Parameter | Value | Notes |
|-----------|-------|-------|
| Input Voltage | 12V DC | Can be modified for LiPo |
| Pulse Width | 10ms | Adjustable via RC components |
| Max Current | ~500A | Depends on battery source |
| PCB Size | 80mm x 60mm | Standard JLCPCB size |
| Copper Weight | 2oz | Recommended for high current |
| Probe Tip Diameter | 4mm | Copper recommended |

## 👤 Author
**Chris**
- YouTube: [@DIYGUYCHRIS](https://www.youtube.com/channel/UC_GCvo_dC3joZjL0TlD8xZA)
- GitHub: [@DIYGUYCHRIS](https://github.com/BEEMB)

## 🙏 Acknowledgments
- **Analog Devices** for the excellent LT3652 IC and documentation
- [**JLCPCB**](https://jlcpcb.com/?from=TIP) for reliable PCB fabrication services
- [**Altium**](https://www.altium.com/yt/diyguychris) for providing professional PCB design tools
- **Open Source Community** for continuous inspiration and support

### ⭐ If you find this project helpful, please give it a star on GitHub!
