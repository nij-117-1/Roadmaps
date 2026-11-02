# Quantum Mechanics & Quantum Engineering Roadmap (HPC Administrator → Quantum Engineer)

**Starting point:** HPC administrator (Slurm, GPU clusters), undergraduate physics completed years ago.
**Target:** Deep, working command of quantum mechanics and quantum information, plus the ability to build and operate quantum–HPC systems.

## How to use this roadmap

- Work through the phase files in order. Each one lists topics, subtopics, materials (free and paid), milestones, and how it connects to your HPC background.
- Milestones are self-checks. Do not move on until you can explain each one without notes.
- Keep a notebook (paper or digital). Derive every key result by hand at least once.
- Pair every physics phase with the matching software phase. Physics without code, or code without physics, stalls.

## Honest expectations

"Top 1%" in quantum mechanics means depth, not just coverage: deriving results from first principles, solving unfamiliar problems, and reading research papers without help. This roadmap gets you there in stages:

| Stage | Duration (approx.) | Outcome |
|---|---|---|
| Foundations (Phases 0–2) | 3–4 months | Solid QM formalism, can solve standard 1D and spin problems |
| Core QM and approximations (Phases 3–4) | 3–4 months | Can handle perturbation theory, angular momentum, hydrogen-like systems |
| Quantum information and QEC (Phases 5–6) | 3–4 months | Can implement and analyse quantum algorithms and codes |
| Hardware, software, and HPC integration (Phases 7–9) | 3–4 months | Can design and operate a quantum–HPC platform |
| Research depth and career (Phases 10–11) | Ongoing | Reads current papers, contributes to projects, applies for roles |

Total: about **12–18 months** at 12–15 hours per week. Top-1% depth typically comes after several more years of research-level practice; this roadmap gives you the foundation and the habits that make that possible.

## Weekly time split (suggested)

- **Theory (physics / math):** 6–8 hours
- **Code (IBM Qiskit, CUDA-Q, simulation):** 3–4 hours
- **HPC-applied work (Slurm, GPU, scheduler integration):** 2–3 hours
- **Review and self-testing:** 1 hour

## Phase index

| File | Topic | Core? |
|---|---|---|
| [00-math-and-physics-refresh.md](00-math-and-physics-refresh.md) | Linear algebra, complex analysis, ODEs, classical mechanics | Yes |
| [01-wave-mechanics.md](01-wave-mechanics.md) | Wavefunctions, Schrödinger equation, 1D problems | Yes |
| [02-formalism-hilbert-space.md](02-formalism-hilbert-space.md) | Kets, operators, measurement, dynamics | Yes |
| [03-angular-momentum-spin-atoms.md](03-angular-momentum-spin-atoms.md) | Angular momentum, spin, hydrogen atom | Yes |
| [04-approximations-and-time-dependence.md](04-approximations-and-time-dependence.md) | Perturbation theory, variational, WKB, time-dependent problems | Yes |
| [05-many-body-scattering-open-systems.md](05-many-body-scattering-open-systems.md) | Identical particles, scattering, density matrices, decoherence | Yes |
| [06-quantum-information-and-algorithms.md](06-quantum-information-and-algorithms.md) | Qubits, entanglement, gates, algorithms | Yes |
| [07-quantum-error-correction.md](07-quantum-error-correction.md) | Stabilizer codes, surface code, decoding | Yes |
| [08-quantum-hardware-and-cryogenics.md](08-quantum-hardware-and-cryogenics.md) | Qubit modalities, cryogenics, control electronics | Engineering |
| [09-quantum-software-and-simulation.md](09-quantum-software-and-simulation.md) | Qiskit, CUDA-Q, simulators, cuQuantum | Engineering |
| [10-quantum-hpc-integration.md](10-quantum-hpc-integration.md) | Scheduling, orchestration, monitoring, facilities | Your strength |
| [11-certifications-career-and-research.md](11-certifications-career-and-research.md) | Certifications, portfolio, papers, job targets | Career |

## Quick-start for the first week

1. Set up Python, Jupyter, Qiskit, and CUDA-Q (or Docker image for CUDA-Q).
2. Create an IBM Quantum account (free Open Plan) and start *Basics of Quantum Information and Computation* on IBM Quantum Learning.
3. Start MIT OCW 18.06 (Strang linear algebra) or 3Blue1Brown's *Essence of Linear Algebra* for a quick visual refresher.
4. Open a notebook and write down, in your own words, what a qubit is and what measurement does.
