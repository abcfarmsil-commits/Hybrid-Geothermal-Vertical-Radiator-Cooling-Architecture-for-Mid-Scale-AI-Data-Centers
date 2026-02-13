# Vertical Radiator Tower (VRT) Specification
Hybrid Geothermal + Gravity-Assisted Cooling Architecture

---

## 1. Purpose

The Vertical Radiator Tower (VRT) is a passive / semi-passive heat rejection
structure designed to:

- Reduce mechanical chiller compressor runtime
- Utilize building height + added tower head (~60 ft target)
- Improve ΔT before mechanical cooling stage
- Enable dry-mode rejection in shoulder seasons
- Support optional adiabatic assist
- Integrate with geothermal stabilization loop

The tower is not intended to replace chillers.
It is designed to reduce compressor load and runtime hours.

---

## 2. Target Design Parameters

| Parameter | Target |
|------------|--------|
| Effective head | 60 ft (building + tower) |
| Operating mode | Closed-loop water |
| Thermal target | 5–15°F drop pre-chiller |
| Flow type | Pump-assisted primary loop |
| Materials | Aluminum core + corrosion-safe piping |
| Mode | Dry primary, adiabatic optional |

---

## 3. Physics Foundation

### 3.1 Thermal Rejection Equation

Heat removed:

Q = ṁ × c_p × ΔT

For water (engineering rule):

MW_thermal ≈ 0.000244 × GPM × ΔT(°F)

Example:
- 1,500 GPM
- 10°F drop

MW_thermal ≈ 0.000244 × 1500 × 10  
= 3.66 MW thermal rejection

---

### 3.2 Height Advantage

Height provides:

1. Increased radiator surface area opportunity
2. Natural convective enhancement
3. Improved static pressure control
4. Easier gravity-assisted downflow
5. Stratified heat release potential

Important:
Height does NOT create free energy.
It improves system geometry and stability.

---

## 4. Structural Configuration

### 4.1 Core Layout

Hot water supply →  
Upward insulated riser →  
Vertical radiator panels (finned aluminum) →  
Optional adiabatic mist assist →  
Return downflow →  
Heat exchanger →  
Rack liquid loop / chiller

---

### 4.2 Radiator Sections

Each vertical section consists of:

- Extruded aluminum core tubing
- Finned heat exchange surfaces
- Modular 8–12 ft panel sections
- Parallel flow manifolds

Estimated stacking:
- 5–8 stacked sections
- Total height: 40–60 ft

---

## 5. Materials Selection

### 5.1 Heat Exchange Core

Preferred:
- Aluminum (high conductivity, lightweight)

Alternative:
- Copper (higher conductivity, higher cost)
- Stainless steel (durable, lower conductivity)

Thermal conductivity reference:
- Aluminum ≈ 205 W/mK
- Copper ≈ 385 W/mK
- Steel ≈ 16 W/mK

Aluminum provides best balance of cost and weight.

---

### 5.2 Structural Frame

- Galvanized steel
- Corrosion-resistant coating
- Seismic-rated anchor system

---

### 5.3 Fluid Circuit

Closed loop:
- Treated water or glycol mix
- Corrosion inhibitor package
- Oxygen control

---

## 6. Operating Modes

### 6.1 Dry Mode (Primary)

Ambient air removes heat through fin stack.

Best used:
- Night operation
- Shoulder seasons
- Cooler climates

---

### 6.2 Adiabatic Assist (Optional)

Non-potable water mist lowers air intake temperature.

Can provide:
- 5–15°F effective air temp reduction
- Major peak shaving during hot months

Water source options:
- Rain capture
- Greywater (treated)
- Cooling loop reclaim

---

### 6.3 Geothermal Assist Mode

During high ambient temps:

- Tower rejects partial load
- Geothermal stabilizes remainder
- Chiller handles only peak residual

---

## 7. Pumping & Head Considerations

Static head from height does NOT increase pump load
in a closed loop (upward head cancels downward return).

Pump sizing determined by:
- Friction loss
- Radiator core resistance
- Heat exchanger ΔP
- Pipe length

Gravity assists:
- Downward return stabilization
- Air purge improvement
- Cavitation mitigation

---

## 8. Control Logic Overview

Priority sequence:

1. Dry tower only
2. Dry + geothermal
3. Dry + adiabatic
4. Geothermal primary
5. Mechanical chiller assist

Goal:
Lock out compressors whenever possible.

---

## 9. Integration With Liquid Rack Cooling

Rack CDU loop →
Plate heat exchanger →
Tower primary loop →
Geothermal secondary loop →
Chiller tertiary stage (if required)

Important:
The tower should interface at the facility loop,
not directly inside rack CDUs.

---

## 10. Expected Performance Range

For 10 MW IT facility:

Conservative:
- 5°F drop
- 15% compressor reduction

Moderate:
- 10°F drop
- 25% compressor reduction

Aggressive:
- 12–15°F drop
- 30–35% reduction during shoulder seasons

Actual values climate-dependent.

---

## 11. Risks & Engineering Considerations

- Wind load at 60 ft
- Freeze protection
- Glycol viscosity increase
- Corrosion management
- Noise (if fan assist used)
- Municipal permitting height limits

---

## 12. Advantages vs Traditional Cooling Towers

| Traditional Tower | Vertical Radiator Tower |
|------------------|------------------------|
| Large basin | Closed loop |
| Evaporative dominant | Dry-first design |
| Legionella risk | Reduced risk |
| High water consumption | Optional water use |
| Large footprint | Vertical footprint |

---

## 13. Scaling Strategy

Single Tower:
- 3–5 MW support

Dual Tower:
- 5–10 MW support

Cluster Array:
- 10–20 MW support

Designed for mid-scale AI facilities first.

---

## 14. Future Work

- CFD modeling
- Hourly climate simulation
- Radiator UA curve development
- Parasitic fan energy optimization
- Cost per kW rejection benchmarking
