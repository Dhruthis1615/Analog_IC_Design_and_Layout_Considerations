# Day 2 – Common Source Amplifier Gain Analysis and Differential Amplifier Design

## Overview
Day 2 focused on studying the gain behavior of a common source NMOS amplifier with different load configurations and on designing a basic differential amplifier using Cadence Virtuoso. The objective was to understand how load implementation and biasing affect gain and overall circuit performance.

---

## Common Source Amplifier Gain Analysis

A common source NMOS amplifier was analyzed using three different load configurations to compare gain behavior and identify limitations of each approach.

### 1. NMOS with Resistor Load
In this configuration, an NMOS common source amplifier with a resistive load was analyzed. The gain was measured by varying the resistor value. This study demonstrated that although gain increases with higher resistance, passive resistive loads limit achievable gain and are not area-efficient for IC design.

---

### 2. NMOS with PMOS Source–Drain Shorted Load
The resistive load was replaced with a PMOS whose source and drain were shorted. This configuration introduced an active device as the load; however, due to the low output resistance of the source–drain shorted PMOS, the gain was not as expected. This highlighted that simply replacing a resistor with a MOS device does not guarantee gain improvement.

---

### 3. NMOS with PMOS Active Load
The source–drain shorted PMOS was replaced with a properly biased PMOS active load using a separate power supply. This configuration provided a much higher output resistance, resulting in improved gain (approximately unity). DC, AC, and transient analyses were performed to verify correct biasing, gain behavior, and time-domain response.

---

## Differential Amplifier Design

A differential amplifier was designed and verified as a fundamental analog building block. The following steps were carried out:
- Schematic creation  
- Symbol generation  
- Testbench setup  
- Simulation and output verification  

This exercise helped in understanding differential operation, biasing requirements, and the importance of symmetry and matching in analog IC design.

---

## Analyses Performed
- DC analysis to verify operating points and regions of operation  
- AC analysis to evaluate small-signal gain  
- Transient analysis to observe time-domain behavior  

---

## Files Included
- `common_source_amplifier_gain_analysis/`  
  Contains Cadence Virtuoso design files for the common source NMOS amplifier with different load configurations, along with DC, AC, and transient simulation results and corresponding waveform images.

- `differential_amplifier/`  
  Includes Cadence schematic, symbol, testbench, simulation files, and output waveform images for the differential amplifier design and verification.
