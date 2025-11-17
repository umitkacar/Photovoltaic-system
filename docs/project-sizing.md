# 📐 Project Sizing & Planning Guide

[← Back to Main](../README.md)

---

## 📑 Table of Contents

- [Introduction](#-introduction)
- [Sizing by Location Type](#-sizing-by-location-type)
- [Sizing by Budget](#-sizing-by-budget)
- [Sizing by Time Constraints](#-sizing-by-time-constraints)
- [Space Requirements](#-space-requirements)
- [Load-Based Sizing](#-load-based-sizing)
- [System Configuration Matrix](#-system-configuration-matrix)
- [Quick Sizing Tools](#-quick-sizing-tools)

---

## 🎯 Introduction

Professional PV system sizing requires balancing **four critical constraints**:
1. **Physical space** (roof area, ground area)
2. **Budget** (upfront capital, financing options)
3. **Time** (installation timeline, grid connection)
4. **Energy demand** (loads, consumption patterns)

This guide provides **decision matrices** and **sizing calculators** for different project types.

---

## 🏢 Sizing by Location Type

### Residential Systems

#### Small Residential (1-3 kW)

**Typical Application**: Apartments, condos, small homes

| Parameter | Specification |
|-----------|--------------|
| **Panel count** | 3-10 panels |
| **Roof area required** | 25-80 sq ft (2.3-7.4 m²) |
| **System voltage** | 12V or 24V |
| **Average cost** | $3,000-$9,000 |
| **Installation time** | 1-2 days |
| **Daily generation** | 4-12 kWh |
| **Best for** | Essential loads, backup power |

**Load Examples**:
- LED lighting (500W total)
- Laptop + phone charging (150W)
- Small refrigerator (150W continuous)
- Entertainment system (200W)

---

#### Medium Residential (4-8 kW)

**Typical Application**: Average homes (1,500-2,500 sq ft)

| Parameter | Specification |
|-----------|--------------|
| **Panel count** | 12-24 panels (330-400W each) |
| **Roof area required** | 250-500 sq ft (23-46 m²) |
| **System voltage** | 48V |
| **Average cost** | $12,000-$24,000 (before incentives) |
| **Cost per watt** | $2.50-3.00/W |
| **Installation time** | 2-4 days |
| **Daily generation** | 16-40 kWh |
| **Annual production** | 5,800-14,600 kWh |
| **Crew size** | 2-3 installers |

**Load Examples**:
- Full home electrical (HVAC, appliances, lighting)
- Electric vehicle charging (Level 2)
- Pool pump (if applicable)
- Home office equipment

**Space Calculation**:
```
Panel dimensions: 65" × 39" = 17.6 sq ft per panel
Number of panels: 20
Total panel area: 20 × 17.6 = 352 sq ft
Add 30% for spacing: 352 × 1.3 = 457 sq ft required
```

---

#### Large Residential (9-15 kW)

**Typical Application**: Large homes, heavy loads, EV charging

| Parameter | Specification |
|-----------|--------------|
| **Panel count** | 25-45 panels (400W each) |
| **Roof area required** | 520-900 sq ft (48-84 m²) |
| **System voltage** | 48V or 96V |
| **Average cost** | $27,000-$45,000 |
| **Cost per watt** | $2.40-2.80/W (economies of scale) |
| **Installation time** | 4-6 days |
| **Daily generation** | 45-75 kWh |
| **Annual production** | 16,400-27,400 kWh |
| **Crew size** | 3-4 installers |

**Load Examples**:
- Large home (3,000+ sq ft)
- Multiple EV charging stations
- Home workshop (power tools)
- Large HVAC systems
- Pool + spa heating

---

### Commercial Systems

#### Small Commercial (20-50 kW)

**Typical Application**: Small offices, retail stores, restaurants

| Parameter | Specification |
|-----------|--------------|
| **Panel count** | 50-150 panels |
| **Roof/ground area** | 1,000-3,000 sq ft (93-279 m²) |
| **System voltage** | 600V DC string |
| **Average cost** | $40,000-$100,000 |
| **Cost per watt** | $2.00-2.50/W |
| **Installation time** | 1-2 weeks |
| **Daily generation** | 100-250 kWh |
| **Annual production** | 36,500-91,250 kWh |
| **Crew size** | 4-6 installers |
| **Payback period** | 5-8 years |

**Demand Charge Savings**: Commercial systems benefit from **peak demand reduction**
- Typical demand charge: $10-20/kW/month
- 50 kW system reduces peak by 35-40 kW (during sun hours)
- Savings: $350-800/month from demand charges alone

---

#### Medium Commercial (100-500 kW)

**Typical Application**: Warehouses, schools, medium manufacturing

| Parameter | Specification |
|-----------|--------------|
| **Panel count** | 250-1,250 panels |
| **Roof/ground area** | 5,000-25,000 sq ft (465-2,323 m²) |
| **System voltage** | 1000V DC |
| **Average cost** | $200,000-$1,000,000 |
| **Cost per watt** | $1.80-2.30/W |
| **Installation time** | 3-8 weeks |
| **Daily generation** | 500-2,500 kWh |
| **Annual production** | 182,500-912,500 kWh |
| **Crew size** | 6-10 installers |
| **Payback period** | 4-7 years |

**Design Considerations**:
- **Structural engineering**: Required for large roof loads
- **Three-phase inverters**: 50-100 kW central inverters
- **Monitoring**: Real-time production and demand monitoring
- **Utility interconnection**: Application process 2-6 months

---

#### Large Commercial / Utility-Scale (1-50 MW)

**Typical Application**: Solar farms, industrial facilities, utilities

| Parameter | Specification |
|-----------|--------------|
| **Panel count** | 2,500-125,000+ panels |
| **Ground area** | 5-250 acres |
| **System voltage** | 1000-1500V DC |
| **Average cost** | $2M-$100M |
| **Cost per watt** | $1.20-1.80/W |
| **Installation time** | 3-18 months |
| **Daily generation** | 5,000-250,000 kWh |
| **Annual production** | 1.8-91 GWh |
| **Crew size** | 20-100+ workers |
| **Payback period** | 3-6 years |

**Special Requirements**:
- **Environmental Impact Study** (EIS)
- **Interconnection study** with utility
- **Transmission upgrades** (if needed)
- **Land acquisition** or lease agreements
- **Power Purchase Agreement** (PPA) with utility

---

### Industrial & Specialized

#### Agricultural / Agrivoltaics

**Concept**: Elevated solar panels over crops/pasture

| Parameter | Specification |
|-----------|--------------|
| **Typical size** | 500 kW - 5 MW |
| **Panel mounting height** | 3-5 meters above ground |
| **Row spacing** | 10-15 meters (for equipment passage) |
| **Land use efficiency** | 150-200% (dual use: solar + crops) |
| **Cost premium** | +15-25% vs. standard ground mount |
| **Best crops** | Leafy greens, berries, pasture |

**Economic Benefits**:
- Electricity revenue: $50,000-500,000/year
- Crop revenue: Maintained or increased (shade reduces water needs)
- Total land value: 2-3× traditional farming

---

#### Floating Solar (Floatovoltaics)

**Application**: Reservoirs, ponds, wastewater treatment

| Parameter | Specification |
|-----------|--------------|
| **Typical size** | 1-150 MW |
| **Water coverage** | 10-40% (prevent excessive shading) |
| **Mounting system** | HDPE floating platforms |
| **Cost** | $2.50-3.50/W (higher than ground) |
| **Efficiency gain** | +5-10% (water cooling) |
| **Water evaporation reduction** | 50-70% |

**Challenges**:
- Corrosion-resistant components (marine-grade)
- Anchoring system (handles water level changes)
- Maintenance access (requires boats)

---

## 💰 Sizing by Budget

### Budget Category Matrix

<table>
<tr>
<th>Budget Tier</th>
<th>System Size</th>
<th>Components</th>
<th>$/Watt</th>
<th>Total Cost</th>
<th>Expected Lifespan</th>
</tr>

<tr>
<td><strong>Economy</strong><br>$5,000-10,000</td>
<td>2-4 kW</td>
<td>
- Standard mono PERC panels<br>
- PWM or entry MPPT<br>
- Modified sine inverter<br>
- Flooded lead-acid batteries
</td>
<td>$2.50-3.00</td>
<td>$5,000-12,000</td>
<td>5-10 years</td>
</tr>

<tr>
<td><strong>Standard</strong><br>$15,000-30,000</td>
<td>5-10 kW</td>
<td>
- TOPCon or PERC panels<br>
- Quality MPPT (Victron, Morningstar)<br>
- Pure sine wave inverter<br>
- AGM or lead-carbon batteries
</td>
<td>$2.20-2.70</td>
<td>$15,000-27,000</td>
<td>10-15 years</td>
</tr>

<tr>
<td><strong>Premium</strong><br>$40,000-80,000</td>
<td>12-20 kW</td>
<td>
- HJT or TOPCon bifacial panels<br>
- Top-tier MPPT with monitoring<br>
- Hybrid grid-tie inverter<br>
- Lithium LFP batteries
</td>
<td>$2.00-2.50</td>
<td>$40,000-50,000</td>
<td>15-25 years</td>
</tr>

<tr>
<td><strong>Luxury</strong><br>$100,000+</td>
<td>25+ kW</td>
<td>
- Perovskite tandems or HJT<br>
- AI-enabled smart inverters<br>
- Flow batteries or large lithium<br>
- Full home automation integration
</td>
<td>$1.80-2.30</td>
<td>$100,000-200,000</td>
<td>25-30 years</td>
</tr>
</table>

---

### Budget Optimization Strategies

#### Strategy 1: Phased Installation

**Phase 1** (Year 1): $15,000
- Install panels + grid-tie inverter (no batteries)
- Immediate utility bill savings
- Net metering captures excess

**Phase 2** (Year 3-5): +$10,000
- Add battery storage
- Enable backup power
- Increase self-consumption to 80%+

**Total**: $25,000 over 5 years (easier to finance)

---

#### Strategy 2: DIY Labor (Off-Grid Only)

**Professional Install**: $20,000 total
- Equipment: $14,000 (70%)
- Labor: $6,000 (30%)

**DIY Install**: $15,000 total
- Equipment: $14,000
- Permit/inspection: $500
- Tool rental: $500
- **Savings**: $5,000

**Caution**: Grid-tied systems usually require licensed electrician for interconnection approval.

---

#### Strategy 3: Lease vs. Buy

| Option | Upfront Cost | Monthly Cost | 20-Year Total | Ownership |
|--------|--------------|--------------|---------------|-----------|
| **Cash purchase** | $25,000 | $0 | $25,000 | You own |
| **Loan (7%, 15 yr)** | $0 | $225 | $40,500 | You own |
| **Lease** | $0 | $150-200 | $36,000-48,000 | Leasing company |
| **PPA** | $0 | $0.12-0.15/kWh | Varies | PPA company |

**Recommendation**: Cash or loan (if you own property). Leases lose 30% tax credit benefit.

---

## ⏱️ Sizing by Time Constraints

### Installation Timeline Estimator

#### Residential (5 kW System)

| Phase | Duration | Cumulative |
|-------|----------|------------|
| **1. Site assessment & design** | 1-2 weeks | 2 weeks |
| **2. Permitting** | 2-8 weeks | 10 weeks |
| **3. Equipment procurement** | 2-4 weeks | 14 weeks |
| **4. Installation** | 2-3 days | 14 weeks |
| **5. Inspection** | 1-2 weeks | 16 weeks |
| **6. Utility interconnection** | 2-8 weeks | 24 weeks |
| **TOTAL** | — | **16-24 weeks** |

**Fast-Track Options**:
- Pre-approved system designs (cuts permitting to 1-2 weeks)
- Expedited inspection (available in some jurisdictions)
- Battery-only system (no interconnection approval needed)

---

#### Commercial (100 kW System)

| Phase | Duration | Cumulative |
|-------|----------|------------|
| **1. Feasibility study** | 2-4 weeks | 4 weeks |
| **2. Structural engineering** | 2-4 weeks | 8 weeks |
| **3. Design & engineering** | 4-6 weeks | 14 weeks |
| **4. Permitting** | 4-12 weeks | 26 weeks |
| **5. Utility interconnection study** | 8-16 weeks | 42 weeks |
| **6. Equipment procurement** | 4-8 weeks | 50 weeks |
| **7. Installation** | 3-6 weeks | 56 weeks |
| **8. Commissioning & testing** | 1-2 weeks | 58 weeks |
| **9. Final inspection & PTO** | 2-4 weeks | 62 weeks |
| **TOTAL** | — | **52-62 weeks (1+ year)** |

---

#### Utility-Scale (10 MW)

| Phase | Duration |
|-------|----------|
| **Development & permitting** | 12-24 months |
| **Financing & PPA negotiation** | 6-12 months |
| **Procurement** | 3-6 months |
| **Construction** | 6-12 months |
| **Commissioning** | 1-3 months |
| **TOTAL** | **28-57 months (2.5-5 years)** |

---

### Crew Size vs. Installation Time

**5 kW Residential Roof Mount**:
| Crew Size | Installation Time | Man-Hours |
|-----------|-------------------|-----------|
| 1 person (DIY) | 3-5 days | 24-40 hours |
| 2 people | 1.5-2 days | 24-32 hours |
| 3 people | 1 day | 24-30 hours |

**100 kW Commercial Flat Roof**:
| Crew Size | Installation Time | Man-Hours |
|-----------|-------------------|-----------|
| 4 people | 4 weeks | 640 hours |
| 6 people | 3 weeks | 720 hours |
| 8 people | 2 weeks | 640 hours |

**Optimal**: 6-person crew balances efficiency and coordination

---

## 📏 Space Requirements

### Roof Area Calculator

**Formula**:
$$\text{Required Roof Area} = \frac{P_{\text{system}} \times 1.3}{P_{\text{panel}} \times \eta_{\text{layout}}}$$

Where:
- $P_{\text{system}}$ = Desired system power (W)
- $P_{\text{panel}}$ = Individual panel power (W)
- $\eta_{\text{layout}}$ = Layout efficiency (typically 0.70-0.85)
- 1.3 = Spacing factor for ventilation and maintenance

---

### Panel Area Reference

**Standard Panel Sizes** (2025):

| Power | Dimensions | Area per Panel | Panels/kW | Area/kW |
|-------|------------|----------------|-----------|---------|
| **330W** | 65" × 39" | 17.6 sq ft | 3.03 | 53 sq ft |
| **370W** | 66" × 40" | 18.3 sq ft | 2.70 | 49 sq ft |
| **400W** | 67" × 40" | 18.6 sq ft | 2.50 | 46 sq ft |
| **450W** | 84" × 40" | 23.3 sq ft | 2.22 | 52 sq ft |
| **550W** (bifacial) | 90" × 44" | 27.5 sq ft | 1.82 | 50 sq ft |

**Metric Equivalent**:
| Power | Dimensions (mm) | Area (m²) |
|-------|-----------------|-----------|
| **400W** | 1700 × 1000 | 1.7 m² |
| **550W** | 2280 × 1134 | 2.6 m² |

---

### Roof Suitability Assessment

#### Minimum Requirements

| Roof Type | Min. Area | Max. Slope | Load Capacity | Condition |
|-----------|-----------|------------|---------------|-----------|
| **Asphalt shingle** | 200 sq ft | 45° | 4 lb/sq ft | <10 years old preferred |
| **Metal (standing seam)** | 200 sq ft | 60° | 5 lb/sq ft | Any age (if sound) |
| **Tile** | 300 sq ft | 35° | 6 lb/sq ft | Requires special mounting |
| **Flat (membrane)** | 400 sq ft | <5° | 5 lb/sq ft | Ballasted mounts |

**Load Calculation Example**:
```
Panel weight: 45 lb
Mounting: 15 lb
Snow load (design): 25 lb
Total: 85 lb per panel

Panel area: 18 sq ft
Load: 85 lb / 18 sq ft = 4.7 lb/sq ft ✅ (within typical limits)
```

---

### Ground Mount Space Requirements

**Fixed Ground Mount**:
```
Row spacing = Panel height × 2.5 (to prevent shading)

Example:
Panel height (tilted 30°): 3.5 ft
Row spacing: 3.5 × 2.5 = 8.75 ft

Array: 10 rows × 20 panels
Panel width: 3.3 ft
Total width: 20 × 3.3 = 66 ft
Total length: 10 × 8.75 = 87.5 ft
Total area: 66 × 87.5 = 5,775 sq ft (for 200 panels = 80 kW)

Area per kW: 5,775 / 80 = 72 sq ft/kW
```

**Single-Axis Tracker**:
- **Requires 30-40% more space** (for tracker rotation clearance)
- Area per kW: 90-100 sq ft/kW

---

## 📊 Load-Based Sizing

### Load Category Method

**Step 1: Categorize Loads**

| Category | Examples | Priority | Sizing Factor |
|----------|----------|----------|---------------|
| **Critical** | Medical equipment, security, refrigeration | Must run 24/7 | 1.5× (redundancy) |
| **Essential** | Lighting, communication, cooking | Daily use | 1.3× (safety margin) |
| **Comfort** | HVAC, entertainment, laundry | Deferrable | 1.0× (no extra) |
| **Luxury** | Pool, spa, workshop | Optional | 0.8× (can skip if needed) |

**Step 2: Calculate Weighted Load**

$$E_{\text{sized}} = (E_{\text{critical}} \times 1.5) + (E_{\text{essential}} \times 1.3) + (E_{\text{comfort}} \times 1.0) + (E_{\text{luxury}} \times 0.8)$$

---

### Example: Medium Residential Home

| Load | Power (W) | Hours/Day | Energy (Wh) | Category | Factor | Weighted (Wh) |
|------|-----------|-----------|-------------|----------|--------|---------------|
| Refrigerator | 150 | 24 | 3,600 | Critical | 1.5 | 5,400 |
| LED lights | 200 | 6 | 1,200 | Essential | 1.3 | 1,560 |
| TV + Internet | 150 | 5 | 750 | Essential | 1.3 | 975 |
| HVAC | 2,500 | 8 | 20,000 | Comfort | 1.0 | 20,000 |
| Washer/Dryer | 2,000 | 1 | 2,000 | Comfort | 1.0 | 2,000 |
| Hot tub | 3,000 | 2 | 6,000 | Luxury | 0.8 | 4,800 |
| **TOTAL** | — | — | **33,550** | — | — | **34,735** |

**System Sizing**:
```
Daily energy needed: 34,735 Wh = 34.7 kWh
PSH (location): 5.0
Panel power required: 34,700 / 5.0 = 6,940 W ≈ 7 kW system
```

---

## 🎛️ System Configuration Matrix

### Quick Sizing Table (Residential)

| Daily Consumption | System Size | Panel Count (400W) | Battery (48V) | Inverter | Approximate Cost |
|-------------------|-------------|--------------------|--------------|---------|--------------------|
| **5-10 kWh/day** | 2-3 kW | 5-8 | 200 Ah Li | 2000W | $8,000-15,000 |
| **10-20 kWh/day** | 4-6 kW | 10-15 | 300 Ah Li | 3000W | $15,000-25,000 |
| **20-35 kWh/day** | 7-10 kW | 18-25 | 400 Ah Li | 5000W | $25,000-40,000 |
| **35-50 kWh/day** | 11-15 kW | 28-38 | 600 Ah Li | 8000W | $40,000-60,000 |
| **50+ kWh/day** | 16-25 kW | 40-63 | 800+ Ah Li | 10000W+ | $60,000-100,000 |

---

### Commercial Quick Sizing

| Building Type | Peak Demand | System Size | Annual Production | Est. Cost |
|---------------|-------------|-------------|-------------------|-----------|
| **Small office** (2,000 sq ft) | 10-15 kW | 15-20 kW | 21,900-29,200 kWh | $30,000-40,000 |
| **Restaurant** | 30-50 kW | 40-60 kW | 58,400-87,600 kWh | $80,000-120,000 |
| **Retail store** (5,000 sq ft) | 20-35 kW | 30-50 kW | 43,800-73,000 kWh | $60,000-100,000 |
| **Warehouse** (20,000 sq ft) | 50-100 kW | 100-150 kW | 146,000-219,000 kWh | $200,000-300,000 |
| **School** | 100-250 kW | 150-300 kW | 219,000-438,000 kWh | $300,000-600,000 |

---

## 🧮 Quick Sizing Tools

### Rule-of-Thumb Calculators

#### Residential Grid-Tied

**Method 1: Annual Consumption**
```
System Size (kW) = Annual Consumption (kWh) / (365 × PSH)

Example:
Annual bill: 12,000 kWh
PSH: 5.0
System size: 12,000 / (365 × 5.0) = 6.58 kW ≈ 7 kW
```

**Method 2: Roof Area**
```
System Size (kW) = Available Roof Area (sq ft) / 60

Example:
South-facing roof: 400 sq ft
System size: 400 / 60 = 6.67 kW
```

---

#### Off-Grid

**Battery Bank Sizing**:
```
Ah = (Daily kWh × Days Autonomy × 1000) / (DoD × System Voltage)

Example:
Daily: 8 kWh
Autonomy: 3 days
DoD: 0.8 (lithium)
Voltage: 48V

Ah = (8 × 3 × 1000) / (0.8 × 48) = 625 Ah
```

**Panel Array Sizing**:
```
Panel Watts = (Daily kWh × 1.3 × 1000) / PSH

Example:
Daily: 8 kWh
PSH: 4.0 (worst month)
Panels: (8 × 1.3 × 1000) / 4.0 = 2,600 W
```

---

## 🎯 Key Takeaways

### ✅ Residential Sizing

1. **5 kW average** for typical US home (12,000 kWh/year)
2. **60 sq ft/kW** roof area rule-of-thumb
3. **$2.50-3.00/W** installed cost (2025)
4. **2-4 days** installation time
5. **7-10 year** payback period

### ✅ Commercial Sizing

1. **Size to offset peak demand** (demand charge savings)
2. **1.80-2.50/W** installed cost
3. **4-8 weeks** installation time (50-200 kW)
4. **5-8 year** payback period
5. **Incentives**: 30% ITC + depreciation (MACRS)

### ✅ Budget Planning

1. **Economy**: $2.50-3.00/W (basic components)
2. **Standard**: $2.20-2.70/W (quality components)
3. **Premium**: $2.00-2.50/W (best components, lithium)
4. **Phased installation** reduces upfront cost

### ✅ Space Planning

1. **50-70 sq ft/kW** typical (including spacing)
2. **Ground mount**: 70-100 sq ft/kW (including row spacing)
3. **Tracker**: +30-40% more space
4. **Roof load**: 4-6 lb/sq ft (including snow design)

---

## 🔗 Related Sections

- **Next**: [Cost Analysis & ROI →](cost-analysis.md)
- [Installation Guide →](installation-guide.md)
- [Material Lists & BOMs →](material-lists.md)
- [Detailed Case Studies →](detailed-case-studies.md)

---

<div align="center">

**[🏠 Back to Main README](../README.md)**

</div>
