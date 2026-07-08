# Design Review Template

> Structured framework for engineering design reviews.

---

## Review Info

| Field | Value |
|---|---|
| **Project** | [Name] |
| **Review Date** | YYYY-MM-DD |
| **Review Type** | Schematic / PCB / Firmware / System |
| **Reviewers** | [Names] |

---

## Checklist

### Schematic

- [ ] Power supply design verified (input range, output, ripple)
- [ ] Decoupling capacitors placed correctly
- [ ] Reset circuit verified
- [ ] Clock source selected and verified
- [ ] Debug interface included (SWD/JTAG)
- [ ] Unused pins properly terminated
- [ ] ESD protection on external interfaces

### PCB

- [ ] Stack-up defined (layers, thickness)
- [ ] Power plane impedance checked
- [ ] Differential pairs routed (if applicable)
- [ ] Sensitive analog area isolated
- [ ] Thermal considerations addressed
- [ ] Test points added for critical signals

### Firmware

- [ ] Boot sequence verified
- [ ] Watchdog timer configured
- [ ] Error handling implemented
- [ ] Memory usage within limits
- [ ] Interrupt priorities assigned

---

## Findings

| # | Severity | Description | Owner | Status |
|---|---|---|---|---|
| 1 | High/Med/Low | ... | ... | Open/Closed |

---

## Decision

- [ ] Approved with no changes
- [ ] Approved with minor changes
- [ ] Re-review required
- [ ] Rejected

---

*Template version: v1.0*
