
# XOR Gate Design, Simulation, and Layout using 180nm Technology

![gitbanner](https://github.com/afzalamu/XOR-gate-design-simulation-and-layout-using-180nm-Technology-LTSpice-ElectricBinary/assets/124300839/8f0f9e83-cb62-49a0-a426-4d987972415b)


## Overview

Welcome to the XOR Gate Design project, an assignment of coursework for ELC3611 VLSI Design & Technology in the fifth semester. This project focuses on implementing the XOR function using CMOS logic in TSMC 180nm technology. The design, simulation, and layout were conducted using LTSpice for design and simulation, and Electric Binary for layout.

### Technology File

- **Technology Used:** TSMC 180nm

### Tools Used

- **Design and Simulation:** [LTSpice](link-to-ltspice)
- **Layout Design:** [Electric Binary](link-to-electric)

## Project Details

The primary objective was to implement the XOR function with specific design parameters:
- All PMOS transistors: 20λ wide
- All NMOS transistors: 10λ wide
- Cell height: 6 Metal-1 tracks
- Cell width optimized for minimum area
- λ (Technology Parameter): 100 nm

**Transistor Sizing Reference:**
Transistor sizing was done with respect to a reference inverter with the following dimensions:
- PMOS width: 2u
- NMOS width: 1u

The repository includes:
- CMOS schematic
- Pre-layout simulation waveforms
- Stick diagram
- Layout
- Post-layout simulation waveforms
- Layout area

## CMOS Schematic

![schematic](https://github.com/afzalamu/XOR-gate-design-simulation-and-layout-using-180nm-Technology-LTSpice-ElectricBinary/assets/124300839/73d710a3-9cf4-4688-bc3d-e2235f1bf48d)


The CMOS schematic showcases the key elements and design considerations.


## Pre-layout Simulation

![pre layout simulation](https://github.com/afzalamu/XOR-gate-design-simulation-and-layout-using-180nm-Technology-LTSpice-ElectricBinary/assets/124300839/bb31f323-4a69-48f2-9ac5-3ce923bae373)

To obtain these waveforms transient analysis is performed in LT Spice, using the ```.tran 50u ``` command.
And the simulation results are in accordance with the functioning of the XOR gate.

### LTSpice Commands for Delay Measurement

```plaintext
.meas time_12 find when V(A) = 0.9V rise = 1
.meas time_22 find when V(vout) = 0.9V fall = 1
.meas TPHL time_22 - time_12
.meas time_32 find when V(A) = 0.9V fall  = 2
.meas time_42 find when V(vout) = 0.9V rise = 2
.meas TPLH  time_42 - time_32
.meas dealy param (TPHL + TPLH)/2
```
#### Input-A to Output Delay (Pre-Layout Delay)
![pre layout delay](https://github.com/afzalamu/XOR-gate-design-simulation-and-layout-using-180nm-Technology-LTSpice-ElectricBinary/assets/124300839/bb832be1-331b-4841-8d72-90b278adb3e9)

``` Pre-Layout Delay from input A to output is 50 us ```

## Stick Diagram and Layout Methodology

The stick diagram and layout employed the Euler path method, resulting in an efficient and compact design.

## Layout

![layout](https://github.com/afzalamu/XOR-gate-design-simulation-and-layout-using-180nm-Technology-LTSpice-ElectricBinary/assets/124300839/27e61e73-5a21-4b1d-92f3-db1f002ef2d5)

The layout is designed using the application of the Euler path method and considerations for minimum area optimization.

### Post-layout Simulation

![post layout simulation](https://github.com/afzalamu/XOR-gate-design-simulation-and-layout-using-180nm-Technology-LTSpice-ElectricBinary/assets/124300839/6eb563ad-782c-4bb8-b892-eeff43407b59)


#### Input-A to Output Delay (Post-Layout Delay)
![post layout delay](https://github.com/afzalamu/XOR-gate-design-simulation-and-layout-using-180nm-Technology-LTSpice-ElectricBinary/assets/124300839/114e2a07-c251-4544-9df1-829af7b52194)

``` Post-Layout Delay from input A to output is 20 us ```

#### Area Calculation

The area  can be calculated using the measuring tool in Electric Binary.
Here, in the layout figure, the length and width are measured, and as a result area can be calculated.
![layout arae](https://github.com/afzalamu/XOR-gate-design-simulation-and-layout-using-180nm-Technology-LTSpice-ElectricBinary/assets/124300839/04dca9e9-1a4c-4aa9-b55d-3aa1dbf38e32)

## Author

- [Afzal Malik](https://github.com/afzalamu)

