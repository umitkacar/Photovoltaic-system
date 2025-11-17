# 🔬 Fundamentals of Photovoltaic Systems

[← Back to Main](../README.md)

---

## 📑 Table of Contents

- [Introduction](#-introduction)
- [Solar Cell Physics](#-solar-cell-physics)
- [Modern Panel Technologies](#-modern-panel-technologies-2025)
- [Panel Architecture & Design](#-panel-architecture--design)
- [Performance Factors](#-performance-factors)
- [Key Takeaways](#-key-takeaways)

---

## 🌞 Introduction

A **Photovoltaic (PV) system** converts solar energy directly into electrical energy through the **photovoltaic effect**. This phenomenon occurs when photons (light particles) strike a semiconductor material and free electrons, creating an electric current.

### Why PV Systems?

| Advantage ✅ | Disadvantage ❌ |
|-------------|----------------|
| ♻️ **Green energy** - Zero emissions during operation | ⚡ Limited by weather (no power at night/cloudy days) |
| 🔇 **Silent operation** - No mechanical parts | 🔋 Requires energy storage (batteries) |
| 💰 **Low O&M costs** - Minimal maintenance required | 📉 Low overall efficiency (~15-22% for standard panels) |
| 📍 **Distributed generation** - Reduces transmission losses | 💵 High initial investment cost |
| 🛡️ **Long lifespan** - 25-30 years with degradation <0.5%/year | 🌡️ Efficiency drops with high temperatures |

---

## ⚛️ Solar Cell Physics

### The Photovoltaic Effect

When sunlight hits a solar cell, three key processes occur:

```
┌─────────────────────────────────────────────────┐
│  1. ABSORPTION                                   │
│     Photon (hν) strikes semiconductor            │
│                  ↓                               │
│  2. GENERATION                                   │
│     Electron-hole pair created                   │
│                  ↓                               │
│  3. SEPARATION & COLLECTION                      │
│     Electric field separates charges → Current   │
└─────────────────────────────────────────────────┘
```

### Semiconductor Materials

#### Silicon (Si) - The Industry Standard

**Why Silicon?**
- ✅ **Abundant**: Second most abundant element in Earth's crust
- ✅ **Optimal bandgap**: 1.1 eV (ideal for solar spectrum)
- ✅ **Mature technology**: Decades of manufacturing experience
- ✅ **Stable**: Excellent long-term performance

#### Doping Process

Pure silicon is a poor conductor. **Doping** introduces impurities to create mobile charge carriers:

| Type | Dopant Element | Electrons | Result |
|------|---------------|-----------|--------|
| **N-Type** | Phosphorus (P), Arsenic (As) | 5 outer electrons | **Excess electrons** (negative charge carriers) |
| **P-Type** | Boron (B), Gallium (Ga) | 3 outer electrons | **Excess holes** (positive charge carriers) |

### The PN Junction

When N-type and P-type materials are joined:

```
       N-Type              │              P-Type
                           │
  Excess electrons ← ← ← ← │ → → → → Excess holes
         (-)               │              (+)
                           │
              ⚡ ELECTRIC FIELD FORMS ⚡
                           │
    Depletion Region (no free carriers)
```

**What happens when light hits:**

1. **Photon absorption**: Electron knocked free from silicon atom
2. **Electric field**: Pushes electron toward N-side, hole toward P-side
3. **Current flow**: Electrons flow through external circuit
4. **Voltage generation**: Each cell produces ~0.5-0.9V

> 💡 **Key Insight**: The PN junction is the "engine" of the solar cell. The built-in electric field is what separates the photon-generated charges and drives current through your load.

---

## 🚀 Modern Panel Technologies (2025)

### Technology Evolution Timeline

```
2010-2015          2016-2020          2021-2023          2024-2025
────────────────────────────────────────────────────────────────
  PERC            → TOPCon 1.0      → TOPCon 2.0      → Perovskite
 (18-20%)          (22-24%)          (24-26%)           Tandems
                                                        (30-34%+)
                     HJT              HJT + Bifacial
                   (23-25%)           (25-26%)
```

### 1️⃣ TOPCon (Tunnel Oxide Passivated Contact)

**Market Leader: 75% of Chinese manufacturing in 2025**

#### How It Works
- **Tunnel oxide layer**: Ultra-thin (1-2 nm) oxide between silicon and metal contact
- **Passivation**: Reduces electron recombination at rear surface
- **Result**: Higher voltage and efficiency

#### Performance
| Parameter | Value |
|-----------|-------|
| **Efficiency** | 24-26% (commercial), up to 28% (lab) |
| **Bifacial Factor** | Up to 90% (TOPCon 2.0) |
| **Temperature Coefficient** | -0.30%/°C (better than PERC) |
| **Degradation** | <0.45%/year |

#### Advantages
- ✅ Compatible with existing PERC production lines (easy upgrade)
- ✅ Excellent bifacial performance
- ✅ Lower cost than HJT
- ✅ Better temperature coefficient than PERC

#### Leading Manufacturers
- 🏭 **Trina Solar**: Vertex N series (up to 90% bifaciality)
- 🏭 **Jinko Solar**: N-type TOPCon at 34.22% efficiency (with perovskite tandem)
- 🏭 **Longi**: Hi-MO 6 series

---

### 2️⃣ HJT (Heterojunction Technology)

**Premium Option: 15% market share, highest efficiency**

#### How It Works
- **Hybrid structure**: Crystalline silicon (c-Si) core + thin-film amorphous silicon (a-Si) layers
- **Low-temperature processing**: <200°C (vs. 800°C for standard cells)
- **Intrinsic layers**: Passivate surface defects

#### Performance
| Parameter | Value |
|-----------|-------|
| **Efficiency** | 25-26% (commercial), up to 27% (lab) |
| **Bifacial Factor** | 92-95% |
| **Temperature Coefficient** | **-0.24%/°C** (best in class!) |
| **Degradation** | <0.25%/year (lowest degradation) |

#### Advantages
- ✅ **Best temperature performance**: Ideal for hot climates
- ✅ **Highest bifacial factor**: Captures more rear-side irradiance
- ✅ **Low degradation**: Longest effective lifespan
- ✅ **Low-light performance**: Generates power even in cloudy conditions

#### Disadvantages
- ❌ Higher manufacturing cost (requires new equipment)
- ❌ Lower market availability
- ❌ Requires indium tin oxide (ITO) - rare material

#### Leading Manufacturers
- 🏭 **Huasun Solar**: HJT-perovskite tandem reaching 800W
- 🏭 **REC**: Alpha Pure series
- 🏭 **Meyer Burger**: SmartWire HJT

---

### 3️⃣ Perovskite & Tandem Cells

**Future Technology: 34%+ efficiency in lab, commercial breakthrough in 2025**

#### What are Perovskites?
- **Crystal structure**: ABX₃ (e.g., CH₃NH₃PbI₃)
- **Flexible bandgap**: Can be tuned to absorb different wavelengths
- **Low-cost manufacturing**: Solution-processed, can be printed!

#### Tandem Architecture

```
        ☀️ Sunlight ☀️
             ↓
    ┌─────────────────┐
    │  Perovskite     │ ← Absorbs high-energy photons (blue/UV)
    │  (Top Cell)     │   Bandgap: ~1.7 eV
    └─────────────────┘
             ↓ (remaining light passes through)
    ┌─────────────────┐
    │  Silicon        │ ← Absorbs low-energy photons (red/IR)
    │  (Bottom Cell)  │   Bandgap: 1.1 eV
    └─────────────────┘
             ↓
        MAXIMUM CAPTURE
```

#### Performance (2025 Status)
| Configuration | Efficiency | Status |
|--------------|------------|--------|
| **Perovskite-Silicon (Lab)** | 34.85% | 🔬 Research record |
| **Trina Solar Module** | 30.6% | 🏭 Pre-commercial |
| **Jinko TOPCon-Perovskite** | 34.22% | 🔬 Cell-level record |
| **Huasun HJT-Perovskite** | 800W module | 🏭 Limited production |

#### Challenges (Being Solved)
- ⚠️ **Stability**: Perovskite degrades with moisture/oxygen
  - *Solution*: Encapsulation improvements, 2D/3D hybrid perovskites
- ⚠️ **Lead content**: Environmental concern
  - *Solution*: Lead-free alternatives (tin-based) under development
- ⚠️ **Scalability**: Lab-to-fab gap
  - *Solution*: Roll-to-roll printing, large-area deposition techniques

---

### 4️⃣ Bifacial Solar Panels

**Market Penetration: 60% of new installations**

#### How It Works
- **Transparent backsheet**: Allows light to hit rear surface
- **Rear-side generation**: Captures reflected/diffuse light from ground, roofs, snow
- **Bifacial Factor**: Ratio of rear power to front power (e.g., 90% means rear produces 90% of front)

#### Power Gain Scenarios

| Installation | Ground Albedo | Bifacial Gain |
|-------------|---------------|---------------|
| **Desert/Sand** | 15-25% | +5-10% |
| **Concrete/Urban** | 20-30% | +8-15% |
| **White Gravel** | 30-40% | +12-20% |
| **Fresh Snow** | 60-90% | +20-30% |

#### Best Practices
- ✅ **Higher mounting**: Increase clearance (>1m) for better rear irradiance
- ✅ **Reflective surfaces**: Use white or light-colored ground cover
- ✅ **Avoid shading**: Ensure rear side has clear view of reflective surfaces
- ✅ **East-West orientation**: For bifacial ground mounts, captures morning + evening light

---

### 5️⃣ Half-Cut Cell Modules

**Market Adoption: 80% of panels now use half-cut design**

#### How It Works
```
Traditional Cell (156mm)       Half-Cut Cell (156mm × 78mm)
┌──────────────┐              ┌───────┬───────┐
│              │              │   ⚡   │   ⚡   │
│      ⚡       │  → CUT →     ├───────┼───────┤
│              │              │   ⚡   │   ⚡   │
└──────────────┘              └───────┴───────┘
  Area: A                       Area: A/2 each
  Current: I                    Current: I/2 each
```

#### Electrical Benefits

**Power Loss Formula:**
$P_{loss} = I^2 \times R$

When current is halved:
- Traditional: $P_{loss} = I^2 \times R$
- Half-cut: $P_{loss} = (I/2)^2 \times R = I^2 \times R / 4$

**Result: 75% reduction in resistive losses!**

#### Performance Gains
| Benefit | Impact |
|---------|--------|
| **Efficiency increase** | +1.5% to 3% |
| **Lower operating temperature** | -2°C to 3°C |
| **Better shading tolerance** | Partial shading affects only half the module |
| **Reduced hotspot risk** | Lower current = less heat generation |

---

## 🏗️ Panel Architecture & Design

### Busbar Evolution

**Busbars** are the metal strips that collect and transport current from cell fingers.

```
Evolution of Busbar Design:

3BB (2015)         5BB (2018)         9BB/MBB (2022+)
┌─────────┐       ┌─────────┐        ┌─────────┐
│ ││  ││  ││      │ │ │ │ │ │       │ ││││││││││
│ ││  ││  ││      │ │ │ │ │ │       │ ││││││││││
│ ││  ││  ││      │ │ │ │ │ │       │ ││││││││││
└─────────┘       └─────────┘        └─────────┘
3 busbars         5 busbars          9+ busbars
                                     (Multi-Busbar)
```

#### Why More Busbars?

| Parameter | 3BB | 5BB | 9BB/MBB |
|-----------|-----|-----|---------|
| **Finger Distance** | Long | Medium | Short |
| **Resistive Loss** | Higher | Medium | Lowest |
| **Current Collection** | Slower | Faster | Fastest |
| **Shading Loss** | Higher | Medium | Lower |
| **Efficiency Gain** | Baseline | +2% | +3-4% |

> 💡 **Engineering Insight**: Shorter distance between busbars = lower resistance = less power loss. Think of it like adding more highways to reduce traffic congestion!

---

### Hybrid PVT (Photovoltaic-Thermal) Panels

**Problem**: Standard PV panels waste 80% of solar energy as heat, which actually *reduces* efficiency.

**Solution**: Hybrid PVT panels capture this heat for useful purposes.

#### DualSun SPRING Technology

```
        ☀️ Solar Radiation (100%)
              ↓
    ┌──────────────────────┐
    │  PV Cells (Front)    │ → 20% Electricity
    ├──────────────────────┤
    │  Heat Exchanger      │ → 60% Hot Water
    │  (Rear)              │   (up to 70°C)
    └──────────────────────┘
         ↓
    Circulating Water
    Cools cells = +5-15% electrical output
```

#### Dual Benefits

| Benefit | Description | Impact |
|---------|-------------|--------|
| **Dual Heat** | Hot water production | Up to 70°C water temperature |
| **Dual Boost** | Active cooling of PV cells | +5-15% electrical output |
| **Combined Efficiency** | Total solar energy capture | Up to 80% (vs. 20% PV-only) |

#### Applications
- 🏠 **Residential**: Domestic hot water + electricity
- 🏊 **Commercial**: Pool heating + power
- 🏭 **Industrial**: Process heat + electricity
- 🌡️ **District heating**: Combined heat and power (CHP)

---

## 📊 Performance Factors

### 1. Temperature Effects

**Critical Fact**: PV cell efficiency *decreases* with temperature.

#### Temperature Coefficients

| Technology | Pmax Coefficient | Voc Coefficient | Isc Coefficient |
|-----------|------------------|-----------------|-----------------|
| **Standard Si** | -0.40 to -0.45%/°C | -0.30%/°C | +0.05%/°C |
| **TOPCon** | -0.30 to -0.35%/°C | -0.25%/°C | +0.04%/°C |
| **HJT** | **-0.24 to -0.26%/°C** | -0.22%/°C | +0.03%/°C |

#### Example Calculation

**Panel**: 400W @ 25°C, Temperature coefficient = -0.35%/°C
**Operating temperature**: 65°C (hot summer day)

```
ΔT = 65°C - 25°C = 40°C
Power loss = 400W × 0.35% × 40 = 56W
Actual output = 400W - 56W = 344W (14% loss!)
```

**Mitigation Strategies:**
- ✅ Use HJT panels in hot climates (better temperature coefficient)
- ✅ Ensure adequate ventilation (avoid flush roof mounts)
- ✅ Light-colored mounting structures
- ✅ PVT cooling systems

---

### 2. Solar Irradiance

**Standard Test Conditions (STC):**
- Irradiance: 1000 W/m²
- Cell temperature: 25°C
- Air mass: 1.5

**Real-World Conditions:**
- Irradiance varies: 200-1100 W/m²
- Temperature varies: -20°C to +80°C
- Air mass changes with sun angle

#### Performance at Different Irradiances

| Irradiance | Condition | Relative Output |
|------------|-----------|-----------------|
| 1000 W/m² | Full sun | 100% |
| 800 W/m² | Hazy sun | ~78% |
| 500 W/m² | Cloudy | ~45% |
| 200 W/m² | Heavy overcast | ~15% |

---

### 3. Degradation

All PV panels degrade over time, but rates vary by technology:

| Technology | Year 1 | Years 2-25 | Total @ 25 Years |
|-----------|--------|------------|------------------|
| **Standard PERC** | -2.5% | -0.55%/year | ~15-17% |
| **TOPCon** | -2.0% | -0.45%/year | ~12-13% |
| **HJT** | -1.0% | -0.25%/year | ~6-7% |

**Example**: 400W HJT panel after 25 years
Remaining power = 400W × (1 - 0.07) = **372W** (93% retention)

---

## 🎯 Key Takeaways

### ✅ Essential Concepts

1. **PN Junction is the heart**: Electric field separates photon-generated charges
2. **N-Type dominance**: TOPCon and HJT are taking over from P-Type PERC
3. **Tandem cells are coming**: 30%+ efficiency commercially available in 2025
4. **Bifacial is standard**: 60% of new installations use bifacial modules
5. **Temperature matters**: Can lose 10-15% power on hot days
6. **More busbars = better**: 5BB minimum, 9BB/MBB optimal

### 🎓 Technology Selection Guide

| Use Case | Recommended Technology | Why? |
|----------|----------------------|------|
| **Hot climate** | HJT or TOPCon | Best temperature coefficients |
| **Reflective environment** | Bifacial TOPCon/HJT | Maximize rear-side gain |
| **Budget-conscious** | TOPCon (5BB or 9BB) | Best cost/performance ratio |
| **Premium/maximum power** | HJT or Perovskite-Tandem | Highest efficiency available |
| **Space-constrained** | HJT or High-efficiency TOPCon | Maximum W/m² |
| **Combined heat & power** | PVT Hybrid | Dual energy capture |

---

## 🔗 Related Sections

- **Next**: [Components (Batteries & Controllers) →](components.md)
- [System Calculations →](calculations.md)
- [Design Procedures →](design-procedures.md)
- [Advanced Topics (2025 Tech) →](advanced-topics.md)

---

<div align="center">

**[🏠 Back to Main README](../README.md)**

</div>
