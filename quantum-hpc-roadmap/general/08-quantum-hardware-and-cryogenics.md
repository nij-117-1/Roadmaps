# Phase 8: Quantum Hardware and Cryogenics

**Duration:** 4–6 weeks (overview for most roles; deeper if you target hardware or facility roles)
**Goal:** Understand how physical qubits are built and controlled, and what a quantum computer needs from its facility. Essential for any quantum infrastructure job.

## Topics and subtopics

### 8.1 Qubit modalities (overview)
- **Superconducting qubits:** transmons, microwave control, typical frequencies and coherence times
- **Trapped ions:** hyperfine or optical qubits, laser control, high fidelities
- **Neutral atoms:** optical tweezers, Rydberg interactions, reconfigurable arrays
- **Photonic qubits:** linear optics, measurement-based and continuous-variable approaches
- **Spin qubits:** semiconductor quantum dots (overview)
- **Topological qubits:** status and open questions (overview)

### 8.2 Qubit performance metrics
- $T_1$, $T_2$, and $T_2^*$
- Gate fidelity and randomised benchmarking
- Readout fidelity and crosstalk
- Quantum volume and other benchmarks

### 8.3 Cryogenics
- Why superconducting qubits need millikelvin temperatures
- Cryostats and dilution refrigerators (principle of operation)
- Pulse-tube coolers and cryogen-free systems
- Thermal budget, heat loads, and wiring stages (4 K, 800 mK, 100 mK, 10 mK)
- Helium-3 supply and its constraints

### 8.4 Microwave and control electronics
- Arbitrary waveform generators (AWGs) and digital-to-analogue conversion
- Readout chains: amplifiers (HEMT, JPA), mixers, digitisers
- FPGAs for real-time control and feedback
- Attenuators, filters, and thermal anchoring of cables

### 8.5 Calibration
- Frequency and amplitude calibration of pulses
- Drift and automatic recalibration
- Calibration scheduling as an operations task

### 8.6 Facility requirements
- Power (peak and steady-state), cooling water, air-conditioning constraints
- Floor loading, vibration, magnetic field shielding
- Environmental monitoring (temperature, humidity, sound)
- Site survey process (see LRZ paper below)

## Materials

### Free
- **IBM Quantum Learning**, *Use a quantum computer today* (Olivia Lanes). Covers the hardware and calibration basics from the user side.
- **IBM Quantum Learning**, *Quantum computing in practice* (covers hardware noise and mapping)
- **Krinner et al.**, "Engineering cryogenic setups for 100-qubit scale superconducting circuit systems", EPJ Quantum Technology, 2019 (free on arXiv or the journal site). The main free reference for cryogenic wiring.
- **arXiv:2509.12949**, "First Practical Experiences Integrating Quantum Computers with HPC Resources" (LRZ and IQM, 2025). Read this in full; it covers site survey, utilities, and daily operations.
- **Qblox** and **Quantum Machines** documentation (control electronics architectures; free to read)
- **Schuster**, *Circuit QED* thesis or review papers (free on arXiv). Background on superconducting qubits.

### Textbooks
- **Pobell**, *Matter and Methods at Low Temperatures* (Springer, 3rd ed.). Standard reference for cryogenics.
- **Krantz et al.**, "A Quantum Engineer's Guide to Superconducting Qubits" (Applied Physics Reviews, 2019; free on arXiv). Best single review for engineers.
- **Gambetta**, lecture notes and reviews on superconducting qubit control (search arXiv)

### Paid (optional)
- Vendor training courses from IQM, Quantum Machines, or Qblox (check with the vendor; many are offered to customers and partners)

## Milestones (self-check)

- [ ] List the main qubit modalities and one advantage and one limitation of each
- [ ] Explain $T_1$ and $T_2$ and how each is measured in principle
- [ ] Describe the wiring stages of a dilution refrigerator and why attenuators are placed at each stage
- [ ] Estimate the power and cooling requirements of a superconducting QPU from the LRZ paper
- [ ] Explain why readout chains use cryogenic amplifiers

## Connection to your HPC background

Facility work is where HPC experience transfers most directly. The LRZ paper shows that quantum computers need cooling water, power planning, environmental monitoring, and scheduler-driven recalibration. Your experience with these topics on classical clusters gives you an advantage over candidates who only know physics.
