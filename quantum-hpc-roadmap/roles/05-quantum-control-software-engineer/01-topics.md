# Role 5: Topics

## 1. Pulse fundamentals
- Pulse shapes (Gaussian, DRAG, flat-top) and their spectra
- Carrier frequency, envelope, phase, and amplitude
- Rabi pulses, $\pi$ and $\pi/2$ pulses, and how they map to gates
- Virtual Z gates (phase tracking in software)

## 2. Waveform generation
- Arbitrary waveform generators (AWGs): sampling rate, resolution, memory
- Digital up-conversion and mixers
- Sequencing: waveform tables, triggers, and timing
- Phase coherence across channels

## 3. Readout and acquisition
- Readout pulses and resonator response
- Digitisers and demodulation (IQ data)
- Integration windows and discrimination
- Real-time signal processing on FPGAs

## 4. FPGA and real-time control
- FPGA basics: logic, clocks, and fixed-latency pipelines
- Real-time feedback (conditional gates based on measurement)
- Latency budgets and deterministic timing
- Firmware interfaces and version control for firmware

## 5. Control software architecture
- Experiment description languages (sequences, sweeps, parameters)
- Compilation from circuits to pulse schedules
- Device abstraction layers and hardware drivers
- APIs for calibration and user tools

## 6. Optimal control and pulse design
- Gradient-based pulse optimisation (GRAPE, overview)
- Robust pulses against detuning and amplitude errors
- Adiabatic pulses and their limits
- Pulse-level simulation of qubit dynamics

## 7. Testing and reliability
- Hardware-in-the-loop testing and simulators for control software
- Regression testing of pulse sequences
- Logging and traceability for experiments
- Versioning of calibration results

## 8. Quantum concepts that drive control design
- Bandwidth and sampling limits on pulse shapes
- Leakage to non-computational levels in transmons
- Crosstalk between control lines
- Decoherence during pulses (pulse length versus T2)

## Tools to learn
- Python (advanced), C or C++ (for drivers and performance-critical code)
- Pulse-level control: Qiskit Pulse was removed in Qiskit 2.0, so use Qiskit Dynamics for pulse simulation, vendor control SDKs (e.g., Qblox, Quantum Machines), and CUDA-Q for pulse-level hybrid work
- Vendor SDKs for AWG and control stacks (Qblox, Quantum Machines), where available
- Verilog or VHDL basics (for FPGA-focused roles)
- Linux drivers and real-time concepts (for hardware interfaces)
