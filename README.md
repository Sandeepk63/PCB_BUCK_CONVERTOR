# Buck Converter Project

This repository contains the design files for a **Buck Converter** PCB project, designed using Altium Designer. The project features an adjustable step-down voltage regulator capable of handling various input and output requirements.

## Project Overview

[cite_start]The design is centered around the **LM2596SX-ADJ** step-down regulator[cite: 6, 7]. [cite_start]This "Simple Switcher" power converter is a 150 kHz 3A step-down voltage regulator[cite: 6]. 

![Project Overview](./Screenshot%202026-04-12%20172457.png)

### Key Specifications
* [cite_start]**Regulator IC:** Texas Instruments LM2596 (Adjustable version)[cite: 6, 7].
* [cite_start]**Input Voltage:** Designed for a standard +12V input[cite: 16].
* [cite_start]**Output:** Adjustable via an onboard potentiometer[cite: 11].
* [cite_start]**Power Handling:** Rated for up to 3A[cite: 6].

---

## Hardware Components

[cite_start]The schematic utilizes several key components[cite: 6]:

| Designator | Component | Description |
| :--- | :--- | :--- |
| **U1** | LM2596SX-ADJ | [cite_start]Step-Down Voltage Regulator (TO-263) [cite: 7] |
| **C1** | 680µF Capacitor | [cite_start]Aluminum Electrolytic SMD, 35V [cite: 7] |
| **C2** | 220µF Capacitor | [cite_start]Aluminum Electrolytic Radial, 50V [cite: 10] |
| **D1** | B5819W | [cite_start]Schottky Barrier Rectifier (SOD123) [cite: 8] |
| **L1** | 330µH Inductor | [cite_start]Power Inductor [cite: 10] |
| **VR1** | 10kΩ Potentiometer | [cite_start]Single-Turn Cermet Trimmer [cite: 11] |
| **R1** | 10kΩ Resistor | [cite_start]0805 Surface Mount [cite: 12] |

![Schematic Preview](./Screenshot%202026-04-12%20172738.png)

---

## File Structure

* [cite_start]**`Buck_Convertor.PrjPcb`**: The main Altium project file[cite: 1].
* **`schematic_buck'.SchDoc`**: The circuit schematic[cite: 1, 6].
* **`PCB1.PcbDoc`**: The printed circuit board layout[cite: 1].
* [cite_start]**`Project Outputs for Buck_Convertor/`**: Contains generated fabrication files, including Gerber files and DRC reports[cite: 1].
* **`CAMtastic1.Cam`**: CAM document for fabrication verification[cite: 1].

---

## Fabrication & Testing

![PCB Layout](./Screenshot%202026-04-12%20173030.png)

1. **Software:** You will need **Altium Designer** to open the project and modify the design[cite: 1].
2. **Fabrication:** Gerber files (e.g., `.GTL`, `.GBL`) are provided in the outputs folder for manufacturing[cite: 1, 3].
3. **Testing:** The board includes dedicated test points (**in1**, **in2**, **out1**, **out2**) for monitoring input and output voltages[cite: 15, 16].

## Author
**Sandeep Kumar** [cite: 1, 16]
