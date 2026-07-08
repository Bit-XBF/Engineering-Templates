# EMC Design Checklist

> Pre-layout and pre-compliance checklist for electromagnetic compatibility.

---

## PCB Layout

### Stack-up

- [ ] Dedicated ground plane (continuous, no splits)
- [ ] Power and ground planes adjacent (low impedance)
- [ ] Signal layers adjacent to reference planes

### Routing

- [ ] High-speed signals routed on inner layers
- [ ] Clock traces as short as possible
- [ ] Differential pairs length-matched and tightly coupled
- [ ] No traces crossing split planes

### Grounding

- [ ] Single-point ground for low-frequency analog
- [ ] Multi-point ground for high-frequency digital
- [ ] Chassis ground separated from signal ground
- [ ] Stitching vias around board edge (≤ λ/20 spacing)

---

## Filtering & Decoupling

- [ ] Decoupling capacitor per power pin (100nF, close to pin)
- [ ] Bulk capacitor per power rail (10-100µF)
- [ ] Ferrite bead on sensitive analog supplies
- [ ] Common-mode choke on external power input
- [ ] Pi-filter on I/O lines if needed

---

## Shielding

- [ ] Shield can over sensitive / noisy circuits (if applicable)
- [ ] Shield connected to ground at multiple points
- [ ] No long slots or gaps in shield
- [ ] Cable shield terminated 360° at connector

---

## I/O & Connectors

- [ ] ESD protection on all external connectors
- [ ] TVS diode selection verified (clamping voltage < IC max)
- [ ] Series resistor on fast digital outputs (reduce edge rate)
- [ ] RC filter on slow digital inputs (debounce + filtering)

---

## Surge & EFT

- [ ] Surge protection on power input (if required by standard)
- [ ] Gas discharge tube / MOV for high-energy surges
- [ ] Clearance and creepage distances checked

---

## Pre-Compliance Checks

- [ ] Near-field probe scan (identify hot spots)
- [ ] Spectrum analyzer check for unexpected emissions
- [ ] ESD gun test on exposed connectors (if available)

---

*Template version: v1.0*
