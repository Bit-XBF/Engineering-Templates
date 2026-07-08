# Hardware Design Checklist

> Pre-design-freeze verification checklist for hardware projects.

---

## Power

- [ ] Input voltage range verified
- [ ] Output voltage accuracy within spec
- [ ] Ripple and noise within limits
- [ ] Power-up sequence correct (if multi-rail)
- [ ] Reverse polarity protection in place
- [ ] Overcurrent / short-circuit protection designed
- [ ] Thermal calculation completed

## Microcontroller

- [ ] Boot mode pins configured
- [ ] Reset circuit (RC / supervisor) verified
- [ ] Clock source (crystal / internal) selected
- [ ] SWD/JTAG debug interface accessible
- [ ] Unused pins terminated (pull-up / pull-down / output)
- [ ] Watchdog available and configured

## Communication Interfaces

- [ ] Termination resistors correct (CAN / RS485)
- [ ] ESD protection on external connectors
- [ ] Pull-up resistors for I2C
- [ ] UART level matching (3.3V / 5V / RS232)

## Analog

- [ ] ADC reference voltage stable
- [ ] Anti-aliasing filter in place
- [ ] Sensor excitation circuit verified
- [ ] Analog and digital grounds separated

## Mechanical & Layout

- [ ] Board outline and mounting holes defined
- [ ] Connector placement accessible
- [ ] High-current traces width adequate
- [ ] Keep-out zones respected

---

*Template version: v1.0*
