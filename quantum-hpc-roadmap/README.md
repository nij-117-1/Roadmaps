# Quantum–HPC Roadmap (Index)

This folder has two parts:

1. **[general/](general/README.md)**: the general quantum mechanics and quantum engineering roadmap (12 files, Phases 0–11). Start here if you are new to quantum.
2. **[roles/](roles/)**: role-specific roadmaps. Each role uses the general phases at a different depth, plus its own topics, materials, and milestones.

## Role roadmaps

| # | Role | Physics depth | Best fit for |
|---|---|---|---|
| 1 | [Quantum–HPC Systems Engineer](roles/01-quantum-hpc-systems-engineer/README.md) | Working | Slurm, GPU clusters, platform operations (closest to your current job) |
| 2 | [Quantum Orchestration Software Engineer](roles/02-quantum-orchestration-software-engineer/README.md) | Working to deep | Python and C++ workflow and API engineering |
| 3 | [Quantum Facility and Infrastructure Engineer](roles/03-quantum-facility-infrastructure-engineer/README.md) | Working on hardware | Data-centre, power, cooling, and cryogenic facilities |
| 4 | [Quantum Operations and Calibration Engineer](roles/04-quantum-operations-calibration-engineer/README.md) | Working | Monitoring, calibration automation, and incident response |
| 5 | [Quantum Control Software Engineer](roles/05-quantum-control-software-engineer/README.md) | Working to deep | Pulses, AWGs, FPGAs, and real-time control |
| 6 | [Quantum Error Correction and Decoder Engineer](roles/06-quantum-error-correction-decoder-engineer/README.md) | Working to deep | Real-time decoding, GPU and FPGA performance |

Each role folder has four files: `README.md` (overview and depth map), `01-topics.md`, `02-materials.md`, and `03-milestones-and-portfolio.md`.

## Choosing a role

- **Stay close to your current work:** Role 1 (Systems Engineer) or Role 4 (Operations).
- **Move toward software:** Role 2 (Orchestration) or Role 6 (Decoder), both of which use GPUs heavily.
- **Move toward hardware and facilities:** Role 3 (Facility) or Role 5 (Control).

Start with the general roadmap's Phases 0–2 whatever role you pick. All six roles share that foundation.

## Shared foundation (all roles)

Before any role-specific work, complete:
- [general/00-math-and-physics-refresh.md](general/00-math-and-physics-refresh.md)
- [general/01-wave-mechanics.md](general/01-wave-mechanics.md)
- [general/02-formalism-hilbert-space.md](general/02-formalism-hilbert-space.md)

Then go to the role-specific depth table in each role's README.

## Notes

- Certification prices and exam versions change. Check the provider's website before you enrol.
- Some tools and vendor offerings change quickly (for example, CUDA-Q releases; Qiskit Pulse was removed in Qiskit 2.0). Check current documentation for any tool before you rely on it.
