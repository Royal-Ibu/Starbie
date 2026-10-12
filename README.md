# ⭐ Starbie

A custom printed circuit board designed in KiCad as part of [Hack Club's Half Life](https://halflife.hackclub.com/) hardware program. Starbie is a tiny motion-controlled digital pet: basically a desktop Tamagotchi with minimal gameplay buttons. Instead of pressing controls, you interact with it by physically moving the board.

## Take a look

<img width="852" height="675" alt="Starbie Top" src="https://github.com/user-attachments/assets/d973a894-85eb-42e6-a5d3-fb24a9738f0e" />


## What it is
Starbie is designed to sit on your desk, show its personality on a small display, and react to how you handle it. Tilting, moving, and otherwise checking in on your pet are meant to be part of the experience.

The board includes a microcontroller, display, motion sensor, and environmental sensor in a compact PCB design. It is USB powered and built around beginner-friendly through-hole soldering for the add-on components.

## Project status
The PCB design, renders, and an Arduino starter firmware are included here. The default program is a two-eye pet with a tilt-controlled radial menu, hidden stats, and a shake reaction.

## Software
Firmware/ contains one self-contained Arduino IDE sketch for the XIAO ESP32-C3. Builders customize pins, menu actions, starting values, and motion settings together at the top of the sketch. The folder also includes a draggable browser simulator.

## Project files


| File or folder | What it contains |
| --- | --- |
| `Starbie.kicad_pro` | Main KiCad project file |
| `Starbie.kicad_sch` | Circuit schematic |
| `Starbie.kicad_pcb` | PCB layout |
| `.png` | PCB renders, screenshots, and build photos |
| `.drl` | Fabrication outputs such as Gerbers and drill files |

## Credits

- **Hack Club Half Life** for the hardware-program context and project inspiration: [halflife.hackclub.com](https://halflife.hackclub.com/)
- **KiCad** for the open-source electronics design tools: [kicad.org](https://www.kicad.org/)
- **References and contributors:** credit to @SharKingStudios for the Starbie beginner guide and README help.
