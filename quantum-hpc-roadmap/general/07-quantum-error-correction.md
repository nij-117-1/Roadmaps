# Phase 7: Quantum Error Correction

**Duration:** 4 weeks
**Goal:** Understand how quantum information is protected from noise, how codes are built and decoded, and why real-time classical decoding is an HPC problem.

## Topics and subtopics

### 7.1 Noise and errors
- Pauli errors (bit flip, phase flip, combined)
- Depolarising and amplitude-damping noise
- Error models used in hardware benchmarking

### 7.2 Classical error correction (review)
- Repetition code and majority voting
- Linear codes, parity checks, syndromes

### 7.3 Quantum codes
- Shor's 9-qubit code (historical)
- Steane 7-qubit code
- Stabiliser formalism: stabiliser groups, logical operators, syndromes
- CSS codes

### 7.4 Fault tolerance
- Threshold theorem (overview)
- Fault-tolerant gates and magic-state distillation (overview)
- Transversal gates

### 7.5 Surface code
- Lattice layout, data and ancilla qubits
- Syndrome extraction cycles
- Logical error rate and code distance
- Decoding: minimum-weight perfect matching (MWPM) and union-find (overview)

### 7.6 Decoding as a real-time HPC problem
- Latency budgets for decoding (microseconds)
- Data rates from readout hardware
- Decoder hardware: GPUs, FPGAs, and ASICs
- Neural-network decoders (overview)

## Materials

### Free
- **IBM Quantum Learning**, *Foundations of quantum error correction* (John Watrous). Free, with exercises.
- **NVIDIA CUDA-Q Academic**, *Quantum Error Correction 101* module (GitHub: `NVIDIA/cuda-q-academic/qec101`). Covers classical and quantum codes, decoders, and magic-state distillation.
- **CUDA-Q QEC documentation** (nvidia.github.io/cuda-quantum), including the QEC 101 learning path
- **Gottesman**, *Stabilizer Codes and Quantum Error Correction* (PhD thesis, arXiv quant-ph/9705052, free). Standard reference for the stabiliser formalism.
- **Preskill's Ph219 notes**, Chapter 7 (quantum error correction; free PDF)
- **Stim** (Google, open source): fast stabiliser circuit simulator. Documentation and tutorials are free.

### Textbooks
- **Lidar & Brun** (eds.), *Quantum Error Correction* (Cambridge, 2013). Advanced reference with chapters by many experts.
- **Nielsen & Chuang**, Chapter 10 (quantum error correction)

### Papers (free on arXiv)
- Fowler et al., "Surface codes: Towards practical large-scale quantum computation" (Physical Review A, 2012)
- Any recent NVIDIA or industry paper on real-time QEC decoding (search arXiv for "real-time decoding GPU quantum error correction"; reading two or three will keep you current)

## Milestones (self-check)

- [ ] Write the stabilisers of the 3-qubit repetition code and explain how a syndrome identifies a bit-flip error
- [ ] Explain why a logical operator must commute with all stabilisers but not be in the stabiliser group
- [ ] Describe the surface-code syndrome cycle in words, including what ancilla qubits measure
- [ ] Explain the threshold theorem in one paragraph
- [ ] Estimate the decoding data rate for a surface-code patch of a given distance and cycle time

## Connection to your HPC background

Real-time decoding of surface-code syndromes is a streaming, latency-bound workload: data arrives from readout hardware, and a decision must be made within a fixed time window. This is the closest match in quantum computing to HPC systems work you already do (streaming pipelines, GPU scheduling, latency tuning). It is also a strong differentiator for your career.
