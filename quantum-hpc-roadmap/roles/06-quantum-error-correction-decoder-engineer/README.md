# Role 6: Quantum Error Correction and Real-Time Decoder Engineer

## What the role does

Builds the software and hardware that decode error syndromes from a quantum processor in real time. Works on decoder algorithms (for example, minimum-weight perfect matching and union-find), their implementation on GPUs and FPGAs, latency and throughput, and the integration with the control stack.

NVIDIA's CUDA-Q QEC and its real-time decoding work, and NVQLink (announced October 2025; the cudaq-realtime API was released at GTC 2026), are examples of this area. The work is a streaming, latency-bound HPC problem, which is one of the closest matches in quantum computing to your background.

## Physics depth required: Working to Deep (QEC theory)

You need to understand stabiliser codes, syndromes, logical errors, and the threshold. You need enough algebra to read decoder papers. You do not need full fault-tolerance theory unless you aim for research.

| General phase | Depth | Why |
|---|---|---|
| [00 Math refresh](../../general/00-math-and-physics-refresh.md) | Working | Linear algebra over binary fields (overview) |
| [01 Wave mechanics](../../general/01-wave-mechanics.md) | Conceptual | Background |
| [02 Formalism](../../general/02-formalism-hilbert-space.md) | Working | Pauli operators and stabilisers |
| [03 Angular momentum and spin](../../general/03-angular-momentum-spin-atoms.md) | Conceptual | Spin-½ and Pauli matrices |
| [04 Approximations](../../general/04-approximations-and-time-dependence.md) | Conceptual | Why noise rates matter |
| [05 Open systems](../../general/05-many-body-scattering-open-systems.md) | Working | Noise and error models |
| [06 Quantum information](../../general/06-quantum-information-and-algorithms.md) | Deep | Gates, Clifford group, encoding |
| [07 Error correction](../../general/07-quantum-error-correction.md) | Deep | Core job |
| [08 Hardware and cryogenics](../../general/08-quantum-hardware-and-cryogenics.md) | Conceptual | Readout latency and data rates |
| [09 Software and simulation](../../general/09-quantum-software-and-simulation.md) | Deep | Stim, CUDA-Q QEC, simulators |
| [10 Quantum–HPC integration](../../general/10-quantum-hpc-integration.md) | Deep | Real-time data paths |

## Files in this role

- [01-topics.md](01-topics.md): skills and subtopics to master
- [02-materials.md](02-materials.md): free and paid resources
- [03-milestones-and-portfolio.md](03-milestones-and-portfolio.md): self-checks, projects, interview preparation

## Suggested timeline

About 6–9 months at 12–15 hours a week. QEC theory is the longest part; the GPU and latency work will feel familiar.
