# Liquid Rack Integration Architecture
CDU Interface + Isolation Strategy

---

## 1. Purpose

This document defines how the hybrid cooling architecture interfaces with:

- Direct-to-Chip liquid cooling racks
- In-row CDU systems
- Facility cooling loops
- Mechanical chillers

CRITICAL PRINCIPLE:

The tower + geothermal system must NEVER directly enter the rack coolant loop.

Isolation is mandatory.

---

## 2. Standard Data Center Liquid Cooling Stack

Typical modern AI liquid-cooled rack layout:

Server cold plates  
→ Rack manifold  
→ Rack CDU (Coolant Distribution Unit)  
→ Facility cooling loop  
→ Chiller plant

The CDU isolates:

- IT loop (clean, controlled chemistry)
- Facility loop (industrial scale water)

---

## 3. Proposed Hybrid Integration Point

Correct insertion location:

CDU secondary (facility side) loop.

Architecture:

Rack IT Loop  
→ CDU heat exchanger  
→ Facility primary loop  
→ Hybrid Vertical Tower  
→ Geothermal loop  
→ Chiller plant (if required)

The hybrid system operates at the facility layer only.

---

## 4. Hydraulic Isolation Strategy

Each layer must be isolated with:

- Plate heat exchangers
- Check valves
- Differential pressure sensors
- Flow meters
- Expansion tanks

Minimum required boundaries:

1. IT loop isolation
2. Tower loop isolation
3. Geothermal loop isolation

Three-loop architecture recommended.

---

## 5. Three-Loop Cooling Architecture

Loop 1 – IT Loop
- Controlled chemistry
- Low oxygen
- Corrosion inhibited
- Managed by rack CDU

Loop 2 – Tower Loop
- High flow rate
- Large thermal rejection
- May include adiabatic assist

Loop 3 – Geothermal Loop
- Closed HDPE ground circuit
- Separate pump set
- Stabilization only

Loop 4 – Mechanical Backup
- Chiller integration
- Automatic switchover

---

## 6. Control Strategy

Priority order:

1. Tower only
2. Tower + geothermal
3. Geothermal only
4. Chiller assist
5. Full mechanical fallback

Chiller lockout enabled when:

Facility supply temp ≤ target return threshold

---

## 7. Temperature Targets

Typical AI rack supply temperatures:

60–75°F liquid supply  
Return may be 80–95°F

Tower target:

Reduce facility return temp by 5–15°F

Example:

Rack return = 90°F  
Tower output = 80°F  
Geothermal stabilization = 75°F  
Chiller only trims remainder.

---

## 8. Flow Rate Considerations

High density AI racks:

40–100 kW per rack

Example:

100 kW rack  
10°F delta  
Flow required ≈ 20–25 GPM per rack

For 100 racks:

2,000–2,500 GPM facility loop

Tower must support full facility flow rate.

---

## 9. Pressure & Pumping

Important clarification:

In closed loops:

Vertical height does NOT increase net static pump load.

Pump load determined by:

- Friction losses
- Heat exchanger ΔP
- Radiator core resistance
- Pipe length

Gravity assists:

- Downflow stability
- Air purge efficiency
- Transient pressure smoot
