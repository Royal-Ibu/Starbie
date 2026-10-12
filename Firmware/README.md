# Starbie Firmware

Firmware source code, sketches, drivers, libraries, and related project code is uploaded here.

Examples:
- Arduino or C/C++ source files
- platformio or make files
- firmware binaries
- MCU configuration files

## Arduino IDE setup
To set-up the firmware, go to Arduino IDE, open File → Preferences and add this to Additional Boards Manager URLs:

https://espressif.github.io/arduino-esp32/package_esp32_index.json
Open Tools → Board → Boards Manager, search for esp32, and install esp32 by Espressif Systems.

Select Tools → Board → esp32 → XIAO_ESP32C3 and select the board's port under Tools → Port.

Open Sketch → Include Library → Manage Libraries and install:

Adafruit GFX Library
Adafruit SSD1306
Adafruit MPU6050
DHT sensor library
If Arduino asks to install dependencies, choose Install All.

Open Starbie_Kakashi.ino, press the arrow-shaped Upload button, and wait for the upload to finish.

Seeed's XIAO ESP32-C3 setup guide also confirms selecting XIAO_ESP32C3 from the ESP32 Arduino board list.
