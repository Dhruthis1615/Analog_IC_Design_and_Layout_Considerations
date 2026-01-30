# Day 3 — Bandgap Reference (BGR) & 6T SRAM Design and Analysis

This day focused on **Bandgap Reference (BGR) circuit design**, **temperature compensation analysis**, and continued work on a **6T SRAM memory cell** using Cadence Virtuoso. The goal was to understand **temperature-stable voltage generation**, **noise behavior**, and **memory stability**.

---

## 1️⃣ Bandgap Reference (BGR) — Core PTAT & CTAT Analysis

### Objective
To study **PTAT (Proportional To Absolute Temperature)** and **CTAT (Complementary To Absolute Temperature)** voltage behavior and understand how temperature compensation is achieved in bandgap references.

---

### Work Done
- Generated **CTAT voltage** using BJT **VBE**
- Generated **PTAT voltage** using **ΔVBE**
- Performed **temperature sweep analysis**
- Extracted and compared **PTAT and CTAT slopes**
- Verified complementary temperature trends

---

### Key Observations
- **CTAT (VBE)** decreases with increasing temperature  
- **PTAT (ΔVBE)** increases with increasing temperature  
- Slope comparison confirms the basis for **temperature compensation**

---

### Plots Included
- VBE vs Temperature (CTAT behavior)
- PTAT vs CTAT comparison
- PTAT & CTAT slope analysis

---

## 2️⃣ Op-Amp Based Bandgap Reference (Final BGR Circuit)

### Objective
To combine PTAT and CTAT components using an **op-amp feedback loop** to generate a **temperature-stable reference voltage (VREF)**.

---

### Work Done
- Implemented **Op-Amp Based BGR Architecture**
- Combined PTAT and CTAT through resistor network
- Generated **VREF ≈ constant over temperature**
- Verified bias stability and feedback operation

---

### Noise Spectrum Analysis
Frequency-domain performance was evaluated using:
- **SNR (Signal-to-Noise Ratio)** — Measures signal clarity
- **SFDR (Spurious-Free Dynamic Range)** — Measures spectral purity
- **THD (Total Harmonic Distortion)** — Measures harmonic distortion

---

### Observations
- Lower input amplitude → Better linearity and spectral purity  
- Higher input amplitude → Increased harmonic distortion and THD  
- Noise spectrum validates **reference voltage signal quality**

---

### Plots Included
- Op-Amp Based BGR Schematic
- Noise Spectrum (50 mV input)
- Noise Spectrum (0.5 V input)
- VREF generation plot

---

## 3️⃣ 6T SRAM Cell — Independent Project (Stability & Butterfly Curve Analysis)

### Objective
To independently design and analyze a **6-Transistor (6T) SRAM memory cell**, focusing on **data stability, noise tolerance, and realistic memory behavior**.  
This project was completed **entirely without external help**, demonstrating **strong problem-solving ability, circuit intuition, and core VLSI design skills**.

---

### Work Done
- Designed the **6T SRAM schematic independently from scratch**
- Implemented **cross-coupled inverter-based storage nodes**
- Created the **full memory cell architecture (pull-up, pull-down, access transistors)**
- Performed **DC sweep analysis** to study cell behavior
- Generated the **Butterfly Curve** to evaluate memory stability
- Verified **bistable storage states** (logic ‘0’ and logic ‘1’)
- Analyzed **cell robustness under device sizing constraints**
- Debugged and validated correct **data retention and switching behavior**

---

### Key Concept — Static Noise Margin (SNM)
SNM represents the **maximum noise voltage the SRAM cell can tolerate without flipping stored data**.

- Larger butterfly square → **Higher stability and stronger data retention**
- Smaller butterfly square → **Higher sensitivity to noise and mismatch**

This metric is critical in **commercial memory and cache design**.

---

### Why This Project
This SRAM project demonstrates:
- Ability to **design a complete memory sub-block independently**
- Practical understanding of **memory architecture and stability challenges**
- Experience with **industry-relevant SNM and butterfly curve analysis**
- Strong **debugging, transistor sizing, and validation skills**
- Confidence in handling **complex nanoscale CMOS circuits**
- Readiness for **VLSI, Memory Design, and Analog IC roles**

---

### Plots Included
- SRAM schematic  
- Butterfly curve  





