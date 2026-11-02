# Role 3: Topics

## 1. Cryogenics
- Why superconducting qubits need millikelvin temperatures
- Dilution refrigerator principle (He-3/He-4 mixture)
- Pulse-tube coolers and cryogen-free systems
- Thermal stages (room, 50 K, 4 K, about 800 mK, about 100 mK, about 10 mK) and heat loads
- Helium-3 supply, recovery, and cost constraints
- Cooldown and warm-up procedures and their risks

## 2. Wiring and thermal management
- Coaxial wiring through stages; attenuators and filters at each stage
- Thermal anchoring and heat leaks
- Cryogenic amplifiers (HEMT, JPA) and their power budget
- Cable selection, bending radius, and handling

## 3. Power and cooling
- Peak vs. steady-state power for cryostats, control racks, and compressors
- Cooling water specifications (temperature, flow, quality)
- Heat rejection to room air and facility HVAC
- Redundancy: UPS, generator backup, and power quality

## 4. Environmental control
- Temperature and humidity specifications (for example, 25–60% non-condensing, from the LRZ paper)
- Magnetic field measurement (DC and AC) and shielding
- Floor loading and vibration
- Acoustic noise and fluorescent lighting interference
- Electromagnetic interference from nearby equipment (including GPU racks)

## 5. Site survey and installation
- Site survey checklist (fields, vibration, temperature, humidity, sound, floor)
- Installation sequence: cryostat, control racks, gas handling, cooling loops
- Commissioning and acceptance testing
- Vendor responsibilities versus facility responsibilities

## 6. Facility monitoring and operations
- Sensors: cryostat temperatures, pressures, pump status, power, water flow, room environment
- Alarm thresholds and escalation
- Maintenance schedules for pumps, compressors, and gas handling
- Logs and retention for audit and root cause analysis

## 7. Safety and compliance
- Cryogen safety (helium, nitrogen) and oxygen-deficiency monitoring
- High-voltage and electrical safety in control racks
- Export controls on quantum equipment and components (overview)
- Supply-chain constraints for He-3 and specialist components (overview)

## 8. Quantum concepts that affect the facility
- Why temperature and magnetic fields change qubit frequency and coherence
- Why calibration drifts when the environment drifts
- Why uptime and calibration windows are operational metrics

## Tools to learn
- Building-management and SCADA concepts (for facility monitoring)
- Prometheus or your site's monitoring stack, with vendor sensor exports
- Basic electrical and plumbing drawings
- Spreadsheet or Python for site survey data analysis
