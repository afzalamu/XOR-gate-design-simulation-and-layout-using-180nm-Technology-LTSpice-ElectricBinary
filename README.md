
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

![CMOS Schematic](link-to-cmos-schematic)

The CMOS schematic showcases the key elements and design considerations.


## Pre-layout Simulation

![Pre-layout Simulation](link-to-pre-layout-simulation)

Insights from the pre-layout simulation, along with any noteworthy observations or optimizations.

### LTSpice Commands for Delay Measurement

```plaintext
Insert relevant LTSpice commands for delay measurement here
```

## Stick Diagram and Layout Methodology

The stick diagram and layout employed the Euler path method, resulting in an efficient and compact design.

## Layout

![Layout](link-to-layout)

The layout design, including the application of the Euler path method and considerations for minimum area optimization.

### Post-layout Simulation

![Post-layout Simulation](link-to-post-layout-simulation)

Observations from the post-layout simulation, including input-A to Output Delay and other relevant metrics.

#### LTSpice Commands for Delay Measurement (Post-layout)

```plaintext
Insert relevant LTSpice commands for delay measurement in post-layout simulation here
```
#### Input-A to Output Delay and Layout Area

Include details about the observed Input-A to Output Delay and the optimized layout area achieved in the post-layout simulation.

#### Transistor Area Calculation

Include specific commands or methodologies used to calculate the transistor area in the layout.



## Author

- [Your Name](link-to-your-github-profile)

## License

This project is licensed under the [License Name](link-to-license-file) - see the [LICENSE.md](LICENSE.md) file for details.
```

Feel free to customize any additional details as needed.
