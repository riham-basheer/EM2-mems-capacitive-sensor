# Electromagnetics II

**Technologies:** COMSOL Multiphysics (Electrostatics Module)

## About
Designed and simulated a MEMS comb-drive capacitive sensor using finite element analysis — connecting Maxwell's equations to practical sensor performance through 3D modeling and parametric sweeps.

---

# Capacitive MEMS Sensor Design — COMSOL Simulation

**Technologies:** COMSOL Multiphysics (Electrostatics Module)

## Overview
Designed and simulated a MEMS comb-drive capacitive sensor using COMSOL Multiphysics. Modeled the 3D geometry from scratch, applied electrostatic physics, and analyzed how geometric parameters affect sensor capacitance and electric field distribution — connecting theory to practical sensor performance.

## What I Did

### 3D Geometry & Physics Setup
- Built the comb-drive structure in COMSOL: interdigitated fingers with 4 μm thickness on a 10 μm substrate
- Applied 4V to one arm, grounded the other
- Specified dielectric permittivities for all materials and solved Poisson's equation via the Electrostatics module

### Capacitance vs. Gap (Parameter Sweep)
- Designed and executed a parameter sweep varying finger engagement D from 30 μm to 100 μm (step of 2 μm)
- Computed capacitance at each point
- Demonstrated a linear increase in capacitance with D — consistent with theory: closer electrode spacing increases capacitance, and multiple finger pairs in parallel sum their individual contributions

### Electric Field & Potential Visualization
- Mapped the electric potential distribution and the y-component of the electric field
- Identified three distinct field line types and their mechanical effects:
  - **Vertical side-to-side fields (strong):** Align fingers — contribute to sensor force
  - **Top-side distant fields (weak):** Tend to disengage fingers
  - **Tip-to-side fringe fields:** No contribution to alignment force — but critical for proximity sensing

### E vs. V Relationship
- Plotted applied potential against the y-component of the electric field
- Confirmed the quadratic relationship E ∝ V² as expected from electrostatic theory

## Key Findings
- Capacitance scales linearly with D — confirming the parallel-plate model for multi-finger comb-drive sensors
- Fringe fields are the sensing mechanism — they extend beyond the plane of the conductors, enabling detection of nearby objects
- Not all field lines contribute equally — understanding which fields drive alignment vs. sensing is critical for MEMS design

## Key Takeaways
- Translated electrostatic theory into an observable, parameterizable sensor model
- Sweeping geometric parameters and visualizing field distributions bridged the gap between Maxwell's equations and MEMS design
- Demonstrated why comb-drive geometry is chosen for precision capacitive sensing