# SAS Engineering
## ASME Section VIII, Division 1 — Pressure Vessel Design Suite

A browser-based engineering calculation suite for selected pressure vessel design calculations based on **ASME BPVC Section VIII, Division 1**.

> 🚧 **Status: Beta / Under Development**

SAS Engineering is a personal engineering software project developed to bring commonly used pressure vessel design calculations into one simple, browser-based interface.

The idea is straightforward:

> Enter the design conditions and geometry, perform the relevant code-based calculation, and clearly see how the result compares with the design requirement.

The suite is being developed with a focus on **engineering transparency**, rather than simply providing a final calculated number.

---

## Current Modules

### Pressure Boundaries

- **UG-27 — Internal Pressure: Shell Thickness**
  - Cylindrical shells
  - Spherical shells

- **UG-32 — Formed Heads**
  - Ellipsoidal heads
  - Torispherical heads
  - Hemispherical heads

- **UG-28 — External Pressure: Cylindrical Shells**
  - External pressure evaluation
  - Buckling-related calculations

- **UG-33 — External Pressure: Formed Heads**
  - External pressure evaluation
  - Allowable external pressure
  - Factor A / Factor B based evaluation

### Openings, Reinforcement & Welds

- **UG-37 — Opening Reinforcement**
  - Required reinforcement area
  - Available reinforcement area
  - Reinforcement checks

- **UG-37 / UG-40 — Reinforcement Pad Sizing**
  - Pad outside diameter
  - Reinforcement limits

- **UG-39 — Flat Head Reinforcement**
  - Area replacement calculations

- **UW-16 — Weld Sizing & Efficiency**
  - Weld sizing
  - Joint efficiency considerations

### Flanges & Bolting

- **Appendix 2 — Flange Moment**
  - Operating condition
  - Gasket seating condition
  - Flange moment calculations

- **Appendix 2 — Bolt Sizing & Loads**
  - Required bolt area
  - Bolt loading
  - Over-bolting checks

### Stress, MAWP & Material Checks

- **UG-23 — Stress Limits**
  - General membrane stress
  - Local stress
  - Shear stress limits

- **UG-34 — Unstayed Flat Heads**
  - Flat head thickness
  - Bending-based calculations

- **UG-98 / UG-99 — MAWP & Pressure Testing**
  - Limiting component MAWP
  - Test pressure calculations

- **UCS-66 — MDMT / Brittle Fracture**
  - Exemption curves
  - Temperature-related material considerations

---

## How the Calculators Work

Each module follows a similar engineering workflow:

```text
Design Conditions
        ↓
Geometry
        ↓
Material Parameters
        ↓
Code Calculation
        ↓
Intermediate Results
        ↓
Allowable / Required Value
        ↓
Comparison with Design Requirement
        ↓
Engineering Result
```

The objective is to make the calculation process visible and easier to review instead of presenting only a final answer.

---

## Example: External Pressure - UG-33

A typical calculation follows the sequence:

```text
Head Geometry
      ↓
Equivalent Radius
      ↓
Ro / te
      ↓
Factor A
      ↓
Factor B
      ↓
Allowable External Pressure
      ↓
Compare with Design Pressure
      ↓
PASS / REVIEW
```

The calculator displays important intermediate values so that the engineer can understand how the final result was obtained.

---

## Engineering Approach

The suite is being developed around a few simple principles.

### 1. Keep the calculation visible

Important intermediate values should be shown rather than hidden behind a single "Calculate" button.

### 2. Keep inputs explicit

Design pressure, temperature, geometry, thickness, corrosion allowance, material parameters and other relevant inputs are entered separately.

### 3. Make the result easy to review

The final result should clearly show:

- Calculated value
- Allowable / required value
- Design value
- Governing condition
- PASS / REVIEW status

### 4. Make verification possible

The calculations are being checked against independent engineering calculations and benchmark cases as the project develops.

---

## Beta Status

This project is currently in **Beta**.

The suite is actively being developed and the calculation modules are being reviewed and tested.

Current development areas include:

- Independent calculation checks
- Benchmark examples
- Input validation
- Edge-case testing
- Calculation transparency
- Improved engineering documentation
- Additional design modules
- User interface improvements

If you find an error, unexpected result or possible improvement, please raise an issue in the repository.

---

## Code & Calculation Basis

The calculations are based on selected methodologies from the:

**ASME Boiler and Pressure Vessel Code**

- Section VIII, Division 1
- Relevant requirements referenced by individual calculation modules
- Section II, Part D where applicable

Each module should be used together with the applicable ASME Code requirements and the appropriate code edition.

**Code edition implemented:** `[2023]`

---

## Important Disclaimer

SAS Engineering is an **independent engineering software project**.

It is **not affiliated with, endorsed by, or certified by ASME**.

The software is currently intended for:

- Engineering study
- Preliminary design
- Calculation development
- Learning
- Engineering software development
- Independent calculation checks

The results should **not be treated as a replacement for the applicable ASME BPVC, qualified engineering judgement, design verification, inspection requirements or certification procedures**.

Before using any result for an actual pressure vessel design, fabrication or certification activity, the calculation should be independently reviewed and verified against the applicable current Code requirements.

---

## Technology

The current version is built as a lightweight browser-based application using:

- HTML
- CSS
- JavaScript

No specialised software installation is required to access the web-based interface.

---

## Project Structure

The repository contains individual calculation modules together with a central interface.

Example:

```text
MasterUI.html
│
├── UG27.html
├── UG28.html
├── UG32.html
├── UG33.html
├── UG37.html
├── UG39.html
├── UW16.html
├── APP2FD.html
├── APP2Bolt.html
├── UG23.html
├── UG34.html
├── UG98-99.html
└── UCS66.html
```

The exact module list will continue to evolve during the beta phase.

---

## Who Is This For?

SAS Engineering is intended primarily for people working or learning in areas such as:

- Pressure vessel design
- Static equipment
- Mechanical design
- Engineering analysis
- Process equipment
- CAE / FEA
- Mechanical engineering education

---

## Roadmap

Planned improvements include:

- [ ] More Section VIII Division 1 calculation modules
- [ ] More independent benchmark cases
- [ ] Calculation verification library
- [ ] Detailed calculation breakdowns
- [ ] Improved input validation
- [ ] Engineering calculation reports
- [ ] Improved material-property handling
- [ ] Additional nozzle and flange calculations
- [ ] Additional stress and stability checks
- [ ] Improved user interface
- [ ] Better mobile support

---

## Feedback

This is an independent engineering project and practical feedback is welcome.

If you work with pressure vessels, static equipment, mechanical design or ASME-based calculations, feedback on the following is particularly useful:

- Calculation methodology
- Engineering assumptions
- Boundary conditions
- Edge cases
- Usability
- Verification cases
- Additional useful modules

Please use **GitHub Issues** to report problems or suggest improvements.

---

## About the Author

**Suraj Suryawanshi**

Mechanical Product Design & Development Engineer  
IIT M.Tech | NPD / NPI | Mechanical Design | CAE / FEA | ASME | DFM / DFA

This project is part of my broader work in mechanical engineering, product development, simulation and engineering automation.

**Engineering Portfolio:** `[https://geasskami.github.io/Portfolio/SAS_MS.html]`

**LinkedIn:** `[www.linkedin.com/in/surajas]`

---

## Project Status

**Current version:** Beta  
**Project type:** Independent engineering software project  
**Focus:** Pressure Vessel Design & Engineering Calculations
