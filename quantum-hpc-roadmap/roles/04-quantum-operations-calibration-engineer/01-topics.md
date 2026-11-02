# Role 4: Topics

## 1. Qubit characterisation experiments
- Resonator and qubit spectroscopy (finding frequencies)
- Rabi experiments (pulse amplitude calibration)
- Ramsey experiments (frequency fine-tuning, $T_2^*$)
- Echo experiments (T2 echo)
- $T_1$ relaxation experiments
- Readout calibration and discrimination thresholds

## 2. Gate calibration
- Single-qubit gate calibration (DRAG pulses, amplitude and phase)
- Two-qubit gate calibration (cross-resonance, CZ, iSWAP, depending on platform)
- Randomised benchmarking and interleaved randomised benchmarking
- Gate fidelity and how it is reported

## 3. Drift and monitoring
- Time series of qubit parameters and their statistics
- Detecting drift and deciding when to recalibrate
- Calibration age as a scheduling metric
- Correlating drift with environmental data (temperature, power, vibration)

## 4. Automation and scheduling
- Calibration graphs and dependencies between steps
- Scheduling calibration as Slurm or workflow jobs
- Balancing calibration time against user demand
- Rollback when a calibration produces worse results

## 5. Data analysis
- Curve fitting (exponential decay, sinusoidal fits)
- Error bars and confidence intervals
- Outlier handling and quality checks
- Plotting and reporting for engineers and users

## 6. Operations and incident response
- Runbooks for failed calibrations and degraded qubits
- Escalation to vendors and internal engineers
- Post-incident analysis and records
- Communicating qubit availability to users

## 7. Quantum concepts that drive operations
- What $T_1$, $T_2$, and fidelity mean physically
- Why small frequency errors cause large gate errors
- Crosstalk and why neighbouring qubits are calibrated together
- Measurement error and its effect on results

## Tools to learn
- Python (fitting with NumPy and SciPy)
- Qiskit Experiments or similar calibration tooling (check current documentation)
- Vendor control-stack interfaces (for example, Qblox or Quantum Machines SDKs, where available)
- Grafana or equivalent dashboards for time series
- Slurm or workflow engines for scheduled calibration
