# Phase 1: Wave Mechanics

**Duration:** 4–5 weeks
**Goal:** Understand the wavefunction, the Schrödinger equation, and the standard one-dimensional problems.

## Topics and subtopics

### 1.1 Wave–particle duality
- de Broglie wavelength, wave packets, group and phase velocity
- Probability interpretation (Born rule) for position

### 1.2 The Schrödinger equation
- Time-dependent and time-independent forms
- Separation of variables, stationary states, energy eigenvalues
- Probability current and conservation of probability
- Normalisation and boundary conditions

### 1.3 Free particles and wave packets
- Plane waves, Fourier representation of wave packets
- Spreading of wave packets over time

### 1.4 Uncertainty principle
- Position–momentum uncertainty from Fourier analysis
- General uncertainty relation for two observables (preview; full treatment in Phase 2)

### 1.5 One-dimensional bound states
- Infinite square well (and its time evolution)
- Finite square well and bound-state matching conditions
- Delta-function potential

### 1.6 Scattering and tunnelling in 1D
- Step potentials, transmission and reflection coefficients
- Rectangular barrier, tunnelling
- Resonant transmission (Ramsauer–Townsend effect, overview)

### 1.7 The harmonic oscillator
- Power-series solution and Hermite polynomials
- Ladder (creation and annihilation) operators
- Coherent states (overview)

### 1.8 Ehrenfest theorem and the classical limit
- Expectation values and how classical equations emerge
- When and why wave packets follow classical trajectories

## Materials

### Free
- **MIT OCW 8.04** Quantum Physics I (Barton Zwiebach, 2016), lecture videos and notes. Note: the 2013 version (Allan Adams) is also excellent and covers more ground.
- **MITx 8.04x** on edX (free audit). Same course, with graded problem sets.
- **Susskind**, *Quantum Mechanics: The Theoretical Minimum* (lectures and book)
- **IBM Quantum Learning**, *Quantum mechanics* module, *Superposition with Qiskit* and *Exploring uncertainty with Qiskit* (free, interactive)
- **Zwiebach**, *Mastering Quantum Mechanics* (MIT Press, 2022), companion to 8.04

### Textbooks
- **Griffiths & Schroeter**, *Introduction to Quantum Mechanics* (3rd ed.), Chapters 1–3 and 5 (harmonic oscillator)
- **Shankar**, *Principles of Quantum Mechanics* (2nd ed.), Chapters 1–5 (more mathematical; use alongside Griffiths)
- **Townsend**, *A Modern Approach to Quantum Mechanics* (2nd ed.), for a gentler second read

## Milestones (self-check)

- [ ] Derive the probability current and show that it satisfies a continuity equation
- [ ] Explain why bound-state energies of the infinite well are quantized, from boundary conditions
- [ ] Explain why a particle can tunnel through a barrier higher than its energy, with the formula for transmission
- [ ] Explain the difference between the ground state of the harmonic oscillator and a classical particle at rest
- [ ] Describe in words what happens to a Gaussian wave packet as it evolves freely

## Connection to your HPC background

Finite-difference and split-operator methods for the time-dependent Schrödinger equation are classic HPC workloads. When you reach this phase, plan a small Python script that solves the 1D time-dependent Schrödinger equation on a grid; run it on a CPU and later on a GPU (CuPy or NumPy comparison). This will connect the physics to the code you already know how to run at scale.
