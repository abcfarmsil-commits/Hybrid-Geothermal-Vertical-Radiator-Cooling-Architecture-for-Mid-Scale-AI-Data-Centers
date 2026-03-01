# ABCFarmsIL — Impact Metrics Dictionary (MRV Spec)

**Scope:** Phase 0.8 → Phase 2 of the modular agro-ecosystem. All metrics are designed to be log-backed, reconcilable, and auditable.

> MRV = Measurement, Reporting, Verification.

## Microgreens Grown (trays / month)

**Definition:** Finished trays harvested at sellable quality; excludes failed/composted trays.

**Method:** Count trays from harvest log; reconcile with sales invoices (line items by tray).

**Instrumentation / Data:** Harvest QR/batch log; invoice exports (CSV/PDF).

**Frequency:** Weekly log, monthly roll-up.

**QA / Verification:** Spot photo of first/last tray per batch; reconcile harvest vs. sales within ±3%.

**Verification Artifacts:** Harvest log CSV + 4 photos/month + invoice export.

**Notes:** Phase targets: 0.8 = ~80 trays/mo; 1 = 200–400 trays/mo; 2 = 400+ trays/mo.

---

## Carbon Offset (tCO2e / year)

**Definition:** (A) Avoided transport emissions from local deliveries + (B) avoided landfill methane from organics diverted to fungi/vermi + (C) renewable kWh displacement, minus operational energy.

**Method:** Apply standard factors: gCO2e/mile by vehicle class; kgCO2e/kg organic waste; kgCO2e/kWh grid intensity. Sum A+B+C and subtract operational energy footprint.

**Instrumentation / Data:** Delivery miles log; organics diversion mass log; inverter kWh export; utility kWh.

**Frequency:** Monthly calculation; annual attestation.

**QA / Verification:** Maintain a versioned factor sheet; document system boundaries once and keep constant.

**Verification Artifacts:** Carbon Calc spreadsheet + delivery log + diversion log + utility bills + inverter CSV.

**Notes:** Phase signposts: Phase 1 ≈ 18 tCO2e/yr; Phase 2 ≈ 36 tCO2e/yr (illustrative targets).

---

## Water Reuse Rate (%)

**Definition:** Percent of total process water demand met by recirculated/reclaimed sources.

**Method:** Install two meters: (i) make-up water added, (ii) recirculated water volume. Monthly reuse = recirc ÷ (recirc + make-up).

**Instrumentation / Data:** Two inline meters; monthly meter photos and readings.

**Frequency:** Monthly.

**QA / Verification:** Sanity check against production volume (trays/mo) to flag anomalies.

**Verification Artifacts:** Meter log + monthly photo set.

**Notes:** Note: set acceptable drift band seasonally as system stabilizes.

---

## Renewable Energy Use (%)

**Definition:** Percent of total electrical demand met by on-site PV/battery generation.

**Method:** Monthly RE share = inverter production ÷ (inverter production + utility import).

**Instrumentation / Data:** Inverter app export (CSV) and utility bill (kWh).

**Frequency:** Monthly.

**QA / Verification:** Cross-check seasonality (winter/summer) and inverter uptime; flag gaps >24h.

**Verification Artifacts:** PDF utility bills + inverter CSV.

**Notes:** Phase targets: 0–50% (0.8), ~70% (Phase 1), 92–100% (Phase 2).

---

## Jobs Created (FTE)

**Definition:** Full-time equivalent roles directly employed in operations (paid hours only).

**Method:** FTE = total paid hours in quarter ÷ 520; exclude volunteer hours.

**Instrumentation / Data:** Payroll system export; contractor invoices with time detail.

**Frequency:** Quarterly (with annual roll-up).

**QA / Verification:** Maintain role descriptions; prevent double counting across grants.

**Verification Artifacts:** Timesheet summary, payroll export (PDF/CSV).

---

## Youth Trained (count / year)

**Definition:** Learners who complete all required checklists for assigned modules.

**Method:** Completion verified via signed module checklists + attendance records.

**Instrumentation / Data:** Training checklist packet; roster with dates.

**Frequency:** Quarterly review; annual count.

**QA / Verification:** Random audit of 10% of packets for signature/date completeness.

**Verification Artifacts:** Signed checklists (PDF) + roster (CSV).

**Notes:** Phase targets: 3/yr (0.8), 6/yr (1), 12/yr (2).

---

## Local Deliveries (miles)

**Definition:** Maximum one-way delivery radius for product distribution.

**Method:** Calculate straight-line or route distance from facility to customer addresses; store per order.

**Instrumentation / Data:** Delivery log with addresses (or ZIP centroid) and computed miles.

**Frequency:** Monthly monitor; flag orders beyond target radius.

**QA / Verification:** Distance recomputation spot-check 1/month; verify geocoding method stays fixed.

**Verification Artifacts:** Delivery log (CSV) + distance method note.

**Notes:** Phase targets: <10 miles (0.8), <15 miles (1–2).

---

## Standard Claims Language

- Microgreens outputs are derived from reconciled harvest and sales logs with ±3% tolerance.

- Carbon claims follow a documented boundary and factor sheet; spreadsheets available on request.

- Water reuse and renewable energy shares are meter-based and reported monthly.

- Jobs and training counts are verified against payroll and signed module checklists.
