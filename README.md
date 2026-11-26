# GNSS L1 RHCP Microstrip Patch Antenna

CST Microwave Studio project: design and electromagnetic simulation of a right-hand circularly polarized (RHCP) microstrip patch antenna for the GPS/GNSS L1 band.

## Project Overview

The target operating frequency is **1.575 GHz (GPS L1)**. The design uses a microstrip patch on an FR-4 substrate and corner truncation to generate circular polarization. The project explores antenna geometry, feed configuration, impedance matching, and simulated antenna performance.

## Design Workflow

- Build the patch antenna and substrate model in CST Microwave Studio.
- Tune the geometry and feed to obtain a resonance near the GNSS L1 frequency.
- Use corner truncation to support RHCP operation.
- Evaluate impedance matching and circular-polarization performance from the simulated results.

## Reported Simulation Results

The following values are from an optimized simulation configuration documented during the project:

| Parameter | Result |
|---|---:|
| Target frequency | 1.575 GHz |
| Reflection coefficient, S11 | -16.7 dB |
| Axial ratio | 1.81 dB |
| VSWR | 1.359 |

These are **simulation results**, not measured prototype results.

## Files

- `antennadesign.cst` — CST Microwave Studio project.
- [Lab report (PDF)](Lab_report%20(1).pdf) — project documentation and results.

## Tools and Topics

- CST Microwave Studio
- Microstrip antenna design
- GNSS / GPS L1
- Circular polarization (RHCP)
- Impedance matching
- S-parameter and axial-ratio evaluation

## Notes

The CST project file can be opened in CST Studio Suite. The report provides additional background and project documentation.

---

**Author:** Ziad Ahmed Fergany  
**Focus:** RF & Microwave Engineering · Antenna Design
