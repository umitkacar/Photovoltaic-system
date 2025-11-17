# 📦 Material Lists & Bill of Materials (BOM)

[← Back to Main](../README.md)

---

## 📑 Contents

- [BOM Templates](#-bom-templates)
- [Component Specifications](#-component-specifications)
- [Supplier Guide](#-supplier-guide)
- [Procurement Tips](#-procurement-tips)

---

## 📋 BOM Templates

### Template 1: 6 kW Residential (Grid-Tied)

**System Specifications**:
- **Capacity**: 6,000W
- **Panels**: 15× 400W mono TOPCon
- **Inverter**: String inverter, 6kW
- **Mounting**: Roof mount (asphalt shingle)
- **Location**: Residential, grid-tied

---

#### Complete Bill of Materials

| Category | Item | Spec | Qty | Unit Price | Total |
|----------|------|------|-----|------------|-------|
| **PANELS** |
| | Mono TOPCon panel | 400W, 24% eff | 15 | $128 | $1,920 |
| **INVERTER** |
| | String inverter | 6kW, 98% eff | 1 | $1,800 | $1,800 |
| **RACKING** |
| | Aluminum rails | 168" length | 6 | $45 | $270 |
| | Roof flashings | Universal | 36 | $12 | $432 |
| | Mid clamps | Anodized aluminum | 28 | $3 | $84 |
| | End clamps | Anodized aluminum | 8 | $4 | $32 |
| | L-feet | Adjustable | 36 | $5 | $180 |
| | Lag bolts | 5/16" × 3" | 144 | $0.50 | $72 |
| **ELECTRICAL (DC)** |
| | PV wire | 10 AWG, 600V | 200 ft | $1.20/ft | $240 |
| | MC4 connectors | Pairs | 10 | $3 | $30 |
| | Cable clips | UV-resistant | 50 | $0.30 | $15 |
| | PV combiner box | 2-string, fused | 1 | $180 | $180 |
| | DC disconnect | 600V, 30A | 1 | $120 | $120 |
| **ELECTRICAL (AC)** |
| | AC wire | 10 AWG THHN | 50 ft | $0.80/ft | $40 |
| | EMT conduit | 3/4", 10 ft sections | 3 | $18 | $54 |
| | AC breaker | 30A, dual-pole | 1 | $35 | $35 |
| | Junction boxes | 4×4 | 2 | $8 | $16 |
| **GROUNDING** |
| | Ground wire | #6 AWG bare copper | 100 ft | $1.50/ft | $150 |
| | Grounding lugs | WEEB style | 12 | $4 | $48 |
| **CONSUMABLES** |
| | Roof sealant | Polyurethane, 10 oz tube | 6 | $8 | $48 |
| | Thread locker | Blue Loctite | 2 | $12 | $24 |
| | Cable ties | UV black, 100 pack | 2 | $15 | $30 |
| | Warning labels | NEC compliant set | 1 | $25 | $25 |
| **MONITORING** |
| | Production monitor | WiFi-enabled | 1 | $250 | $250 |
| |**SUBTOTAL** | | | | | **$6,095** |
| **LABOR** | Installation (30 man-hours @ $100/hr) | | | | $3,000 |
| **PERMITS** | Building + electrical | | | | $500 |
| **CONTINGENCY** | 5% for misc. | | | | $380 |
| **TOTAL PROJECT COST** | | | | | **$9,975** |

**With overhead & profit (80%)**: $17,955 → **~$18,000 installed**

---

### Template 2: 10 kW Off-Grid (with Battery)

**System Specifications**:
- **Capacity**: 10,000W
- **Panels**: 25× 400W
- **Battery**: 48V, 400Ah lithium LFP
- **MPPT**: 100A, 250V
- **Inverter**: 5kW pure sine wave

#### BOM Summary

| Category | Items | Cost |
|----------|-------|------|
| Panels (25× 400W) | TOPCon bifacial | $3,200 |
| Ground mount racking | Galvanized steel | $2,500 |
| Lithium battery (400Ah @ 48V) | LFP, 19.2 kWh | $12,000 |
| MPPT charge controller | 100A, 250V | $850 |
| Inverter/charger | 5kW hybrid | $2,200 |
| Electrical (DC/AC) | Wire, breakers, disconnects | $900 |
| Grounding & safety | Components | $300 |
| **SUBTOTAL** | | **$21,950** |
| Labor (50 man-hours) | | $5,000 |
| **TOTAL** | | **$26,950** |

---

### Template 3: 100 kW Commercial Flat Roof

#### BOM Summary

| Category | Qty | Unit Cost | Total |
|----------|-----|-----------|-------|
| **Panels** (250× 400W bifacial) | 250 | $120 | $30,000 |
| **Inverters** (2× 50kW string) | 2 | $8,500 | $17,000 |
| **Ballasted racking** | 250 panels | $80/panel | $20,000 |
| **Combiner boxes** (8-string ea.) | 4 | $800 | $3,200 |
| **DC wire & conduit** | Bulk | | $4,500 |
| **AC equipment** (panel, breakers, meter) | | | $3,500 |
| **Monitoring system** (string-level) | 1 | $2,500 | $2,500 |
| **SUBTOTAL** | | | **$80,700** |
| **Labor** (400 man-hours @ $120/hr) | | | $48,000 |
| **Engineering & design** | | | $8,000 |
| **Permits & inspection** | | | $3,000 |
| **Overhead & profit** (35%) | | | $48,745 |
| **TOTAL** | | | **$188,445** |

**$/W**: $1.88/W

---

## 🔍 Component Specifications

### Solar Panels

**Residential** (400W typical):
- **Dimensions**: 67" × 40" (1.7m × 1.0m)
- **Weight**: 45-50 lb (20-23 kg)
- **Technology**: Mono TOPCon or PERC
- **Warranty**: 25-year performance (80%+)
- **Certifications**: UL 1703, IEC 61215

**Commercial/Utility** (500-600W):
- **Dimensions**: 90" × 44" (2.3m × 1.1m)
- **Weight**: 60-70 lb (27-32 kg)
- **Technology**: Bifacial TOPCon or HJT
- **Warranty**: 30-year performance

---

### Inverters

#### String Inverters
**Residential**: 3-10 kW, single-phase
- Input: 200-600V DC
- Output: 240V AC, 60Hz
- Efficiency: 97-99%
- Warranty: 10-25 years

**Commercial**: 20-100 kW, three-phase
- Input: 300-1000V DC
- Output: 480V AC, 60Hz
- Efficiency: 98-99%

---

## 🏬 Supplier Guide

### Panel Manufacturers

| Tier | Brand | Technology | Warranty | Price Range |
|------|-------|------------|----------|-------------|
| **Tier 1** | Jinko, Trina, Longi, Canadian Solar | TOPCon | 25-30 yr | $0.28-0.35/W |
| **Tier 2** | JA Solar, Risen, Hanwha | PERC/TOPCon | 25 yr | $0.22-0.30/W |
| **Premium** | SunPower, REC, Meyer Burger | HJT, IBC | 25-40 yr | $0.40-0.55/W |

---

### Inverter Manufacturers

| Brand | Type | Market | Reliability |
|-------|------|--------|-------------|
| **SolarEdge** | Optimizers + String | Residential/Commercial | ⭐⭐⭐⭐⭐ |
| **Enphase** | Microinverters | Residential | ⭐⭐⭐⭐⭐ |
| **Fronius** | String | Residential/Commercial | ⭐⭐⭐⭐⭐ |
| **SMA** | String, Central | Commercial/Utility | ⭐⭐⭐⭐⭐ |
| **Victron** | Off-grid/Hybrid | Off-grid | ⭐⭐⭐⭐⭐ |

---

### Distributor/Wholesalers (USA)

| Company | Focus | Min. Order | Pro Account |
|---------|-------|------------|-------------|
| **CED Greentech** | Full-service | $500 | Free (contractors) |
| **Soligent** | Nationwide | $1,000 | Free |
| **Sunwize** | Off-grid specialist | $500 | Free |
| **Wholesale Solar** | DIY-friendly | No minimum | Not required |
| **altE Store** | Residential/Off-grid | No minimum | Not required |

---

## 💡 Procurement Tips

### Volume Discounts

| Order Size | Typical Discount |
|------------|-----------------|
| 1-10 panels | List price |
| 11-50 panels | 5-10% off |
| 50-200 panels | 10-15% off |
| 200+ panels (pallet) | 15-20% off |

---

### Timing Strategies

**Best time to buy**:
- **Q1** (Jan-Mar): Slow season, better pricing
- **Q4** (Oct-Dec): End-of-year clearance

**Avoid**:
- **Summer peak** (June-Aug): High demand, higher prices

---

### Warranty Considerations

**Panel warranties** (read fine print!):
- **Product warranty**: 10-15 years (defects)
- **Performance warranty**: 25-30 years (80%+ output)
- **Linear vs. tiered**: Linear is better (guaranteed annual degradation)

**Inverter warranties**:
- **Standard**: 10-12 years
- **Extended**: 20-25 years (purchase at install, ~$200-500)

---

## 🎯 Key Takeaways

### ✅ BOM Development

1. **Start with spec sheet** (panel, inverter ratings)
2. **Calculate quantities** (panels, clamps, wire)
3. **Add 10% contingency** for damaged/defective parts
4. **Get 3 quotes** minimum

### ✅ Cost Optimization

1. **Bulk buy** panels (pallet = 28-32 panels)
2. **Single supplier** for discounts
3. **Off-season** purchasing (Q1, Q4)
4. **Quality over price** (warranty matters!)

### ✅ Lead Times

1. **Panels**: 2-8 weeks
2. **Inverters**: 2-6 weeks
3. **Batteries**: 4-12 weeks (lithium)
4. **Racking**: 1-4 weeks

---

## 🔗 Related Sections

- **Previous**: [← Installation Guide](installation-guide.md)
- **Next**: [Detailed Case Studies →](detailed-case-studies.md)
- [Cost Analysis →](cost-analysis.md)

---

<div align="center">

**[🏠 Back to Main README](../README.md)**

</div>
