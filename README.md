# Computer-Aided-Design-Techniques_Project
DIY Liquid Level Detection Circuit

# Liquid Level Detection Circuit – CAD Project (Semester II, 2025)

## Overview
This project presents a simulated electronic system designed to **monitor and signal liquid levels** within a container using a resistive sensor. The system is fully designed and tested in **OrCAD**, utilizing standard analog components like operational amplifiers, resistors, and LEDs for visual feedback.

## Functionality
- A resistive sensor with a **linear variation from 14 kΩ to 28 kΩ** corresponds to a liquid height between **0 and 285 cm**.
- The sensor forms a **voltage divider** with a fixed resistor (21.5 kΩ) to produce a voltage signal based on liquid height.
- A **buffer amplifier (TL082)** ensures a stable signal for comparison.
- **Three voltage comparators** detect when the liquid level exceeds specific thresholds and activate colored LEDs:
  - **Red LED** for low level
  - **Yellow LED** for medium level
  - **Green LED** for high level

## Thresholds (cm ➜ inches)
The system triggers visual indicators based on the following liquid height thresholds, also converted to inches:

| Level        | Height (cm) | Height (inches) |
|--------------|-------------|------------------|
| Low          | < 80 cm     | < 31.5 in        |
| Medium       | 80–150 cm   | 31.5–59.1 in     |
| High         | > 150 cm    | > 59.1 in        |

*Conversion: 1 inch = 2.54 cm*

## Simulation Techniques
Multiple simulation analyses were used to validate the circuit:
- **Transient Analysis**: Verifies dynamic stability.
- **Parametric Sweep**: Checks linearity of sensor response.
- **Monte Carlo**: Assesses tolerance impacts on thresholds.
- **Worst-Case**: Ensures robustness in extreme scenarios.

## Tools Used
- **OrCAD Capture & PSpice**
- Standard analog components (resistors, TL082 op-amp, LEDs)
- eTape liquid level sensor model

## Author
**Alexandru-Gabriel Brabete**  
2nd Year 

## References
See the full project documentation for schematics a simulation details
