# Phase 9: Quantum Software and Simulation

**Duration:** 5–6 weeks (run in parallel with Phases 6–8)
**Goal:** Write, run, and profile quantum programs on simulators and real hardware. Learn both major software stacks for quantum–HPC work: Qiskit and CUDA-Q.

## Topics and subtopics

### 9.1 Python for quantum (review)
- NumPy, SciPy, and Jupyter
- Complex arithmetic and matrix operations in NumPy
- Writing reproducible notebooks and scripts

### 9.2 Qiskit fundamentals
- Circuits, registers, gates, and measurements
- Transpilation and backend-specific optimisation
- Simulators: Aer (statevector, density matrix, noise models)
- Running on real hardware through IBM Quantum (Qiskit Runtime primitives: Sampler and Estimator)

### 9.3 CUDA-Q fundamentals
- Kernels, quantum programs in Python and C++
- Targets: CPU simulation, GPU simulation (state vector and tensor network), and QPU backends
- Multi-GPU and MPI-based simulation
- cuQuantum integration for accelerated tensor operations

### 9.4 Simulation methods
- State-vector simulation: memory scales as $2^n$
- Density-matrix simulation: memory scales as $4^n$
- Tensor-network simulation (MPS and related methods)
- Stabiliser simulation (Gottesman–Knill theorem; Stim)
- Trajectory and noise sampling methods (PTSBE, overview)

### 9.5 Performance and profiling
- Benchmarking simulators: time, memory, and scaling with qubit count
- Profiling GPU kernels (Nsight Systems and Nsight Compute, overview)
- Batching shots and parameter sweeps

### 9.6 Variational workflows
- Parameterised circuits and cost functions
- Classical optimisers (COBYLA, SPSA, gradient-based)
- Running variational loops across CPU and GPU

### 9.7 Hybrid and workflow tools
- Qiskit Runtime sessions and batching
- CUDA-Q hybrid workflows
- Orchestrating classical and quantum steps (preview of Phase 10)

## Materials

### Free (primary)
- **IBM Quantum Learning**, *Introduction to quantum computing with Qiskit* (openHPI / IBM, free)
- **IBM Quantum Learning**, *Quantum chemistry with VQE* (free introductory VQE course)
- **IBM Quantum Learning**, *Quantum machine learning* (free, about 10 hours)
- **Qiskit documentation** (docs.quantum.ibm.com) and **Qiskit tutorials** (free, updated frequently)
- **NVIDIA CUDA-Q Academic** (GitHub: `NVIDIA/cuda-q-academic`). Modules: Quantum Algorithm Simulation 101, Quantum Information Science Examples, Dynamics 101, AI for Quantum, Chemistry Simulations.
- **CUDA-Q documentation and applications** (nvidia.github.io/cuda-quantum), including Shor, UCCSD, MPS encoding, Trotter simulation, and PTSBE
- **QuREKA CUDA-Q Academic** (free starter points for running CUDA-Q in the cloud; check current availability)
- **Qiskit Aer and cuQuantum** documentation

### Free (community)
- **Monit Sharma, The Quantum Classroom** (open learning space; Qiskit path and circuit playground)

### Textbooks
- **Nielsen & Chuang** (Chapter 4 on quantum circuits) for the theory behind the software
- **Bergholm et al.** or **Wong**, *Quantum Computing: An Applied Approach* (Springer, 2nd ed.). Practical, code-driven.

### Paid (optional)
- IBM Quantum paid plans for higher QPU runtime (the free Open Plan is enough to start)
- Vendor cloud credits (check current programmes)

## Milestones (self-check)

- [ ] Build a 3-qubit GHZ circuit in Qiskit, run it on a simulator, and explain the measured distribution
- [ ] Write the same circuit as a CUDA-Q kernel and run it on a CPU and a GPU target (if available)
- [ ] Measure how state-vector simulation time changes as you increase the number of qubits from 20 to 30 on one GPU
- [ ] Write a variational loop (for example, a two-qubit VQE) and show that the optimiser converges
- [ ] Explain why Stim can simulate Clifford circuits with thousands of qubits but a state-vector simulator cannot

## Connection to your HPC background

This is the phase where your background is most direct. Treat simulators as HPC applications:
- Submit state-vector simulations as Slurm jobs with `--gres=gpu:N` and record time-to-solution.
- Use `srun` or MPI for multi-GPU runs.
- Build a benchmark suite that reports qubits, depth, time, and memory per job.

The results become portfolio material for Phase 11.
