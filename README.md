#  DIY Wind Turbine Project: Smart Archimedes Turbine (IoT)

## About the Project
This project documents the scratch-build of a horizontal axis wind turbine (HAWT), using a rotor design based on the Archimedes screw. The goal is to create a small-scale renewable energy source, partially manufactured through 3D printing, capable of charging a 12V battery and equipped with smart remote monitoring (IoT) directly on a smartphone.

## Progress So Far
I have completed the mechanical design (CAD) phase for the main assembly:
* **The Rotor:** Helicoidal design (Archimedes screw). This geometry allows for efficient wind capture even at low wind speeds, providing high torque and very quiet operation.
* **Nacelle and Chassis:** Aerodynamically designed to minimize turbulence, including the mount for the generator and the main shaft.
* **Yaw System:** The base is equipped with a free-rotation system (yaw) to allow the turbine to constantly align with the wind direction.

### 3D Renders (Current Design)
<p align="center">
  <img src="https://github.com/razvancioc/DIY-Wind-Turbine-Project-Smart-Archimedes-Turbine-IoT-/blob/main/MEDIA/Lcorner.png" width="800" />
</p>
<p align="center">
  <img src="https://github.com/razvancioc/DIY-Wind-Turbine-Project-Smart-Archimedes-Turbine-IoT-/blob/main/MEDIA/Rcorner.png"  width="800" />
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/6eb6785e-4bef-4326-b2a8-eec25f9a681f" alt="Electrical Schematic" width="800" />
</p>

## Selected Hardware and Electronics
* **Generator:** [To be defined: e.g., DC 775 Motor or salvaged Nema 17 Stepper Motor]
* **Microcontroller & IoT:** ESP32 NodeMCU (for Wi-Fi connectivity)
* **Sensors:** INA219 (Voltage, Current, and Power measurement), RPM Sensor (Hall/Optical)
* **Energy Conversion:** Schottky Diode + XL6009 Buck-Boost Module for voltage stabilization at 14.4V
* **Safety System:** Relay module + Power resistor (Dump Load) for automatic braking in extreme wind conditions.

## Next Steps
1. **Manufacturing:** Slicing the 3D model to fit the Bambu Lab A1 build plate and printing the components using outdoor-resistant filament (PETG / ASA).
2. **Mechanical Assembly:** Mounting the main shaft using an M5 threaded rod, integrating the bearings, and securing the generator inside the nacelle.
3. **Electronics Wiring:** Building the rectification circuit, and connecting the charging module and sensors to the ESP32.
4. **Smart Telemetry (Software):** Programming the ESP32 and configuring a mobile dashboard (e.g., via Blynk IoT) to monitor live RPM and generated energy.
