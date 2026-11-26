# GNSS L1 RHCP Microstrip Patch Antenna

CST Microwave Studio project for the electromagnetic design and simulation of a right-hand circularly polarized (RHCP) microstrip patch antenna targeting the GPS/GNSS L1 band.

## Project Overview

- **Target band:** GPS L1
- **Target frequency:** 1.575 GHz
- **Antenna type:** Corner-truncated microstrip patch
- **Polarization objective:** RHCP
- **Simulation tool:** CST Microwave Studio

The design uses corner truncation to excite two orthogonal patch modes with the phase relationship required for circular polarization. The project covers geometry definition, feed configuration, impedance matching, and far-field evaluation.

## Antenna Geometry

The dimensions below are taken from the design table supplied with the CST results.

| Parameter | Description | Value |
|---|---|---:|
| $L_p$ | Patch length | 44.65 mm |
| $W_p$ | Patch width | 44.65 mm |
| $t$ | Corner truncation length | 8.485 mm |
| $W_f$ | Feed-line width | 3 mm |
| $h$ | Substrate thickness | 1.6 mm |
| $L_g$ | Ground-plane length | 100 mm |
| $W_g$ | Ground-plane width | 100 mm |

## CST Simulation Results

The following values are read from the supplied CST plots. They describe **simulation results**, not measurements from a fabricated antenna.

| Metric | Result | Interpretation |
|---|---:|---|
| VSWR at 1.575 GHz | 1.3575 | Good impedance match at GPS L1 |
| Axial-ratio 3 dB lower edge | 1.5702 GHz | From the plotted 3 dB crossing |
| Axial-ratio 3 dB upper edge | 1.5902 GHz | From the plotted 3 dB crossing |
| 3 dB axial-ratio bandwidth | 20 MHz | The 1.575 GHz target is inside this interval |
| Minimum plotted S11 | Approximately -19 dB near 1.555 GHz | Approximate visual reading of the S11 trace |

### Important frequency observation

The deepest S11 notch in the supplied plot appears near **1.555 GHz**, slightly below the GPS L1 target of 1.575 GHz. However, the VSWR marker at 1.575 GHz is approximately **1.3575**, and the plotted axial-ratio bandwidth below 3 dB includes 1.575 GHz. Further fine-tuning could bring the deepest impedance resonance closer to the exact L1 center frequency while preserving the circular-polarization bandwidth.

## Far-Field Evaluation

The supplied CST results include:
- A 3D far-field radiation/directivity visualization.
- A two-dimensional far-field directivity cut at $\phi = 0^\circ$.

The screenshots show the radiation-pattern shape, but the peak directivity/gain value is not sufficiently identified in the supplied plots, so no numerical gain claim is made here.

## Project Files

- `antennadesign.cst` — CST Microwave Studio antenna model.
- [Lab report (PDF)](Lab_report%20(1).pdf) — project report and supporting documentation.

## Tools and Engineering Topics

- CST Microwave Studio
- Microstrip patch antenna design
- GNSS / GPS L1
- RHCP and circular polarization
- Corner truncation
- Impedance matching
- S-parameters and VSWR
- Axial-ratio bandwidth
- Far-field radiation-pattern analysis

## Reproducibility and Scope

Open the `.cst` project in CST Studio Suite to inspect the model and simulation setup. The reported values above are transcribed from the supplied result plots; they should be treated as simulation results unless independently confirmed by prototype measurements.

---

**Author:** Ziad Ahmed Fergany  
**Focus:** RF & Microwave Engineering · Antenna Design
