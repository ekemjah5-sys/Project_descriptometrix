# Physics-Informed Matrix Engine for Bypassing Scaling Relations in Alkyne Purification

[![License: MIT](https://shields.io)](https://opensource.org)
[![Python 3.8+](https://shields.io)](https://python.org)
[![LaTeX Document](https://shields.io)](https://overleaf.com)

This repository contains the official reproducible framework and analytical source code for the manuscript **"A physics-informed matrix engine bypasses scaling relations in alkyne-poisoned catalytic interfaces"** targeted for *Nature Catalysis*.

## 🚀 Overview

Discovering catalyst surfaces capable of resisting trace alkyne impurities during olefin purification is fundamentally throttled by thermodynamic linear scaling relations. Traditional static electronic metrics (e.g., d-band center projections) fail to distinguish between non-destructive, transient π-coordination and destructive, irreversible σ-acetylide poisoning.

This project introduces an analytical quantum-mechanical screening engine based on a modified three-center Hückel-Coulson Hamiltonian framework. Processing candidate configurations in **< 0.2 milliseconds**, the engine maps electronic phase boundaries by isolating two dynamic, wavefunction-based descriptors:
1. Local π-backbonding susceptibility (\(\Delta E_{\pi}\)) — *Proxy for high reversible activation.*
2. Coulson terminal carbon charge redistribution (\(\Delta q_{C1}\)) — *Proxy for poisoning deactivation resistance.*

---

## 🛠️ Installation & Dependencies

The physics engine is written in standard Python and utilizes optimized linear algebra solvers. 

### Prerequisites
Ensure you have an environment configured with `numpy` and `scipy`. You can initialize a clean workspace using Anaconda or standard pip:

```bash
pip install numpy scipy
```

---

## 💻 Standalone Execution Suite

You can execute the core physics validator engine directly from your terminal interface to confirm reproducibility against our reported benchmarks:

```bash
python matrix_engine.py
```

### Analytical Verification Baseline
When using our verified single-atom alloy data arrays, the script outputs the following verification profile:

```text
======================================================================
 DESCRIPTOMETRIX MATRIX ENGINE: VERIFICATION & BENCHMARK SUITE
======================================================================
Catalyst Environment : Pd(111) Top
Alkyne Intermediary  : Nitro-Phenyl

--> Calculated E_pi (Susceptibility)      : 7.7137 eV
--> Calculated q_C1 (Carbon Polarization) : -0.0177 e
--> Ground State Bonding Energy Level     : -13.3016 eV
======================================================================
```

---

## 📁 Repository Structure

```text
├── main.tex             # LaTeX unified source file for paper review
├── cover_letter.tex     # Formal editorial communication script
├── matrix_engine.py     # Standalone Python tight-binding module
├── .gitignore           # LaTeX and workspace upload exclude map
└── README.md            # Repository usage documentation
```

---

## ✒️ Citation & Authorship

**Title:** A physics-informed matrix engine bypasses scaling relations in alkyne-poisoned catalytic interfaces  
**Corresponding Author:** Aniema Ekemini (ekemjah5@gmail.com)  
**Co-Author:** Ededet Asuquo  
**Institution:** Department of Science, Southern British High School, Calabar, CRS, Nigeria  

*For inquiries regarding high-throughput data arrays (300,000 processed configurations) or microkinetic Kinetic Monte Carlo execution matrices, please reach out to the corresponding author.*

---
Licensed under the [MIT License](LICENSE).
