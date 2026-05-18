
<h1 align="center">
  <br>
  <img width=19% alt="image" src="https://github.com/user-attachments/assets/c8f81ec5-089a-4a20-8c75-ff4b583b7dfd" />
  <br>
  APX DEVBOARD
  <br>
</h1>

<h4 align="center">
A STM32 based devboard with Buttons, a LED and 8 GPIO pins.
</h4>

<div align="center">

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Project](https://img.shields.io/badge/Project-Hardware-yellow.svg)
![Series](https://img.shields.io/badge/Series-APX-red.svg)
![Hackatime Badge](https://hackatime-badge.hackclub.com/U0A2SJ7B739/RESOLUTION%20DEVBOARD)

</div>

<p align="center">
  <a href="#about-the-project">About</a> •
  <a href="#repository-structure">Structure</a> •
  <a href="#schematic-on-kicad">Schematic</a> •
  <a href="#pcb-on-kicad">PCB</a> •
  <a href="#CAD">CAD</a> •
  <a href="#bill-of-materials">BOM</a> •
  <a href="#license">License</a> •
  <a href="#credits">Credits</a>
</p>

<br>
<br>
<p align=center>
<img width=80% alt="banner" src="https://github.com/user-attachments/assets/1a03fb36-2362-4ddb-9e22-4016e1b35800" />


</p>

## About the Project

**APX DEVBOARD** is a STM32 based devboard designed with GPIO pins, buttons and an LED

### Features

- **STM32G431CBT6** MCU 32-Bit 170MHz 128KB (128K x 8) FLASH 48-LQFP (7x7)
- **8 GPIO pins** to help make any hardware project
- **GPIO linked LED** to program it without needing an external LED
- **GPIO linked button** to use it without needing an external button
- **BOOT and RESET buttons**
- **USB-C input**
- **Amiri silkscreen** for a professional look
- **Original edge cut** to look cool lol
- **Small size** of 2.3*3.7 cm

## Repository Structure

- `src/` — KiCad and Fusion360 project sources
- `production/` — PCB and CAD fabrication files (Gerbers, BOM, Pick & Place, 3mf)
- `images/` — images used in the README and documentation

## Schematic on KiCad

Source : `src/schem`  

<img width=90% alt="Capture d&#39;écran 2026-05-12 005443" src="https://github.com/user-attachments/assets/72e2f2ab-9be3-47b6-a6d2-7fb9fac3bd40" />



## PCB on KiCad

Source : `src/pcb/`  

<div align="center">
  <table>
    <tr>
      <td valign="bottom"><img width=100% alt="image" src="https://github.com/user-attachments/assets/29cef8c3-a4b7-4903-ad75-b839e9825c97" /></td>
      <td valign="bottom"><img width=100% alt="Capture d&#39;écran 2026-05-12 010605" src="https://github.com/user-attachments/assets/3b472e1d-b635-426f-a7e0-d8d084e70b27" /></td>
      <td valign="bottom"><img width=100% alt="Capture d&#39;écran 2026-05-12 010555" src="https://github.com/user-attachments/assets/69088e1d-ac4f-472f-8fa1-4bd4c43c3400" /></td>
  </table>
</div>
<div align="center">
  <table>
    <tr>
      <td valign="bottom"><img width=100% alt="Capture d&#39;écran 2026-05-12 010746" src="https://github.com/user-attachments/assets/40868afa-0214-426a-b003-32e463abf93a" /></td>
      <td valign="bottom"><img width=100% alt="Capture d&#39;écran 2026-05-12 010754" src="https://github.com/user-attachments/assets/bafa0d8f-0914-42bf-94ea-4730fb627c44" /></td>
  </table>
</div>  


> The PCB design is made on only 2 layers, to reduce the cost of the board !  

<br>

## Share Links

go check out the pcb on [KiCanva](https://kicanvas.org/?github=https://github.com/Gabouin/APX_DEVBOARD/blob/main/src/APX%20Devboard.kicad_pcb) !
<br>
go check out the case on [Fusion360](https://a360.co/4uNEBf6) !

<br>

## CAD

Source : `src/CAD` and
         `production/CAD`

<div align="center">
  <table>
    <tr>
      <td valign="bottom"><img width="547" height="565" alt="Capture d&#39;écran 2026-05-19 003227" src="https://github.com/user-attachments/assets/0351fa97-3902-4bd5-ae9c-1e3e2e8a36cc" /></td>
      <td><img width="602" height="515" alt="Capture d&#39;écran 2026-05-19 003627" src="https://github.com/user-attachments/assets/5d442b80-dcd1-4693-8da4-0410cd78a075" /></td>
    </tr>
  </table>
</div>

<br>


## Bill of Materials

Source: `production/pcb/bom.csv`

|Designator                       |Footprint                       |Quantity|Value           |LCSC Part #|
|---------------------------------|--------------------------------|--------|----------------|-----------|
|PA2                              |0603                            |1       |LED             |C2286      |
|BOOT                             |SW-SMD_L3.9-W3.0-P4.45          |1       |BOOT            |C455280    |
|C11, C12, C5, C6, C8             |0603                            |5       |1uF             |C15849     |
|C1, C10, C2, C3, C4, C7          |0603                            |6       |100nF           |C14663     |
|C9                               |0603                            |1       |10nF            |C57112     |
|DEBUG                            |PinHeader_1x04_P2.54mm_Vertical |1       |Conn_01x04      |C2691448   |
|J1                               |PinHeader_1x05_P2.54mm_Vertical |1       |Header Left     |C124379    |
|J2                               |PinHeader_1x05_P2.54mm_Vertical |1       |Header Right    |C124379    |
|PA3                              |SW-SMD_L3.9-W3.0-P4.45          |1       |PA3             |C455280    |
|R1, R2                           |0603                            |2       |100k            |C23186     |
|R3, R4, R7                       |0603                            |3       |10k             |C25804     |
|R6, R5                           |0603                            |2       |5.1k            |C25803     |
|RESET                            |SW-SMD_L3.9-W3.0-P4.45          |1       |RESET           |C455280    |
|STM32                            |LQFP-48_L7.0-W7.0-P0.50-LS9.0-BL|1       |STM32G431CBT6   |C529355    |
|U1                               |SOT-23-3                        |1       |XC6206PxxxMR    |C5446      |
|USB-C1                           |USB-C-SMD_TYPE-C-16PIN-2MD-073  |1       |TYPE-C 16PIN 2MD|C2765186   |

## JLPCB order

<div align="center">
  <table>
    <tr>
      <td valign="bottom"><img width=85% alt="image" src="https://github.com/user-attachments/assets/d4035cf5-02b6-49b9-a1f5-948ee2a729e2" /></td>
      <td valign="bottom"><img width=100% alt="image" src="https://github.com/user-attachments/assets/420f9535-a772-4240-a25a-6e6930607eb8" /></td>
  </table>
</div>  



## You might also like

- [APX USB HUB](https://github.com/gabouin/APX-USB-HUB) - A PTC-secured USB HUB designed for [Macondo - Hack Club](https://macondo.hackclub.com)
- [HackPad](https://github.com/Gabouin/Hackpad) - A 6-keys macropad designed for [Blueprint - Hack Club](https://blueprint.hackclub.com)
- See more in my [github](https://github.com/gabouin)


## License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.


## Credits

This project uses:

- **KiCad** - PCB design and schematic capture
- **JLCPCB** - PCB manufacturing
- **LCSC** - Parts order
- **Figma** - Silkscreen and banner design
- **Fusion 360** - CAD
- **[@NotARoomba](https://github.com/notaroomba)** - Readme template



