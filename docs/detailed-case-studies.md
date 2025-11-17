# 📊 Detailed Case Studies

[← Back to Main](../README.md)

---

## 📑 Contents

- [Case Study 1: Residential Off-Grid](#-case-study-1-residential-off-grid)
- [Case Study 2: Commercial Grid-Tied](#-case-study-2-commercial-grid-tied)
- [Case Study 3: Industrial with Storage](#-case-study-3-industrial-with-storage)

---

## 🏡 Case Study 1: Residential Off-Grid

### Project Overview

**Location**: Colorado Mountains (39.5°N, 105.8°W)
**Client**: Weekend cabin owner
**System Type**: Off-grid with battery storage
**Completion**: March 2025

---

### Requirements Analysis

**Energy Consumption**:
| Load | Power | Hours/Day | Energy (Wh/day) |
|------|-------|-----------|-----------------|
| LED lights | 100W | 5h | 500 |
| Refrigerator | 150W | 24h | 3,600 |
| Laptops | 120W | 4h | 480 |
| Water pump | 500W | 0.5h | 250 |
| Microwave | 1,000W | 0.2h | 200 |
| TV/entertainment | 100W | 3h | 300 |
| Misc. | — | — | 300 |
| **TOTAL** | | | **5,630 Wh/day** |

**Design constraints**:
- Lowest temperature: -25°C
- PSH (worst month): 3.5 hours
- 3 days autonomy required
- Budget: $25,000-30,000

---

### System Design

**PV Array**:
- **Panels**: 8× Canadian Solar 330W TOPCon
- **Total capacity**: 2,640W
- **Configuration**: 4 series × 2 parallel
- **String Voc (cold)**: 209.8V
- **String Vmp**: 151.2V
- **Total Isc**: 18.9A

**Energy Storage**:
- **Type**: Discover AES Lead-Carbon
- **Configuration**: 3× 48V/154Ah banks = 462Ah @ 48V
- **Total capacity**: 22.2 kWh
- **Usable (50% DoD)**: 11.1 kWh
- **Days autonomy**: 11,100 Wh / 5,630 Wh = 2.0 days ✅

**Charge Controller**:
- **Model**: Victron SmartSolar MPPT 250/60
- **Max Voc**: 250V (209.8V actual ✅)
- **Max charge current**: 60A (55A actual ✅)

**Inverter**:
- **Model**: Victron MultiPlus 48/3000
- **Continuous power**: 3,000W
- **Surge power**: 6,000W
- **Efficiency**: 94%

---

### Complete BOM & Costs

| Component | Specification | Qty | Unit | Total |
|-----------|--------------|-----|------|-------|
| **Panels** | Canadian Solar 330W | 8 | $110 | $880 |
| **Ground mount** | Unirac SolarMount | 1 set | $1,800 | $1,800 |
| **Batteries** | Discover AES 48V/154Ah | 3 | $1,650 | $4,950 |
| **MPPT** | Victron 250/60 | 1 | $700 | $700 |
| **Inverter** | Victron MultiPlus 48/3000 | 1 | $1,800 | $1,800 |
| **PV wire** | 10 AWG, 200 ft | 1 | $240 | $240 |
| **Battery cables** | 2/0 AWG, 20 ft | 1 | $150 | $150 |
| **Combiner box** | 2-string, fused | 1 | $180 | $180 |
| **Breakers** | Assorted | — | $200 | $200 |
| **Monitoring** | Victron Color GX | 1 | $350 | $350 |
| **Misc. electrical** | Wire, conduit, etc. | — | $400 | $400 |
| **MATERIALS TOTAL** | | | | **$11,650** |
| **Labor** | 50 man-hours @ $100/hr | | | $5,000 |
| **Permits** | County building | | | $300 |
| **TOTAL PROJECT** | | | | **$16,950** |

---

### Installation Timeline

| Week | Phase | Man-Hours | Crew |
|------|-------|-----------|------|
| **Week 1** | Site prep, ground mount foundation (concrete piers) | 16 | 2 |
| **Week 2** | Racking assembly, panel installation | 24 | 2 |
| **Week 3** | Electrical, battery installation, commissioning | 20 | 2 |
| **TOTAL** | | **60** | **2 avg** |

**Timeline**: 3 weeks (weather permitting)

---

### Performance & ROI

**Annual Production**:
- Daily (worst month): 2,640W / 3.5 PSH = 9,240 Wh
- Daily (avg, 5.0 PSH): 13,200 Wh
- Annual: 13.2 kWh × 365 = 4,818 kWh

**Savings** (vs. generator):
- Propane generator cost: $0.40/kWh (fuel + maintenance)
- Annual savings: 4,818 kWh × $0.40 = $1,927

**Payback**: $16,950 / $1,927 = **8.8 years**

**Lifetime value** (25 years):
- Total savings: $1,927 × 25 = $48,175
- Battery replacement (year 10): -$5,000
- Inverter replacement (year 15): -$2,000
- **Net savings**: $48,175 - $16,950 - $7,000 = **$24,225**

---

## 🏢 Case Study 2: Commercial Grid-Tied

### Project Overview

**Location**: Houston, TX
**Client**: 50,000 sq ft warehouse
**System Type**: Grid-tied, no storage
**Completion**: June 2025

---

### Requirements

**Annual consumption**: 350,000 kWh
**Peak demand**: 120 kW
**Roof**: Flat, TPO membrane
**Goal**: Offset 80% of consumption

---

### System Design

**PV Array**:
- **Panels**: 375× Trina Vertex N 400W bifacial
- **Total capacity**: 150 kW
- **Configuration**: 25 strings × 15 panels
- **Mounting**: Ballasted, 10° tilt
- **Bifacial gain**: +12% (white roof)

**Inverters**:
- **Model**: 3× SolarEdge SE50K (50kW each)
- **Total capacity**: 150 kW
- **MPPT inputs**: 8 per inverter (24 total)

---

### Complete BOM & Costs

| Component | Cost |
|-----------|------|
| Panels (375× 400W) | $45,000 |
| Inverters (3× 50kW) | $24,000 |
| Ballasted racking | $30,000 |
| Electrical (DC/AC) | $12,000 |
| Monitoring system | $3,500 |
| **MATERIALS** | **$114,500** |
| Labor (400 man-hours @ $120/hr) | $48,000 |
| Engineering & design | $8,000 |
| Permits & inspection | $4,500 |
| Utility interconnection | $3,000 |
| **SOFT COSTS** | **$63,500** |
| **SUBTOTAL** | **$178,000** |
| Overhead & profit (25%) | $44,500 |
| **TOTAL** | **$222,500** |

**$/W**: $1.48/W (excellent commercial rate!)

---

### Financial Analysis

**Incentives**:
- Federal ITC (30%): -$66,750
- MACRS depreciation (26%): -$57,850
- **Net cost**: $97,900

**Annual savings**:
- Production: 150 kW × 5.2 PSH × 365 = 284,700 kWh
- With bifacial gain (+12%): 318,864 kWh
- Electricity rate: $0.11/kWh
- Demand charge savings: 100 kW × $12/kW × 12 = $14,400
- **Total savings**: (318,864 × $0.11) + $14,400 = **$49,475/year**

**Payback**: $97,900 / $49,475 = **2.0 years** 🚀

**ROI (25-year)**:
- Total savings: $49,475 × 25 = $1,236,875
- Inverter replacement (year 12): -$25,000
- **Net profit**: $1,236,875 - $97,900 - $25,000 = **$1,113,975**

**IRR**: **48.5%** (exceptional!)

---

## 🏭 Case Study 3: Industrial with Storage

### Project Overview

**Location**: California (high electricity rates)
**Client**: Manufacturing facility
**System Type**: Grid-tied + battery storage (demand shaving)
**Completion**: August 2025

---

### Requirements

**Peak demand**: 250 kW
**Annual consumption**: 1,200,000 kWh
**Demand charges**: $18/kW/month
**Time-of-use rates**: $0.35/kWh (peak), $0.12/kWh (off-peak)

---

### System Design

**PV Array**:
- **Capacity**: 300 kW (750× 400W panels)
- **Mounting**: Carport structure (covers parking lot)

**Energy Storage**:
- **Capacity**: 500 kWh lithium-ion
- **Power**: 250 kW discharge rate (1-hour)
- **Purpose**: Peak shaving + demand charge reduction

**Inverters**:
- **Model**: 3× SMA Sunny Central 100 kW
- **Hybrid**: Grid-tie with battery integration

---

### Complete Costs

| Component | Cost |
|-----------|------|
| PV system (300 kW) | $540,000 |
| Carport structure (adds cost) | +$150,000 |
| Battery system (500 kWh) | $400,000 |
| Additional electrical & controls | $80,000 |
| **TOTAL** | **$1,170,000** |

**After incentives**:
- Federal ITC (30%): -$351,000
- MACRS (26%): -$304,200
- **Net cost**: $514,800

---

### Financial Results

**Annual savings**:
- PV production: 300 kW × 5.8 PSH × 365 = 635,100 kWh
- Battery arbitrage: Shift 200 kWh/day × 365 = 73,000 kWh from peak to off-peak
  - Savings: 73,000 × ($0.35 - $0.12) = $16,790
- Demand charge reduction: 150 kW × $18 × 12 = $32,400
- Total energy savings: 635,100 × $0.25 (blended) = $158,775
- **Total annual savings**: $158,775 + $16,790 + $32,400 = **$207,965**

**Payback**: $514,800 / $207,965 = **2.5 years**

**25-year NPV** (6% discount): **$2.1M**

---

## 🎯 Key Takeaways

### ✅ Off-Grid Lessons

1. **Oversize PV** by 20-30% (cloudy days)
2. **3 days autonomy** minimum
3. **Lead-carbon** good budget alternative to lithium
4. **Ground mount** easier for maintenance/snow

### ✅ Commercial Lessons

1. **Demand charges** = huge savings opportunity
2. **Bifacial + white roof** = free 10-15% gain
3. **Payback <3 years** common with incentives
4. **MACRS depreciation** adds 26% benefit

### ✅ Industrial + Storage

1. **Peak shaving** highly valuable (high demand charges)
2. **Battery arbitrage** works with TOU rates
3. **Carport solar** dual-purpose (power + shade)
4. **ROI >40%** possible with optimal design

---

## 🔗 Related Sections

- **Previous**: [← Material Lists](material-lists.md)
- [Project Sizing →](project-sizing.md)
- [Cost Analysis →](cost-analysis.md)
- [Installation Guide →](installation-guide.md)

---

<div align="center">

**[🏠 Back to Main README](../README.md)**

</div>
