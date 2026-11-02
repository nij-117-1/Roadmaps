# Role 1: Milestones and Portfolio

## Milestones (self-check)
- [ ] Explain the lifecycle of a hybrid job from submission to results, naming each system involved
- [ ] Configure a Slurm partition that accepts simulator GPU jobs and an accounting report for them
- [ ] Explain why state-vector memory doubles with each added qubit, and size a GPU for 30 qubits
- [ ] Describe the latency budget for a feedback loop and which network path it uses
- [ ] Write a site-readiness checklist for a new QPU (power, cooling, network, floor, environment)
- [ ] Describe, without notes, the difference between a simulator and a QPU for scheduling purposes
- [ ] Explain to a non-physicist what "calibration age" means and why it affects queueing

## Portfolio projects
1. **Simulator cluster:** Slurm partition plus Apptainer image for CUDA-Q and Qiskit Aer. Document the setup and submit benchmark jobs.
2. **Benchmark suite:** scripts that run state-vector simulations at increasing qubit counts and report time, memory, and GPU utilisation.
3. **Hybrid job example:** a variational loop that alternates between a GPU simulator and an optimiser, scheduled as dependent Slurm jobs.
4. **Monitoring dashboard:** Grafana panels for queue wait, GPU utilisation, and mock QPU calibration age.
5. **Facility runbook:** a document for a QPU recalibration or maintenance event (who is notified, what is checked, rollback steps).

## Interview preparation
- **Systems design:** design a quantum–GPU platform for 20 users with mixed simulator and QPU demand. Be ready to justify partitions, quotas, and network layout.
- **Troubleshooting:** a simulator job fails only on certain nodes; a QPU queue is stuck; a calibration job overran its window. Practise the diagnostic steps.
- **Quantum fundamentals:** explain superposition, entanglement, and decoherence in two minutes each, in plain language.
- **Vendor questions:** be ready to discuss how you would evaluate a vendor's site-readiness report or integration plan.

## Application checklist
- [ ] CV section titled "Quantum–HPC Systems" with Slurm, GPU, and integration projects
- [ ] GitHub repository with the portfolio projects and clear READMEs
- [ ] Apply to senior and mid-level roles (NVIDIA, D-Wave, IonQ, Quantinuum, and university or national lab centres)
