# Starbie!

A custom printed circuit board designed in KiCad as part of [Hack Club's Half Life](https://halflife.hackclub.com/) hardware program. Starbie is a tiny motion-controlled digital pet: basically a desktop Tamagotchi with minimal gameplay buttons. Instead of pressing controls, you interact with it by physically moving the board.

## Take a look

<img width="1318" height="745" alt="Screenshot 2026-10-11 165803" src="https://github.com/user-attachments/assets/92cd74cf-9d42-4341-950f-21084106061d" />

## What it is

Starbie is designed to sit on your desk, show its personality on a small display, and react to how you handle it. Tilting, moving, and otherwise checking in on your pet are meant to be part of the experience.

The board includes a microcontroller, display, motion sensor, and environmental sensor in a compact PCB design. It is USB powered and built around beginner-friendly through-hole soldering for the add-on components.

## Project status

The PCB design, renders, and the Arduino starter firmware are included here. The default program is a two-eye pet with a tilt-controlled radial menu, hidden stats, and a shake reaction.

## What’s in the project

- **Schematic:** the circuit diagram and electrical connections.
- **PCB layout:** the physical placement of component footprints and copper routing.
- **3D preview:** a way to check component placement and the overall board before manufacturing.
- **Build documentation:** photos, the bill of materials, and manufacturing files.

## Project files

The repository is intended to contain the following files:

| File or folder | What it contains |
| --- | --- |
| `Starbie.kicad_pro` | Main KiCad project file |
| `Starbie.kicad_sch` | Circuit schematic |
| `Starbie.kicad_pcb` | PCB layout |
| `docs/images/` | PCB renders, screenshots, and build photos |
| `manufacturing/` | Fabrication outputs such as Gerbers, drill files, and a bill of materials, |

## Credits

- **Hack Club Half Life** for the hardware-program context and project inspiration: [halflife.hackclub.com](https://halflife.hackclub.com/)
- **KiCad** for the open-source electronics design tools: [kicad.org](https://www.kicad.org/)
- **References and contributors:** SharKingStudios for the detailed Starbie beginner guide.
