# Geothermal Integration Architecture
Hybrid Vertical Radiator + Ground Stabilization Loop

---

## 1. Purpose

The geothermal loop is designed to:

- Stabilize return temperatures from the vertical radiator tower
- Provide thermal buffering during high ambient heat
- Reduce peak compressor load
- Improve seasonal cooling consistency
- Enable hybrid passive + mechanical optimization

This system does NOT replace chillers.
It reduces compressor runtime and peak load.

---

## 2. System Role in Cooling Hierarchy

Priority Order:

1. Vertical Radiator Tower (dry rejection)
2. Vertical Tower + Adiabatic Assist
3. Geothermal Stabilization Loop
4. Mechanical Chiller
5. Emergency Backup Cooling

The geothermal loop acts as a thermal shock absorber.

---

## 3. Ground Loop Configuration

### 3.1 Closed-Loop Vertical Bore System (Preferred)

- 200–500 ft boreholes
- HDPE U-bend piping
- Grouted with high conductivity backfill
- Manifolded in parallel arrays

Advantages:
- Predictable performance
- No aquifer permitting issues
- Low maintenance

---

### 3.2 Horizontal Field (Alternative)

- Requires large land area
- 6–10 ft burial depth
- More temperature swing exposure

Better for rural deployments.

---

## 4. Thermal Performance Characteristics

Ground temperature typically:

- 50–65°F stable year-round (climate dependent)

If tower return temperature = 90°F  
Ground = 55°F  

Potential ΔT stabilization:

Up to 10–20°F buffering before mechanical cooling.

---

## 5. Heat Transfer Modeling

Thermal exchange rate:

Q = U × A × ΔT

Where:
- U = overall heat transfer coefficient
- A = pipe surface area
- ΔT = temperature difference

Typical bore field sizing:

For 1 MW thermal rejection:
- ~20–40 vertical wells (depending on soil conductivity)

For 5 MW support:
- 100+ boreholes possible

Exact sizing climate dependent.

---

## 6. Hybrid Flow Architecture

Data Hall Loop →
Plate Heat Exchanger →
Primary Vertical Tower Loop →
Geothermal Secondary Loop →
Chiller Tertiary Stage

Important:
Geothermal loop should be hydraulically isolated from rack CDUs.

---

## 7. Seasonal Operation Modes

### 7.1 Winter / Cool Climate

Tower handles majority of rejection.
Geothermal minimal usage.

### 7.2 Shoulder Season

Tower + geothermal hybrid.
Chillers mostly locked out.

### 7.3 Peak Summer

Tower pre-cools.
Geothermal stabilizes.
Chillers handle only residual.

---

## 8. Energy Impact Modeling

For a 10 MW IT facility:

Cooling load ≈ 30–40% of IT load  
≈ 3–4 MW cooling demand

If geothermal reduces compressor load by:

15–25%

Annual electrical savings:

~0.5–1.0 MW continuous equivalent

Annual kWh savings:

0.75 MW × 8760 hours ≈ 6,570,000 kWh

At $0.08/kWh:

≈ $525,600/year savings

Carbon reduction:

Assume 0.4 kg CO₂/kWh grid factor

6,570,000 × 0.4 = 2,628,000 kg CO₂  
= 2,628 metric tons CO₂ annually

---

## 9. CAPEX Considerations

Estimated cost per borehole:

$8,000 – $15,000 (region dependent)

For 50 boreholes:

$400k – $750k installed

ROI target window:

5–8 years depending on electricity rates.

---

## 10. Risks & Engineering Constraints

- Soil conductivity variability
- Drilling permits
- Urban site constraints
- Ground thermal saturation over time
- Proper load balancing required

Thermal recharge modeling is critical.

---

## 11. Why Combine with Vertical Radiator Tower?

Geothermal alone:
- Expensive to oversize
- Ground saturation risk

Tower alone:
- Ambient dependent

Hybrid:
- Reduces bore field size
- Reduces tower load
- Reduces chiller dependency
- Improves system resilience

This combination creates layered cooling redundancy.

---

## 12. Future Modeling Work

- Soil conductivity simulation
- 8760-hour seasonal modeling
- Borefield thermal recovery modeling
- Hybrid optimization algorithm
- CAPEX vs MW offset curve
