<div align="center">

# ⚡ Professional Photovoltaic System Design Guide

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Documentation](https://img.shields.io/badge/docs-latest-brightgreen.svg)](docs/)
[![NEC 2023](https://img.shields.io/badge/NEC-2023%20Compliant-orange.svg)](docs/design-procedures.md)
[![Technology](https://img.shields.io/badge/Tech-TOPCon%20%7C%20HJT%20%7C%20MPPT-blue.svg)](docs/advanced-topics.md)

*A comprehensive, industrial-grade resource for designing modern solar PV systems with advanced calculations, NEC compliance, and cutting-edge technologies.*

[📚 Documentation](docs/) | [🧮 Calculations](docs/calculations.md) | [🔧 Design Tools](docs/design-procedures.md) | [🚀 Advanced Topics](docs/advanced-topics.md)

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Quick Start](#-quick-start)
- [Documentation Structure](#-documentation-structure)
- [Key Features](#-key-features)
- [Technologies Covered](#-technologies-covered)
- [Standards & Compliance](#-standards--compliance)
- [Contributing](#-contributing)
- [References](#-references)

---

## 🌟 Overview

This repository provides a **detailed, professional-grade tutorial** for designing modern **Photovoltaic (PV) systems**. Whether you're an electrical engineer, solar installer, system integrator, or researcher, you'll find:

- ✅ **Fundamental theory** of solar cell operation (PN junctions, doping, photovoltaic effect)
- ✅ **Component deep-dives** (panels, batteries, charge controllers, inverters)
- ✅ **Mathematical formulas** for system sizing and NEC code compliance
- ✅ **Practical design procedures** with real-world examples
- ✅ **Latest technologies** (TOPCon, HJT, Perovskite, MPPT algorithms, IoT/AI integration)

> 💡 **Designed for:** Industrial applications, commercial installations, off-grid systems, and grid-tied solutions

---

## 🚀 Quick Start

### Prerequisites
- Basic understanding of electrical circuits (voltage, current, power)
- Familiarity with DC/AC power systems
- Access to solar radiation data for your location (Peak Sun Hours)

### Design Workflow
```mermaid
graph LR
    A[📊 Load Analysis] --> B[🔋 Battery Sizing]
    B --> C[☀️ Panel Sizing]
    C --> D[⚙️ MPPT Selection]
    D --> E[🔌 Inverter Sizing]
    E --> F[📐 NEC Compliance]
    F --> G[✅ Installation]
```

**Start here:** [Design Procedures →](docs/design-procedures.md)

---

## 📂 Documentation Structure

### Core Modules

<table>
<tr>
<td width="33%" valign="top">

### 🔬 [Fundamentals](docs/fundamentals.md)
Learn the physics and engineering behind PV systems
- **Solar Cell Physics**
  - PN Junction theory
  - Photovoltaic effect
  - Doping processes
- **Modern Panel Technologies**
  - TOPCon (24-26% efficiency)
  - HJT (26%+ efficiency)
  - Perovskite Tandems (34%+)
  - Bifacial modules (90%+ gain)
- **Panel Architecture**
  - Multi-busbar designs (3BB → 5BB → MBB)
  - Half-cut cell modules
  - PVT hybrid systems

</td>
<td width="33%" valign="top">

### ⚙️ [Components](docs/components.md)
Deep dive into system components and selection criteria
- **Energy Storage**
  - Lead-acid (Flooded, AGM, Gel)
  - Lead-carbon (3500 cycles)
  - Lithium-ion (10,000+ cycles)
  - Flow batteries (100% DoD)
- **Charge Controllers**
  - PWM vs MPPT comparison
  - Advanced MPPT algorithms
  - Efficiency analysis (94-98%)
- **Inverters & Power Electronics**
  - String inverters
  - Micro-inverters
  - Power optimizers

</td>
<td width="33%" valign="top">

### 🧮 [Calculations](docs/calculations.md)
Essential formulas and sizing methods
- **System Voltage Calculations**
  - Temperature compensation
  - Maximum Voc calculations
  - NEC 690 compliance
- **Sizing Formulas**
  - Panel array sizing
  - Battery capacity (Ah)
  - MPPT current ratings
- **Protection Sizing**
  - Cable sizing (1.56 × Isc)
  - Breaker ratings
  - Voltage drop analysis
  - Fusing requirements

</td>
</tr>
</table>

### Additional Resources

| Document | Description | Key Topics |
|----------|-------------|------------|
| 🛠️ [**Design Procedures**](docs/design-procedures.md) | Step-by-step design methodology | Off-grid design, Grid-tied systems, Hybrid installations |
| 🚀 [**Advanced Topics**](docs/advanced-topics.md) | Cutting-edge technologies & trends | AI optimization, IoT monitoring, Smart inverters, NEC 2023 updates |

### 🏗️ Professional Implementation Guides

| Document | Description | Key Topics |
|----------|-------------|------------|
| 📐 [**Project Sizing**](docs/project-sizing.md) | Size systems by space, budget & time | Residential/Commercial/Industrial sizing, Budget tiers, Timeline planning |
| 💰 [**Cost Analysis**](docs/cost-analysis.md) | Detailed financial analysis & ROI | Component costs, Labor rates, Payback periods, Incentives (2025) |
| 🔧 [**Installation Guide**](docs/installation-guide.md) | Step-by-step installation procedures | OSHA safety, Man-hour estimates, Tool checklists, Quality control |
| 📦 [**Material Lists & BOMs**](docs/material-lists.md) | Bill of Materials templates | Complete BOMs for 3-100kW systems, Supplier guide, Procurement tips |
| 📊 [**Detailed Case Studies**](docs/detailed-case-studies.md) | Real-world project examples | Off-grid cabin, Commercial warehouse, Industrial+storage with full financials |

---

## 🎯 Key Features

### 🔢 Comprehensive Calculations
- **Maximum system voltage** with temperature compensation
- **Battery bank sizing** with DoD and autonomy considerations
- **MPPT charge controller** current and voltage ratings
- **NEC-compliant** cable and breaker sizing (1.56 × Isc rule)
- **Voltage drop analysis** for DC and AC circuits

### 🏭 Industrial Standards
- ⚡ **NEC 2023** Article 690 compliance
- 🌡️ **Temperature derating** for panels and cables
- 🔒 **Safety factors** (1.25× for continuous loads, 1.56× for overcurrent protection)
- 📊 **C10-rated** battery capacity calculations

### 🌐 Modern Technologies
- 🔬 **N-Type cells** (TOPCon, HJT) dominating 2025 market
- 🤖 **AI-driven MPPT** achieving 30% yield improvements
- 📡 **IoT monitoring** for predictive maintenance
- ⚡ **800W+ modules** with perovskite-silicon tandems

---

## 🔧 Technologies Covered

### Panel Technologies (2025)

```
┌─────────────────────────────────────────────────────┐
│  Technology  │ Efficiency │  Market Share │  Status │
├──────────────┼────────────┼───────────────┼─────────┤
│  TOPCon      │  24-26%    │     75%       │  ⭐⭐⭐  │
│  HJT         │  25-26%    │     15%       │  ⭐⭐⭐  │
│  Perovskite  │  34%+      │     <1%       │  🔬 Lab │
│  Bifacial    │  +10-30%   │     60%       │  ⭐⭐⭐  │
│  Half-Cut    │  +1.5-3%   │     80%       │  ⭐⭐⭐  │
└─────────────────────────────────────────────────────┘
```

### Battery Technologies

| Type | Cycles @ 50% DoD | Lifespan | Efficiency | Best For |
|------|------------------|----------|------------|----------|
| **Flooded Lead-Acid** | 1,500 | 5-7 years | 80-85% | Budget systems |
| **Lead-Carbon** | 3,500 | 8-12 years | 85-90% | Off-grid industrial |
| **Lithium-Ion** | 10,000+ | 10-15 years | 95-98% | Premium residential/commercial |
| **Flow Batteries** | 20,000+ | 25-30 years | 70-85% | Grid-scale storage |

### Charge Controller Comparison

| Feature | PWM | MPPT |
|---------|-----|------|
| **Efficiency** | 70-80% | 94-98% |
| **Voltage Matching** | Pulls panel down to battery V | Converts optimally |
| **Power Gain** | Baseline | +10-30% |
| **Cost** | $ | $$$ |
| **Best Application** | Small systems (<500W) | All systems >500W |

---

## 📜 Standards & Compliance

### NEC 2023 Updates for Solar

- ✅ **Article 690**: PV Systems - Major revisions to rapid shutdown
- ✅ **Article 691**: Large-Scale PV Systems (>1000V)
- ✅ **Article 705**: Interconnected Electric Power Production Sources
- ✅ **Section 690.12**: Rapid shutdown requirements clarified
- ✅ **Section 690.31(G)**: New high-voltage (>1000V) installation rules

**Key Calculation Requirements:**
- Conductor sizing: **≥ 1.56 × Isc** (NEC 690.8(B))
- Maximum voltage: **Temperature-corrected Voc** (NEC 690.7)
- Voltage drop: **≤ 2% DC, ≤ 3% total** (NEC 210.19(A))

---

## 🎓 Learning Path

### Beginner
1. Start with [Fundamentals](docs/fundamentals.md) → Understand solar cell physics
2. Read [Components](docs/components.md) → Learn about batteries and controllers
3. Study [Calculations](docs/calculations.md) → Master sizing formulas

### Intermediate
4. Follow [Design Procedures](docs/design-procedures.md) → Design your first off-grid system
5. Review NEC requirements in [Advanced Topics](docs/advanced-topics.md)

### Advanced
6. Explore [Advanced Topics](docs/advanced-topics.md) → TOPCon, HJT, AI/IoT integration
7. Design complex systems with hybrid storage and grid-tie

---

## 🔄 System Design Checklist

- [ ] **Load Analysis**: Calculate daily Wh consumption
- [ ] **Location Data**: Obtain Peak Sun Hours (PSH) for your site
- [ ] **Battery Selection**: Choose chemistry (Lead-acid vs Li-ion vs Flow)
- [ ] **System Voltage**: Select 12V, 24V, 48V, or 96V based on load
- [ ] **Panel Sizing**: Calculate total Wp needed with 1.3× safety factor
- [ ] **MPPT Sizing**: Ensure Icharge ≤ controller rating
- [ ] **String Configuration**: Verify Voc,max < controller/inverter max voltage
- [ ] **Cable Sizing**: Use NEC tables with 1.56× Isc derating
- [ ] **Breaker/Fuse Sizing**: Apply 1.25× continuous current rule
- [ ] **Voltage Drop**: Verify ≤ 2% on DC side, ≤ 3% total
- [ ] **Grounding**: Follow NEC 690.43 (now moved to Article 250)
- [ ] **Rapid Shutdown**: Comply with NEC 690.12

---

## 💡 Example Projects

### Off-Grid Cabin (3kW)
- **Load**: 5,000 Wh/day
- **Panels**: 16× 250W (4kW array)
- **Batteries**: 48V, 400Ah lithium-ion
- **MPPT**: 60A, 150V
- **Inverter**: 3000W pure sine wave

### Commercial Grid-Tied (50kW)
- **Panels**: 125× 400W TOPCon bifacial
- **Inverters**: 3× 17kW string inverters with MPPT
- **Monitoring**: IoT-enabled with AI predictive maintenance
- **Compliance**: NEC 2023 Article 690, rapid shutdown

---

## 🤝 Contributing

Contributions are welcome! Please:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-calculation`)
3. Commit your changes (`git commit -m 'Add new MPPT sizing formula'`)
4. Push to the branch (`git push origin feature/new-calculation`)
5. Open a Pull Request

---

## 📚 References

### Standards & Codes
- **NEC 2023**: NFPA 70, National Electrical Code
- **IEC 61730**: PV Module Safety Qualification
- **UL 1741**: Inverters, Converters, Controllers and Interconnection System Equipment

### Research & Data Sources
- PV Tech Magazine (2025 SNEC Conference)
- IEEE Transactions on Power Electronics
- Solar Energy International (SEI)
- National Renewable Energy Laboratory (NREL)

### Manufacturers & Tech Leaders
- Trina Solar, Jinko Solar, Huasun Solar (TOPCon/HJT leaders)
- Victron Energy, Morningstar (Charge controllers)
- Tesla, BYD, CATL (Energy storage)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

<div align="center">

### ⭐ If this guide helps your PV design, please star this repository!

**Made with ⚡ for the renewable energy community**

[🔝 Back to Top](#-professional-photovoltaic-system-design-guide)

</div>
