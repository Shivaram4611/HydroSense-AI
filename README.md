# HydroSense AI — Web Simulation & Digital Twin Platform

[![Web Platform](https://img.shields.io/badge/Platform-Web%20%7C%20Single%20Page%20App-0ea5e9.svg)](#)
[![UN SDG 6](https://img.shields.io/badge/UN%20SDG-6%20Clean%20Water-0284c7.svg)](https://sdgs.un.org/goals/goal6)
[![UN SDG 3](https://img.shields.io/badge/UN%20SDG-3%20Good%20Health-16a34a.svg)](https://sdgs.un.org/goals/goal3)
[![License: MIT](https://img.shields.io/badge/License-MIT-amber.svg)](https://opensource.org/licenses/MIT)

Interactive browser-based digital twin and telemetry dashboard for **HydroSense AI** — a smart water security network designed to detect contamination in real time and predict structural pipe failure.

---

## 🌐 Overview

The frontend interface (`index.html`) operates as a zero-dependency, self-contained single-page application (SPA). It simulates an edge-to-cloud environmental monitoring station, providing utilities, evaluators, and public health officials with immediate visibility into live pipeline telemetry, anomaly detection outputs, and automated fail-safe responses.

### Key Capabilities
- **Live Digital Twin & Pipeline Flow Map:** Real-time animated pipeline visualization with interactive solenoid shutoff valves.
- **Dynamic Node Switching:** Toggle between **Municipal Metro (Node A)**, **Rural Outpost (Node B)**, and **Industrial Facility (Node C)**.
- **Interactive Event Injectors:** Simulate hazardous chemical contamination spikes or sudden pressure bursts to observe automated valve isolation and real-time alert logs.
- **Streaming Telemetry Graphing:** Live Chart.js visualization plotting pH and Turbidity (NTU) in a rolling observation window.
- **Interactive Predictive ML Sandbox:** Adjust pipe service age, water hammer pressure variance, and contaminant levels to calculate real-time Pipe Stress Indices (PSI) and failure probabilities[cite: 1].
- **SDG 6 Community ROI Calculator:** Dynamic sliders estimating prevented waterborne illnesses, healthcare cost savings, and preserved clean water volume[cite: 1, 4].
- **Verifiable Audit Generation:** One-click generation of formatted, printable water safety audit certificates for regulatory compliance[cite: 1].
- **Embedded Project Documentation:** Full 9-block Lean Canvas and concept note viewer built directly into the UI for project submission reviewers.

---

## 🖥️ Live Telemetry Parameters

The dashboard continuously simulates and analyzes the following primary indicators[cite: 1]:

| Indicator | Nominal Range | Sensor Type | Threshold Breach Consequence[cite: 1] |
| :--- | :--- | :--- | :--- |
| **pH** | 6.5 – 8.5 pH | Industrial Glass Probe | Chemical/acidic runoff warning; flag potential corrosion[cite: 1] |
| **Turbidity** | 0.5 – 3.0 NTU | Optical Nephelometric Sensor | Silt intrusion / particulate spike; high pathogen risk indicator[cite: 1] |
| **Heavy Metals** | 0.001 – 0.010 ppm | Electrochemical Array | Industrial effluent alert; triggers emergency valve isolation[cite: 1] |
| **Bacterial Proxy** | 0 – 3 CFU/100 mL | Fluorometric / Enzymatic Sensor | Pathogen outbreak alarm; instant alert dispatch[cite: 1] |
| **Line Pressure** | 40 – 65 PSI | Piezoresistive Transducer | Pipe burst / water hammer event; triggers degradation scoring[cite: 1] |

---

## 📁 File Structure

```text
hydrosense-web/
├── index.html          # Complete standalone web application (UI, CSS, JS, Chart.js)
├── README.md           # Documentation for the web platform
