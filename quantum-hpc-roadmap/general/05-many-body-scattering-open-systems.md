# Phase 5: Identical Particles, Scattering, and Open Systems

**Duration:** 5 weeks
**Goal:** Handle systems of identical particles, scattering experiments, and quantum systems that interact with their environment (the reality of all real quantum hardware).

## Topics and subtopics

### 5.1 Identical particles
- Symmetrisation and antisymmetrisation of wavefunctions
- Bosons and fermions; spin–statistics connection (overview)
- Pauli exclusion principle and Slater determinants
- Exchange interaction (overview, helium atom)

### 5.2 Second quantisation (introduction)
- Fock space and occupation number states
- Creation and annihilation operators for bosons and fermions
- Why this is the language of quantum field theory and many-body physics

### 5.3 Scattering theory
- Scattering amplitude and cross-section
- Born approximation
- Partial-wave expansion and phase shifts
- Optical theorem
- Resonances and Breit–Wigner formula

### 5.4 The density matrix
- Pure vs. mixed states
- Density operator $\rho$, trace, purity
- Partial trace and reduced states
- Expectation values from $\rho$

### 5.5 Open quantum systems
- System–environment interaction and the Lindblad master equation (overview)
- Dephasing (T2) and relaxation (T1)
- Quantum channels and Kraus operators (introduction)

### 5.6 Decoherence
- Why superpositions of macroscopic states are fragile
- Decoherence as an information-leaking process
- Connection to the measurement problem (overview)

### 5.7 Thermal states (introduction)
- Gibbs state $\rho = e^{-\beta H}/Z$
- Relation to statistical mechanics

## Materials

### Free
- **MIT OCW 8.06** (Harrow, 2016), lectures on identical particles, density operators, and scattering (the 2016 syllabus covers all three)
- **MIT OCW 8.321** (Todadri, graduate), for identical particles and the density matrix
- **Fowler (UVa)**, *Graduate Quantum Mechanics*, scattering and density matrix sections
- **Preskill's Ph219 notes**, Chapter 3 (quantum information and mixed states)

### Textbooks
- **Sakurai & Napolitano**, Chapters 6 (scattering) and 7 (identical particles)
- **Shankar**, Chapters 19 (scattering) and 21 (identical particles and density matrix)
- **Schlosshauer**, *Decoherence and the Quantum-to-Classical Transition* (Springer, 2007). Standard reference for decoherence.
- **Breuer & Petruccione**, *The Theory of Open Quantum Systems* (Oxford, 2002). Advanced; read selected chapters.

### Papers (free on arXiv)
- Zurek, "Decoherence, einselection, and the quantum origins of the classical" (Reviews of Modern Physics, 2003)

## Milestones (self-check)

- [ ] Explain why a two-fermion state must be antisymmetric, and construct the singlet of two spin-½ particles
- [ ] Derive the Born approximation for the scattering amplitude of a weak potential
- [ ] Compute the density matrix of a mixed state and show that its purity is less than 1
- [ ] Explain the difference between T1 and T2 in terms of the density matrix
- [ ] Describe, in one page, how environment-induced decoherence explains the classical appearance of a system

## Connection to your HPC background

Density matrices scale as the square of the state vector, so simulating open systems is more memory-intensive than pure states. This is why tensor-network and trajectory-based methods exist. Understanding this trade-off will help you size GPU memory for quantum simulators later.
