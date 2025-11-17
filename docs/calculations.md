# 🧮 Essential Calculations & Sizing Formulas

[← Back to Main](../README.md)

---

## 📑 Table of Contents

- [Introduction](#-introduction)
- [Maximum System Voltage (NEC Compliance)](#-maximum-system-voltage-nec-compliance)
- [PV Array Sizing](#-pv-array-sizing)
- [Battery Bank Sizing](#-battery-bank-sizing)
- [Charge Controller Sizing](#-charge-controller-sizing)
- [Inverter Sizing](#-inverter-sizing)
- [Protection & Wiring](#-protection--wiring)
- [Voltage Drop Analysis](#-voltage-drop-analysis)
- [Quick Reference Tables](#-quick-reference-tables)

---

## 📐 Introduction

Accurate calculations are **critical** for:
- ✅ **Safety**: Preventing overvoltage, overcurrent, fire hazards
- ✅ **Code compliance**: Meeting NEC requirements
- ✅ **Performance**: Ensuring system operates at design capacity
- ✅ **Longevity**: Avoiding premature component failure

> ⚠️ **Important**: All formulas use **Standard International (SI) units** unless otherwise noted. Always verify units in your calculations.

---

## ⚡ Maximum System Voltage (NEC Compliance)

**Objective**: Ensure PV string voltage doesn't exceed system limits, especially in cold weather.

### NEC Voltage Limits

| System Type | Maximum System Voltage |
|-------------|----------------------|
| **Residential (Dwelling Unit)** | 600V DC |
| **Commercial** | 1000V DC |
| **Large-Scale (per NEC 691)** | >1000V DC (special requirements) |

---

### Temperature-Corrected Voc Calculation

**Why?** Panel voltage *increases* in cold temperatures. A string that's safe at 25°C may exceed limits at -20°C!

#### Step-by-Step Procedure

**Given:**
- $V_{oc}$ = Open-circuit voltage at STC (25°C) — from panel datasheet
- $\text{TkVoc}$ = Temperature coefficient of Voc (%/°C or V/°C) — from datasheet
- $T_{min}$ = Lowest expected ambient temperature (°C) — from local climate data

---

#### Formula Table

| Step | Formula | Description |
|------|---------|-------------|
| **1. Temperature drop** | $\Delta T = 25°\text{C} - T_{min}$ | Temperature difference from STC |
| **2a. Voltage increase per °C** (if TkVoc in %) | $\Delta V_{oc/°C} = 0.01 \times \text{TkVoc} (\%) \times V_{oc}$ | Convert % to voltage |
| **2b. Voltage increase per °C** (if TkVoc in V/°C) | $\Delta V_{oc/°C} = \|\text{TkVoc}\|$ | Use absolute value |
| **3. Total voltage increase** | $\Delta V_{oc, \text{total}} = \Delta T \times \Delta V_{oc/°C}$ | Total increase from cold |
| **4. Maximum module Voc** | $V_{oc, \text{max}} = V_{oc} + \Delta V_{oc, \text{total}}$ | Cold-weather Voc |
| **5. Maximum string voltage** | $V_{\text{string, max}} = N_{\text{series}} \times V_{oc, \text{max}}$ | Total series voltage |

---

#### Example Calculation

**Panel Specifications:**
- $V_{oc}$ = 36.9V @ 25°C
- $\text{TkVoc}$ = -0.36%/°C
- $T_{min}$ = -23°C (coldest day in location)
- Series modules: 13 panels

**Step 1: Temperature drop**
$$\Delta T = 25°\text{C} - (-23°\text{C}) = 48°\text{C}$$

**Step 2: Voltage increase per °C**
$$\Delta V_{oc/°C} = 0.01 \times 0.36 \times 36.9\text{V} = 0.133\text{V/°C}$$

**Step 3: Total voltage increase**
$$\Delta V_{oc, \text{total}} = 48°\text{C} \times 0.133\text{V/°C} = 6.38\text{V}$$

**Step 4: Maximum module Voc**
$$V_{oc, \text{max}} = 36.9\text{V} + 6.38\text{V} = 43.28\text{V}$$

**Step 5: Maximum string voltage**
$$V_{\text{string, max}} = 13 \times 43.28\text{V} = 562.64\text{V}$$

**✅ Result**: 562.64V < 600V (residential limit) — **COMPLIANT**

---

### Quick Reference: String Length Limits

For **600V residential systems**, maximum series panels by module Voc:

| Module Voc @ STC | TkVoc | Tmin = -20°C | Tmin = -30°C | Tmin = -40°C |
|------------------|-------|--------------|--------------|--------------|
| **36V** | -0.36%/°C | 13 panels | 12 panels | 11 panels |
| **40V** | -0.35%/°C | 12 panels | 11 panels | 10 panels |
| **45V** | -0.30%/°C | 11 panels | 10 panels | 9 panels |
| **50V** | -0.28%/°C | 10 panels | 9 panels | 8 panels |

> 💡 **Pro Tip**: Always use local **record low temperature**, not average winter temperature. Climate data available from NOAA, weather.gov, or ASHRAE handbooks.

---

## ☀️ PV Array Sizing

**Objective**: Calculate required solar panel capacity to meet energy needs.

### Energy Requirement Formula

**Step 1: Calculate total daily energy consumption**

$$E_{\text{load}} = \sum_{i=1}^{n} (P_i \times h_i)$$

Where:
- $E_{\text{load}}$ = Total daily energy (Wh/day)
- $P_i$ = Power of device $i$ (W)
- $h_i$ = Hours of operation per day

---

**Step 2: Account for system losses (safety factor)**

$$E_{\text{needed}} = E_{\text{load}} \times 1.3$$

**Safety factor (1.3) accounts for:**
- Inverter efficiency loss (~10%)
- Wiring losses (~5%)
- Battery inefficiency (~10%)
- Dust/soiling (~5%)

---

**Step 3: Calculate required panel power**

$$P_{\text{panels}} = \frac{E_{\text{needed}}}{\text{PSH}}$$

Where:
- $P_{\text{panels}}$ = Total panel capacity (W or Wp)
- $\text{PSH}$ = Peak Sun Hours per day (hours)

---

### Peak Sun Hours (PSH)

**What is PSH?** The equivalent number of hours per day with 1000 W/m² irradiance.

**Example**:
If your location receives 5 PSH:
- It's equivalent to 5 hours of full sun (1000 W/m²)
- Actual sun may be 10 hours, but varying intensity averages to 5 PSH

**Finding PSH for your location:**
- 🌐 [NREL PVWatts Calculator](https://pvwatts.nrel.gov/)
- 🌐 [Global Solar Atlas](https://globalsolaratlas.info/)
- 📊 Local solar installers/resources

**Typical PSH by Region (USA):**

| Region | PSH (annual avg) | Best Month | Worst Month |
|--------|------------------|------------|-------------|
| **Arizona** | 6.5 | 8.0 (June) | 4.5 (Dec) |
| **California** | 5.5 | 7.5 (July) | 3.5 (Dec) |
| **Texas** | 5.0 | 6.5 (June) | 4.0 (Dec) |
| **Florida** | 5.5 | 6.5 (May) | 4.5 (Dec) |
| **New York** | 4.0 | 5.5 (June) | 2.5 (Dec) |
| **Washington** | 3.5 | 6.0 (July) | 1.5 (Dec) |

> ⚠️ **Design Rule**: For **off-grid systems**, use **worst-month PSH** to ensure year-round operation!

---

### Complete Array Sizing Example

**Scenario**: Off-grid cabin in Colorado

**Given:**
- Daily energy consumption: 4,500 Wh/day
- Location: Colorado mountains
- PSH (worst month): 3.5 hours
- Panel choice: 300W, Vmp=32V, Imp=9.4A

**Calculation:**

**Step 1: Energy needed (with safety factor)**
$$E_{\text{needed}} = 4,500 \text{ Wh} \times 1.3 = 5,850 \text{ Wh}$$

**Step 2: Required panel power**
$$P_{\text{panels}} = \frac{5,850 \text{ Wh}}{3.5 \text{ PSH}} = 1,671 \text{ W}$$

**Step 3: Number of panels**
$$N_{\text{panels}} = \frac{1,671 \text{ W}}{300 \text{ W/panel}} = 5.57 \rightarrow \mathbf{6 \text{ panels}}$$

**✅ Final array**: 6× 300W = **1,800W total** (slight oversizing is good!)

---

## 🔋 Battery Bank Sizing

**Objective**: Calculate battery capacity (Ah) for desired autonomy and DoD.

### Battery Capacity Formula

$$Ah_{\text{battery}} = \frac{E_{\text{load}} \times \text{Days of Autonomy}}{\text{DoD} \times V_{\text{system}} \times k_{\text{temp}}}$$

Where:
- $Ah_{\text{battery}}$ = Required battery capacity (Ah @ C10)
- $E_{\text{load}}$ = Daily energy consumption (Wh/day)
- $\text{Days of Autonomy}$ = Backup days without sun (typically 2-5 days)
- $\text{DoD}$ = Depth of Discharge (0.5 for lead-acid, 0.8-0.9 for lithium)
- $V_{\text{system}}$ = Battery system voltage (12V, 24V, 48V)
- $k_{\text{temp}}$ = Temperature correction coefficient (see table below)

---

### Temperature Correction Coefficients

| Average Battery Temperature | Lead-Acid $k_{\text{temp}}$ | Lithium $k_{\text{temp}}$ |
|-----------------------------|---------------------------|-------------------------|
| **25°C (77°F)** | 1.00 | 1.00 |
| **15°C (59°F)** | 0.90 | 0.95 |
| **5°C (41°F)** | 0.85 | 0.92 |
| **0°C (32°F)** | 0.80 | 0.90 |
| **-10°C (14°F)** | 0.70 | 0.85 |

---

### Battery Bank Sizing Example

**Scenario**: Residential off-grid system

**Given:**
- Daily consumption: $E_{\text{load}}$ = 5,000 Wh/day
- Autonomy: 3 days
- Battery type: Lithium LFP (DoD = 90%)
- System voltage: 48V
- Battery temperature: 15°C → $k_{\text{temp}}$ = 0.95

**Calculation:**

$$Ah_{\text{battery}} = \frac{5,000 \text{ Wh} \times 3 \text{ days}}{0.9 \times 48\text{V} \times 0.95}$$

$$Ah_{\text{battery}} = \frac{15,000}{41.04} = 365.6 \text{ Ah}$$

**Round up**: **400 Ah @ 48V**

---

### Parallel Battery Strings

If individual battery capacity < required capacity, calculate parallel strings:

$$N_{\text{parallel}} = \frac{Ah_{\text{required}}}{Ah_{\text{per battery}}}$$

**Example**:
- Required: 400 Ah
- Available battery: 200 Ah
- Parallel strings: $400 / 200 = 2$ strings

---

### Days of Autonomy Guidelines

| System Type | Recommended Autonomy |
|-------------|---------------------|
| **Grid-tie (backup only)** | 0.5-1 day |
| **Off-grid, sunny region** | 2-3 days |
| **Off-grid, variable weather** | 3-5 days |
| **Critical systems** | 5-7 days |
| **Remote telecoms** | 7-10 days |

---

## ⚙️ Charge Controller Sizing

**Objective**: Ensure MPPT controller can handle PV array voltage and current.

### Key MPPT Ratings

| Rating | Formula | Safety Factor |
|--------|---------|---------------|
| **Maximum Input Voltage** | $V_{\text{oc, max}}$ (cold weather) | Must be < controller max Voc |
| **Maximum Input Current** | $1.25 \times I_{sc} \times N_{\text{parallel}}$ | 1.25× safety factor |
| **Maximum Charge Current** | $\frac{P_{\text{panels}}}{V_{\text{battery}}}$ | Controller output rating |

---

### Charge Controller Formulas

#### 1. Maximum Charging Current (to battery)

$$I_{\text{charge, max}} = \frac{P_{\text{PV array}}}{V_{\text{battery, min}}}$$

Where:
- $P_{\text{PV array}}$ = Total panel power (W)
- $V_{\text{battery, min}}$ = Minimum battery voltage (e.g., 48V for a 48V system)

> 💡 **Note**: Use minimum battery voltage for worst-case current calculation.

---

#### 2. Maximum Input Current (from PV)

$$I_{\text{input, max}} = 1.25 \times I_{sc} \times N_{\text{parallel strings}}$$

**NEC Requirement**: 1.25× safety factor for continuous current.

---

#### 3. MPPT Clipping

If $P_{\text{PV}} > P_{\text{MPPT rated}}$, the controller will "clip" excess power.

$$\text{Clipped Power} = P_{\text{PV}} - P_{\text{MPPT rated}}$$

**Example**:
- PV array: 3,000W
- MPPT rated: 2,500W
- Clipped: 500W (wasted during peak hours)

**Mitigation**: Use multiple MPPTs or upsize controller.

---

### MPPT Sizing Example

**Given:**
- Panels: 8× 350W (Voc=45V, Isc=10A, Vmp=37V)
- Configuration: 4 series × 2 parallel
- Battery: 48V system
- Coldest temp: -15°C

**Step 1: Maximum Voc (cold weather)**

Using formula from Section 1:
- TkVoc = -0.30%/°C
- ΔT = 25 - (-15) = 40°C
- ΔVoc = 0.003 × 45V × 40 = 5.4V
- Voc,max = 45V + 5.4V = 50.4V
- String Voc = 4 × 50.4V = **201.6V**

**Step 2: Maximum input current**
$$I_{\text{input}} = 1.25 \times 10\text{A} \times 2 = 25\text{A}$$

**Step 3: Maximum charge current**
$$I_{\text{charge}} = \frac{8 \times 350\text{W}}{48\text{V}} = 58.3\text{A}$$

**Controller Selection**:
- Voltage rating: ≥ 201.6V → Use **250V** model
- Charge current: ≥ 58.3A → Use **60A** or **70A** model

**✅ Selected**: **Victron SmartSolar 250V / 70A** (or equivalent)

---

## 🔌 Inverter Sizing

**Objective**: Select inverter with adequate continuous and surge power.

### Inverter Sizing Formulas

#### 1. Continuous Power Requirement

$$P_{\text{inverter, cont}} \geq 1.25 \times \sum P_{\text{continuous loads}}$$

**NEC requirement**: 1.25× safety factor for continuous loads (operating >3 hours).

---

#### 2. Surge Power Requirement

$$P_{\text{inverter, surge}} \geq \text{max}\left( P_{\text{largest motor}} \times 3, \sum P_{\text{surge loads}} \right)$$

**Motor starting current**: Typically 3-5× rated power (use 3× for conservative estimate).

---

### Inverter Sizing Example

**Given:**
- Continuous loads: 1,800W
- Largest motor: Refrigerator compressor 800W
- Other surge loads: Well pump 1,200W (occasional)

**Calculation:**

**Continuous rating**:
$$P_{\text{cont}} = 1.25 \times 1,800\text{W} = 2,250\text{W}$$

**Surge rating**:
$$P_{\text{surge}} = \text{max}(800\text{W} \times 3, 1,200\text{W}) = 2,400\text{W}$$

**✅ Selected**: Inverter rated **2,500W continuous, 5,000W surge**

---

### Inverter Efficiency Consideration

Inverter efficiency varies with load:

| Load (% of rated) | Typical Efficiency |
|-------------------|-------------------|
| **10-20%** | 85-90% |
| **30-50%** | 90-93% |
| **50-80%** | 93-95% |
| **80-100%** | 90-93% |

**Design Tip**: Size inverter so typical loads operate at **50-80% of rating** for best efficiency.

---

## 🔒 Protection & Wiring

**Objective**: Size conductors, breakers, and fuses per NEC requirements.

### NEC 690.8(B): PV Circuit Conductor Sizing

$$I_{\text{conductor, min}} \geq 1.56 \times I_{sc}$$

**Why 1.56×?**
- 1.25× for continuous current
- 1.25× for possible irradiance >1000 W/m²
- Total: $1.25 \times 1.25 = 1.5625 \approx 1.56$

---

### Overcurrent Protection (Fuses/Breakers)

#### PV String Fuses

$$I_{\text{fuse}} \geq 1.56 \times I_{sc}$$

**Standard fuse sizes**: 10A, 15A, 20A, 25A, 30A, 35A, 40A, 50A, 60A

**Example**:
- $I_{sc}$ = 12A
- Required: $1.56 \times 12\text{A} = 18.72\text{A}$
- **Select**: 20A fuse

> ⚠️ **Fusing Rule (NEC 690.9)**:
> - **1-2 parallel strings**: Fusing optional (if conductors rated ≥ 1.56 × Isc)
> - **3+ parallel strings**: Fusing REQUIRED

---

#### Charge Controller to Battery Breaker

$$I_{\text{breaker}} = 1.25 \times I_{\text{charge controller rating}}$$

**Example**:
- Charge controller: 60A
- Breaker: $1.25 \times 60\text{A} = 75\text{A}$

---

#### Battery to Inverter Breaker (DC Side)

$$I_{\text{breaker}} = \frac{1.25 \times P_{\text{inverter, rated}}}{\eta_{\text{inverter}} \times V_{\text{battery, min}}}$$

Where:
- $\eta_{\text{inverter}}$ = Inverter efficiency (typically 0.90-0.95)
- $V_{\text{battery, min}}$ = Minimum battery voltage under load

**Example**:
- Inverter: 5000W
- Battery: 48V system (min voltage 42V under load)
- Efficiency: 0.92

$$I_{\text{breaker}} = \frac{1.25 \times 5000\text{W}}{0.92 \times 42\text{V}} = 161.7\text{A}$$

**Select**: 175A or 200A breaker

---

## 📏 Voltage Drop Analysis

**Objective**: Ensure voltage drop ≤ 2% on DC circuits, ≤ 3% total system.

### Voltage Drop Formula

$$V_{\text{drop}} = \frac{2 \times I \times L \times R}{1000}$$

Where:
- $V_{\text{drop}}$ = Voltage drop (V)
- $I$ = Current (A)
- $L$ = One-way cable length (m)
- $R$ = Resistance per km (Ω/km) @ operating temperature
- Factor of 2 accounts for positive + negative conductors

---

### Percentage Voltage Drop

$$\text{Vdrop\%} = \frac{V_{\text{drop}}}{V_{\text{nominal}}} \times 100$$

**NEC Recommendations:**
- **DC circuits**: ≤ 2%
- **Total system**: ≤ 3%

---

### Cable Resistance (Temperature Corrected)

Resistance increases with temperature:

$$R_{T2} = R_{T1} \times [1 + \alpha \times (T_2 - T_1)]$$

Where:
- $\alpha$ = Temperature coefficient of resistance (0.00393 for copper)
- $R_{T1}$ = Resistance at reference temperature $T_1$ (usually 20°C)
- $T_2$ = Operating temperature

---

### Copper Wire Resistance (@ 20°C)

| AWG | mm² | Ω/km | Max Current (60°C) |
|-----|-----|------|--------------------|
| **10 AWG** | 5.26 | 3.28 | 30A |
| **8 AWG** | 8.37 | 2.06 | 40A |
| **6 AWG** | 13.3 | 1.30 | 55A |
| **4 AWG** | 21.2 | 0.815 | 70A |
| **2 AWG** | 33.6 | 0.513 | 95A |
| **1/0 AWG** | 53.5 | 0.322 | 125A |
| **2/0 AWG** | 67.4 | 0.256 | 145A |
| **4/0 AWG** | 107 | 0.161 | 195A |

---

### Voltage Drop Example

**Scenario**: PV array to charge controller

**Given:**
- Current: 40A (PV output)
- Voltage: 150V (PV string voltage at Vmp)
- Cable length: 20m (one-way)
- Cable: 6 AWG copper (R = 1.30 Ω/km @ 20°C)
- Operating temp: 60°C

**Step 1: Temperature-corrected resistance**
$$R_{60} = 1.30 \times [1 + 0.00393 \times (60 - 20)]$$
$$R_{60} = 1.30 \times 1.157 = 1.50 \text{ Ω/km}$$

**Step 2: Voltage drop**
$$V_{\text{drop}} = \frac{2 \times 40\text{A} \times 20\text{m} \times 1.50\text{ Ω/km}}{1000}$$
$$V_{\text{drop}} = \frac{2400}{1000} = 2.4\text{V}$$

**Step 3: Percentage**
$$\text{Vdrop\%} = \frac{2.4\text{V}}{150\text{V}} \times 100 = 1.6\%$$

**✅ Result**: 1.6% < 2% — **ACCEPTABLE**

---

### Cable Sizing Quick Reference

For **2% voltage drop** on **48V DC system** (most common):

| Current | Cable Run (one-way) | Minimum AWG |
|---------|---------------------|-------------|
| **20A** | 5m | 10 AWG |
| **20A** | 10m | 8 AWG |
| **40A** | 5m | 8 AWG |
| **40A** | 10m | 4 AWG |
| **60A** | 5m | 6 AWG |
| **60A** | 10m | 2 AWG |
| **80A** | 5m | 4 AWG |
| **80A** | 10m | 1/0 AWG |

---

## 📊 Quick Reference Tables

### System Voltage Selection

| Total Load Power | Recommended System Voltage |
|------------------|---------------------------|
| **< 500W** | 12V |
| **500W - 2kW** | 24V |
| **2kW - 5kW** | 48V |
| **5kW - 10kW** | 48V or 96V |
| **> 10kW** | 96V or higher |

**Why higher voltage?**
- Lower current = smaller/cheaper cables
- Lower losses (P = I²R)
- More efficient inverters

---

### Safety Factors Summary

| Item | Safety Factor | Reason |
|------|---------------|--------|
| **PV conductor sizing** | 1.56× Isc | NEC 690.8(B) |
| **Continuous load** | 1.25× | NEC general requirement |
| **Energy calculation** | 1.3× | System losses |
| **MPPT input current** | 1.25× Isc | NEC overcurrent protection |
| **Breaker sizing (continuous)** | 1.25× | NEC 690.8(B) |

---

### Temperature Coefficient Examples

Common panel temperature coefficients:

| Panel Type | Pmax (%/°C) | Voc (%/°C) | Isc (%/°C) |
|-----------|-------------|------------|-----------|
| **Mono PERC** | -0.40 | -0.30 | +0.05 |
| **TOPCon** | -0.35 | -0.26 | +0.04 |
| **HJT** | -0.26 | -0.24 | +0.03 |

**Impact at 65°C cell temperature (ΔT = 40°C):**
- PERC: -16% power
- TOPCon: -14% power
- HJT: -10.4% power ✅ (Best!)

---

## 🎯 Key Takeaways

### ✅ Critical Formulas to Remember

1. **Max Voc (cold)**: $V_{oc,max} = V_{oc} + (\Delta T \times \text{TkVoc} \times V_{oc})$
2. **Panel sizing**: $P_{panels} = \frac{E_{load} \times 1.3}{\text{PSH}}$
3. **Battery capacity**: $Ah = \frac{E_{load} \times \text{Days}}{\text{DoD} \times V_{sys} \times k_{temp}}$
4. **MPPT charge current**: $I_{charge} = \frac{P_{panels}}{V_{battery}}$
5. **NEC conductor sizing**: $I_{conductor} \geq 1.56 \times I_{sc}$
6. **Voltage drop**: $V_{drop\%} = \frac{2 \times I \times L \times R}{1000 \times V_{nom}} \times 100$

### ✅ Design Checklist

- [ ] Verify max string voltage < 600V (residential) or 1000V (commercial)
- [ ] Use **worst-month PSH** for off-grid systems
- [ ] Apply 1.3× safety factor for energy calculations
- [ ] Size batteries for appropriate DoD (50% lead-acid, 80% lithium)
- [ ] Ensure MPPT voltage rating > cold-weather Voc
- [ ] Apply 1.56× factor for all PV conductors and overcurrent devices
- [ ] Check voltage drop ≤ 2% DC, ≤ 3% total

---

## 🔗 Related Sections

- **Previous**: [← Components (Batteries & Controllers)](components.md)
- **Next**: [Design Procedures (Step-by-Step) →](design-procedures.md)
- [Fundamentals →](fundamentals.md)
- [Advanced Topics →](advanced-topics.md)

---

<div align="center">

**[🏠 Back to Main README](../README.md)**

</div>
