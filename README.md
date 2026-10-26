# ⭐ Starbie

A custom printed circuit board designed in KiCad as part of [Hack Club's Half Life](https://halflife.hackclub.com/) hardware program. Starbie is a tiny star-shaped motion-controlled digital desk buddy with minimal gameplay buttons. Instead of just pressing controls, you interact with it by physically moving the board.

## Take a look

<img width="852" height="675" alt="Starbie Top" src="https://github.com/user-attachments/assets/d973a894-85eb-42e6-a5d3-fb24a9738f0e" />

<img width="1318" height="745" alt="Screenshot 2026-10-11 165803" src="https://github.com/user-attachments/assets/bfbab53e-36b1-4071-8ec7-0e259b057d90" />


## What it is
Starbie is designed to sit on your desk, show its personality on a small display, and react to how you handle it. Tilting, moving, and otherwise checking in on your pet are meant to be part of the experience.

The board includes a microcontroller, display, motion sensor, and environmental sensor in a compact PCB design. It is USB powered and built around beginner-friendly through-hole soldering for the add-on components.

## Project status
The PCB design, renders, and an Arduino starter firmware are included here. The default program is a two-eye pet with a tilt-controlled radial menu, hidden stats, and a shake reaction.

## Software
Firmware/ contains one self-contained Arduino IDE sketch for the XIAO ESP32-C3. Builders customize pins, menu actions, starting values, and motion settings together at the top of the sketch. The folder also includes a draggable browser simulator.

## Bill of Materials (BOM)
This bill of materials lists the components required to build Starbie, including quantities, estimated costs, descriptions, and supplier links.

| Part | Description | Quantity | Unit Cost | Total Cost | Vendor |
|---|---|---:|---:|---:|---|
| 10k Resistor | Pull-up resistor used on the I2C bus lines or DHT11 data line to help ensure a stable signal. | 1 | $0.05 | $0.05 | [Amazon](https://www.amazon.com/dp/B0B4JFPHTW?th=1) |
| MX Switches | Momentary switches used for Reset (EN), Boot (GPIO9), or other user inputs. | 2 | $0.18 | $0.36 | [Amazon](https://www.amazon.com/dp/B0FQP8VYX4) |
| XIAO ESP32-C3 | Main microcontroller board responsible for running the firmware and processing sensor data. | 1 | $4.90 | $4.90 | [Seeed Studio](https://www.seeedstudio.com/Seeed-XIAO-ESP32C3-p-5431.html) |
| DHT11 | Temperature and humidity sensor for collecting environmental data. | 1 | $3.33 | $3.33 | [Amazon](https://www.amazon.com/dp/B0BLG7R99R) |
| Custom PCB | Printed circuit board connecting the electronic components. | 1 | $4.00 | $4.00 | [JLCPCB](https://cart.jlcpcb.com/quote?stencilLayer=2&stencilWidth=100&stencilLength=100&stencilCounts=5&plateType=1&spm=Jlcpcb.Homepage.1010) |
| 0.96-inch OLED Display | OLED display used to show Starbie's interface and information. | 1 | $6.00 | $6.00 | [Amazon](https://www.amazon.com/dp/B0GBWXTR1Z?th=1) |
| MPU6050 | Accelerometer and gyroscope module for measuring motion and rotation. | 1 | $7.00 | $7.00 | [Amazon](https://www.amazon.com/Wishiot-MPU-6050-Accelerometer-Gyroscope-Converter/dp/B0C3LDTTBJ) |
| Keycaps | Keycaps fitted onto the MX switches for physical user input. | 2 | $0.60 | $1.20 | *I had some spares lying around so I didn't add a supplier link but these are good: [Amazon] (https://www.amazon.com/Profile-Keycaps-Mechanical-Keyboard-Installation/dp/B0CNZJSBRZ/ref=sxbs_pa_sp_search_thematic_btf_sspa?content-id=amzn1.sym.42489dc0-23c6-4615-8826-cd84282ad669%3Aamzn1.sym.42489dc0-23c6-4615-8826-cd84282ad669&cv_ct_cx=keycaps+cheap&keywords=keycaps+cheap&pd_rd_i=B0CNZJSBRZ&pd_rd_r=7dd3c511-a5be-4e19-8841-6df89664dd20&pd_rd_w=lWLCp&pd_rd_wg=ts5wz&pf_rd_p=42489dc0-23c6-4615-8826-cd84282ad669&pf_rd_r=XRSQBKPMWBJWSDXPJXAC&qid=1793025724&sbo=RZvfv%2F%2FHxDF%2BO5021pAnSA%3D%3D&sr=1-4-847e53e6-6a07-4024-a011-ba944385892f-spons&aref=mA4cj2Ly3U&sp_csd=d2lkZ2V0TmFtZT1zcF9zZWFyY2hfdGhlbWF0aWNfYnRm&psc=1)|

### Cost Summary

| Item | Estimated Cost |
|---|---:|
| Components and PCB | $25.64 |
| Shipping and taxes | Not included |
| **Total Estimated Cost** | **$25.64** |

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
