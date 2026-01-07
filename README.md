## DIY Portable Windows Tablet Using LattePanda ##
- Project Overview:
This project demonstrates the design and construction of a portable Windows-based tablet (Pocket PC) using a LattePanda single-board computer, a 7-inch IPS display with capacitive touch, and a battery-powered system with proper power management.

The project focuses on hardware integration, power electronics, and system-level design, without using any custom PCB. All components are interconnected using jumper wires and ready-made modules, making the system modular, safe, and easy to troubleshoot.

-  Objectives:

- To build a compact, portable Windows computer
- To understand battery management and voltage regulation
- To interface HDMI display and USB capacitive touch
- To demonstrate a real-world embedded computing system
- To avoid PCB fabrication by using modular hardware

 ## wiring config ##
 | Connection                   | Description             |
| ---------------------------- | ----------------------- |
| Battery → BMS                | 3S series configuration |
| BMS → Buck Converter         | 12V output              |
| Buck Converter → LattePanda  | Regulated 5V supply     |
| Buck Converter → Display     | Regulated 5V supply     |
| LattePanda HDMI → Display    | Video signal            |
| LattePanda USB → Touch Panel | Touch input             |

## Power Management & Safety ##

A 3S BMS ensures:

- Over-charge protection
- Over-discharge protection
- Short-circuit protection
- Cell balancing
- Buck converter prevents over-voltage damage to LattePanda
- All grounds are common
- No battery is connected directly to the system without regulation

## Build Procedure ##

- Assemble 3 × 18650 cells in series and connect to BMS
- Connect BMS output to buck converter input
- Adjust buck converter output to 5.1V
- Power LattePanda and display from buck converter
- Connect HDMI cable between LattePanda and display
- Connect USB cable from touch panel to LattePanda
- Power ON the system and verify functionality

## project overview ##
This project successfully demonstrates the construction of a DIY portable Windows tablet using a LattePanda SBC. It highlights the importance of safe power management, modular hardware design, and system integration, making it an excellent real-world learning project.

## 3D case ##
I buit a custom made case for the tab:

