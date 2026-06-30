# Universal-Curing-Chamber
PCB to modify any mini fridge or wine cooler into a fully functional environmental chamber for use as a humidor, curing meats &amp; cheeses, or any other thing you need to cure or store.

🚀 Current Status: Version 1 (V1)
The files currently in this repository represent the V1 Prototype. This version is a proven, 2-layer PCB design currently running in active test environments.

V1 Key Features:
Dual-Sensor Logic: Integrated support for multiple SHT31-D temperature and humidity sensors.

Active Cooling: Dedicated PWM control for Peltier modules and circulation fans.

DeHumidification: One peltier is able to be dedicated to dehumidification. It is also able to be tapped by the main cooling peltier if needed for cooling.

Safety array of 4 Thermistors (1 attached to each heatsink) with software safety logic if the heatsinks get too hot.

Wi-Fi Connectivity: Fully enabled for remote monitoring and web-dashboard integration.

🛠 Under Development: Version 2
We are currently finalizing Version 2, a complete architectural overhaul designed for true univeral applicability.

Planned V2 Upgrades:
4-Layer Power Stackup: A dedicated internal power plane and ground shield designed to handle a 12V 30A primary supply.

On board ultrasonic mister circuit and relay for compressor fridges. The mister circuit and relay can be bypassed by the user to enable simple pwm control.

Integrated buck converters AP63203 (3.3V) & AP63205 (5V).

High-Mass Thermal Management: Layer 1 copper heatsink pours stitched via thermal vias to internal planes, ensuring components stay cool under heavy DC loads.

Expandability: all available pins on the esp32 are mapped with easy access to power and ground pins.

Upgraded to the ESP32-S3-WROOM-1-N16R.

Optimized BoM

MCU: ESP32-S3 (Dual-core, Wi-Fi/BLE)

Gate Drivers: Dual TC4427CPA high-speed drivers (1.5A peak drive)

High-Power Switching: 4x AOD4184 MOSFETs (40V 60A rated)

Peripheral Switching: 4x AO3400A MOSFETs for fans and auxiliary gear

📖 Open Source Integrity
To maintain true open-source transparency, this project provides:
Accurate Schematics: Precise part numbers and values are maintained even for common components to ensure easy replication.

Optimized BoM: Verified LCSC/Aliexpress part numbers to help builders achieve professional results at a hobbyist price point

🤝 Contributing
Version 2 is currently in the routing phase. If you have experience with high-current PCB layout or ESP32-S3 firmware optimization, feel free to open an issue or reach out.
