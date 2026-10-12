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

## Controls
Button 1: open the radial menu. Tilt in an action's general direction to select its full sector, then press Button 1 again to select it.
Button 2: show or hide the stats screen. It never changes the pet.
Shake: the only action that works naturally outside the menu.
The normal screen is a wandering 32 x 32, one-bit version of the supplied character. NAP freezes it in place with drifting zs, PLAY runs two fast left-to-right-to-left laps with hearts, PET sends hearts upward, and other actions do a tiny side-to-side shake followed by a jump. A shake wakes a sleeping pet early. Values only appear on the stats screen.

The final word in each menu line selects the visual reaction: NAP_REACTION, JUMP_REACTION, HEART_REACTION, or RUN_REACTION.
