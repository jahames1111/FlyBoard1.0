# ESP32‑S3 Drone Controller PCB

A custom flight‑controller board built around the ESP32‑S3, designed for lightweight drone applications. The board integrates motor outputs, sensor interfaces, long‑range HC‑12 communication, and a safe power‑path charging system.

## Features
- ESP32‑S3 module for control, communication, and real‑time processing  
- Four motor output headers for ESC control  
- Sensor footprints for IMU, barometer, and magnetometer  
- HC‑12 header for long‑range UART radio communication  
- USB‑C port for programming and power input  
- Reset and mode switches for firmware flashing  
- Expansion headers for UART, I²C, and GPIO  
- Clean power distribution with decoupling and filtering
<img width="3507" height="2480" alt="image" src="https://github.com/user-attachments/assets/64631544-7919-446f-a25c-b6464095a6e4" />

## Power System Upgrade
The original TP4056 charger was replaced with the BQ24075 power‑path IC.  
This change provides:
- Safe simultaneous load + charge operation  
- Stable system voltage during USB/battery transitions  
- Improved thermal performance  
- Proper SYS/BAT power‑path routing for the ESP32

## Repository Contents
- Full KiCad project files (`.kicad_pro`, `.kicad_sch`, `.kicad_pcb`)  
- Gerber and drill files for fabrication  
- 3D renders and board previews  
- Documentation and design notes  

## Manufacturing
The `/gerbers/` folder contains a complete ZIP ready for JLCPCB or Hack Club Blueprint submission.

## License
MIT License – free to modify, build, and improve.

