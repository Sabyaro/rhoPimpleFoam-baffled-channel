# rhoPimpleFoam Simulation for a Baffled Channel

This repository contains a CFD simulation setup using the `rhoPimpleFoam` solver in OpenFOAM, tailored to analyze flow and thermal behavior in a **baffled channel**. The case is designed to compute critical surface quantities such as **wall heat flux** and **wall shear stress** while resolving common numerical challenges like initial temperature instabilities.

## 📌 Overview

The simulation focuses on transient compressible flow and conjugate heat transfer in a baffled geometry. This case is valuable for understanding flow separation, recirculation, and enhanced heat transfer in industrial geometries such as:

- Heat exchangers
- Cooling channels with obstacles
- HVAC systems

### 🔍 Key Features

- ✅ **Solver Used**: `rhoPimpleFoam` — a transient solver for compressible flow, combining PISO and SIMPLE algorithms.
- ✅ **Geometry**: Baffled channel created using `blockMesh`.
- ✅ **Stabilized Initialization**: `fvOptions` file is used to mitigate unphysical behavior due to initial temperature gradients.
- ✅ **Wall Post-Processing**: `controlDict` is configured to compute `wallHeatFlux` and `wallShearStress`.

---
📊 Goals of the Simulation
1. Investigate velocity and pressure distribution in baffled regions

2. Assess impact of obstacles on shear stress and heat transfer enhancement

3. Develop stable startup for temperature-driven simulations in compressible flows

🧠 Future Enhancements

> Coupling with conjugate solid domain for full thermal modeling

> Implement turbulence models like k-ω SST or LES

> Parametric study on baffle shape, spacing, and Reynolds number



