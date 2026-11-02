# Role 4: Milestones and Portfolio

## Milestones (self-check)
- [ ] Describe what a Rabi experiment measures and how it sets the pulse amplitude
- [ ] Explain the difference between $T_1$, $T_2$, and $T_2^*$ in terms of the physical process behind each
- [ ] Explain why a Ramsey experiment is sensitive to frequency error, and what the decay envelope tells you
- [ ] Describe the steps of a calibration graph for a single qubit, from spectroscopy to randomised benchmarking
- [ ] Explain why calibration age affects user-visible fidelity
- [ ] Describe how you would detect drift in a qubit frequency from a time series
- [ ] Write a runbook entry for a qubit whose readout fidelity drops below a set threshold

## Portfolio projects
1. **Calibration analysis notebook:** fit a Rabi and a Ramsey experiment (simulated or from the Open Plan) and report the fitted parameters with error bars.
2. **Drift detector:** a script that reads a time series of qubit frequencies and flags when recalibration is needed. Test it on synthetic drift.
3. **Scheduled calibration:** a Slurm or workflow job that runs a short calibration sequence and writes results to a database.
4. **Qubit health dashboard:** Grafana panels for T1, T2, readout fidelity, and calibration age, using simulated data.
5. **Operations runbook:** procedures for a qubit that fails calibration, a degraded two-qubit gate, and a calibration that overruns its window.

## Interview preparation
- **Analysis:** you are given a decay curve with noise. Fit it, give the parameter and its error, and say what you would check next.
- **Operations:** a user reports a job failing on Qubit 7. Walk through the diagnostic steps and the decision to recalibrate or exclude the qubit.
- **Trade-offs:** how often do you recalibrate? What do you lose by calibrating too often, and what do you lose by not calibrating often enough?
- **Physics basics:** explain $T_1$ and $T_2$, and what affects each.

## Application checklist
- [ ] CV section "Quantum Operations and Calibration" with the analysis and dashboard projects
- [ ] Public notebooks with clear explanations and error analysis
- [ ] Apply to calibration and operations roles at Q-CTRL, QPU vendors, and quantum labs at universities and national labs
