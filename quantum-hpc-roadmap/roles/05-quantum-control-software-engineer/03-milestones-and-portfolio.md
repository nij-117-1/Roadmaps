# Role 5: Milestones and Portfolio

## Milestones (self-check)
- [ ] Explain why a Gaussian pulse has a limited bandwidth and what that means for pulse length
- [ ] Describe how a DRAG pulse reduces leakage to the third level of a transmon
- [ ] Explain how a virtual Z gate is implemented and why it has no physical duration
- [ ] Describe the steps from a circuit description to an AWG waveform
- [ ] Explain the latency budget of a conditional gate that depends on a measurement
- [ ] Describe what GRAPE optimises and what its main practical limitation is
- [ ] Explain the trade-off between pulse length and decoherence

## Portfolio projects
1. **Pulse simulator:** a single-qubit simulator that applies a shaped pulse and reports the final state fidelity under a detuning error.
2. **Pulse library:** a small set of parameterised pulses (Gaussian, DRAG, flat-top) with tests for amplitude, area, and spectral content.
3. **Sequence compiler:** a small tool that turns a list of gates into a timed pulse schedule with phase tracking.
4. **Readout analysis:** a script that demodulates synthetic IQ data and computes a discrimination threshold.
5. **Hardware-in-the-loop test:** a test harness that runs a sequence on a control stack or emulator and checks the results against expected values.

## Interview preparation
- **Coding:** write a function that generates a DRAG pulse from a set of parameters, with unit tests.
- **Systems:** design a control system for a 16-qubit device with per-qubit AWG channels and shared readout. Discuss latency and synchronisation.
- **Physics:** explain why a pulse that is too short causes leakage, and why one that is too long causes decoherence.
- **Debugging:** a sequence works in simulation but gives a shifted phase on hardware. What do you check first?

## Application checklist
- [ ] Public repositories with pulse-level tools and tests
- [ ] CV section "Quantum Control Software" with the pulse and sequencing projects
- [ ] Apply to control software roles at Quantum Machines, Qblox, and QPU vendors
