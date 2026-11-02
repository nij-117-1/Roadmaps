# Phase 11: Certifications, Portfolio, Research, and Career

**Duration:** Ongoing (start the portfolio in Phase 6; apply after Phase 10)
**Goal:** Turn your learning into credentials, public evidence of skill, and a job offer. Also build the habit of reading current research, which is what separates top practitioners from the rest.

## 11.1 Certifications

Prioritise the first two. Check current prices and exam versions on the provider's website before you enrol.

| Certification | Provider | Type | Fit |
|---|---|---|---|
| **IBM Certified Quantum Computation using Qiskit v2.X Developer, Associate** | IBM | Paid, $200 USD per attempt (exam C1000-179: 68 questions, 90 minutes, 47 to pass; a $30 practice exam is optional) | Strong, widely recognised. Recommended first. |
| **MITx 8.04x** verified certificate | MIT via edX | Paid verified track (audit is free) | Strong physics credential; matches your QM goal |
| **IBM Quantum Learning course badges** | IBM | Free (completion badges on some courses) | Good for showing progress on your profile |
| **NVIDIA certifications** (general AI and infrastructure tracks) | NVIDIA | Paid | Relevant for GPU-heavy quantum–HPC roles. No quantum-specific NVIDIA certification is currently listed; check the NVIDIA certification page for new tracks. |
| **Relevant HPC certifications** you may already hold or consider | Vendors and HPC training providers | Varies | Strengthens the HPC-side story |

**Practical order:** IBM course badges (free) → MITx 8.04x → IBM Qiskit Developer Associate → NVIDIA certification if your target employer uses NVIDIA.

## 11.2 Portfolio (build as you go)

Publish each item on GitHub with a README that explains the problem, method, and results.

1. **Simulator benchmark suite (Phase 9):** Slurm-submitted state-vector runs; time, memory, and scaling plots.
2. **1D time-dependent Schrödinger solver (Phase 1):** CPU and GPU versions with a speedup study.
3. **Rabi-oscillation and pulse simulator (Phase 4):** shows you understand time-dependent control.
4. **Surface-code decoder or stabiliser simulation (Phase 7):** a small Stim or CUDA-Q QEC example with a threshold plot.
5. **Quantum–HPC operations package (Phase 10):** a Slurm configuration for simulator and QPU jobs, a runbook, and a Grafana dashboard with simulated metrics.
6. **Literature review:** a two-page summary of one current paper per month (see 11.3).

## 11.3 Research habits (for top-1% depth)

- **Read arXiv quant-ph** every week. Start with the listings, read abstracts, then read two or three papers in full each month.
- **Reproduce one published result** per quarter. Pick a simple simulation or benchmark from a paper and reproduce the main figure.
- **Keep a derivation journal.** Re-derive standard results without notes every month.
- **Join a community.** Quantum computing Discord and Slack groups, IBM Quantum community forums, and the Qiskit and CUDA-Q GitHub discussions.
- **Attend one talk or workshop per quarter.** Conferences like IEEE Quantum Week (QCE) and SC (for quantum-HPC) are the most relevant.

## 11.4 Career targets

| Role | Fit for you | Typical employers |
|---|---|---|
| Quantum–HPC systems engineer | Strongest fit | NVIDIA, D-Wave, IonQ, Quantinuum (check current listings) |
| Quantum–HPC orchestration / software engineer | Strong fit | Quantinuum and similar |
| Quantum infrastructure and facility engineer | Strong fit | QPU vendors, national labs, university centres |
| Quantum operations / calibration engineer | Good fit | Q-CTRL and QPU vendors |
| Quantum control software engineer | Good fit, needs Phase 8 depth | Quantum Machines, Qblox |

Some senior quantum job postings ask for extensive HPC experience, often 10 years or more. Target mid-level or lead roles first, and emphasise your Slurm and GPU cluster experience with the portfolio items above.

## 11.5 Application checklist

- [ ] Update your CV with a "Quantum–HPC" section that lists Slurm, GPU, and QPU-related projects
- [ ] Add the portfolio links and certifications to LinkedIn and GitHub
- [ ] Apply to 3–5 roles per week, prioritising the job boards quantumcareers.com, quantumjobslist.com, and vendor career pages
- [ ] Ask for informational calls with engineers at two or three quantum companies
- [ ] Prepare for two interview tracks: systems design (Slurm, GPU, latency) and physics fundamentals (Phases 1–7)

## 11.6 Milestones for the full roadmap

- [ ] Can solve and explain standard QM problems from Phases 1–5 without notes
- [ ] Can implement and explain core quantum algorithms (Phase 6) in Qiskit and CUDA-Q
- [ ] Can size and run a state-vector simulation as a Slurm GPU job and report scaling results
- [ ] Has a published portfolio with at least four items from 11.2
- [ ] Holds at least one recognised certification (IBM Qiskit Developer Associate recommended)
- [ ] Can explain a quantum-HPC integration design end to end in an interview
