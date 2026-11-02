# Phase 6: Quantum Information and Algorithms

**Duration:** 5–6 weeks
**Goal:** Use the QM formalism to understand qubits, entanglement, quantum gates, and the main quantum algorithms. This is where physics becomes computation.

## Topics and subtopics

### 6.1 Qubits and quantum states
- Single-qubit states, Bloch sphere, global phase
- Multi-qubit states, tensor products, computational basis

### 6.2 Quantum gates and circuits
- Pauli gates, Hadamard, phase gates (S, T), rotation gates
- Controlled gates (CNOT, CZ), Toffoli
- Universal gate sets; the Solovay–Kitaev theorem (overview)
- Circuit model and circuit depth

### 6.3 Entanglement
- Bell states and maximally entangled states
- Schmidt decomposition
- Entanglement entropy (von Neumann)
- Bell inequalities and the CHSH inequality

### 6.4 Quantum protocols
- No-cloning theorem
- Quantum teleportation
- Superdense coding
- Quantum key distribution (BB84, overview)

### 6.5 Quantum measurements and information
- Projective and general measurements
- Quantum state discrimination and tomography
- Fidelity and trace distance
- Holevo bound (overview)

### 6.6 Quantum algorithms
- Deutsch and Deutsch–Jozsa
- Simon's algorithm
- Quantum Fourier transform (QFT)
- Quantum phase estimation
- Shor's factoring algorithm
- Grover's search and amplitude amplification

### 6.7 Variational and near-term algorithms (overview)
- Variational quantum eigensolver (VQE)
- Quantum approximate optimisation algorithm (QAOA)
- Quantum machine learning (overview)

### 6.8 Complexity (overview)
- BQP and its relation to BPP and NP
- Query complexity

## Materials

### Free (primary)
- **IBM Quantum Learning**, *Basics of quantum information and computation* (John Watrous). Covers single and multiple systems, Qiskit implementation.
- **IBM Quantum Learning**, *Fundamentals of quantum algorithms* (Deutsch, Deutsch–Jozsa, Simon, Grover, Shor, phase estimation)
- **IBM Quantum Learning**, *General formulation of quantum information* (density matrices, channels, fidelity)
- **IBM Quantum Learning**, *Quantum diagonalization algorithms* and *Variational algorithm design*
- **Preskill's Caltech Ph219 notes**, Chapters 1–5 and 7 (free PDF; Chapter 10 on quantum Shannon theory was updated in June 2025)
- **Nielsen & Chuang solutions** (community-maintained online; use only after you have attempted the problem yourself)
- **Monit Sharma, The Quantum Classroom** (free open resources; reference only)
- **Qiskit Textbook** (archived; use for older examples but check the current IBM Learning content first)

### Textbooks
- **Nielsen & Chuang**, *Quantum Computation and Quantum Information* (10th Anniversary Edition, Cambridge 2010). Primary textbook for this phase.
- **Mermin**, *Quantum Computer Science* (Cambridge, 2007). Shorter, more theory-focused.
- **Kitaev, Shen & Vyalyi**, *Classical and Quantum Computation* (AMS, 2002). Advanced, for the mathematical depth.

### Courses (free video)
- **Daniel Gottesman's** lectures on quantum information (online)
- **Berkeley CS191 / CS294** lecture notes (search for current versions)
- **Oxford Hilary Term 2025** Quantum Information course notes (free online; course page: cs.ox.ac.uk)

## Milestones (self-check)

- [ ] Write the state of a Bell pair, compute its reduced density matrix, and show it is maximally mixed
- [ ] Explain why the no-cloning theorem follows from linearity of quantum evolution
- [ ] Derive the action of the Hadamard gate on $|0\rangle$ and $|1\rangle$ and explain interference in Deutsch's algorithm
- [ ] Explain the role of the QFT in phase estimation and why it leads to Shor's algorithm
- [ ] Describe the difference between a unitary gate and a measurement in the circuit model

## Connection to your HPC background

State-vector simulation memory grows as $2^n$. A GPU with 80 GB of memory can hold a complex state vector of roughly 32 qubits (complex128 at 16 bytes per amplitude, so $2^{32} \times 16$ bytes ≈ 68 GB). Work this out yourself and check it against the memory of a GPU you know. This calculation is the single most useful number for sizing quantum-simulation jobs on your clusters.
