# Phase 4: Approximation Methods and Time-Dependent Problems

**Duration:** 4–5 weeks
**Goal:** Solve problems that have no exact solution, and understand how quantum systems respond to time-dependent drives. Both are essential for real quantum hardware (gates are time-dependent pulses).

## Topics and subtopics

### 4.1 Time-independent perturbation theory
- Small parameter expansion; first- and second-order energy corrections
- Wavefunction corrections
- Degenerate perturbation theory
- Stark and Zeeman effects as examples

### 4.2 Variational principle
- Rayleigh–Ritz method
- Choosing trial wavefunctions
- Bounds on the ground state energy

### 4.3 WKB approximation
- Semiclassical wavefunctions in classically allowed and forbidden regions
- Connection formulas at turning points
- Tunnelling rates (overview)

### 4.4 Time-dependent perturbation theory
- Interaction picture
- First-order transition amplitudes
- Fermi's golden rule for transition rates
- Harmonic perturbations and absorption or emission

### 4.5 Two-level systems under drive
- Rabi oscillations (exact solution)
- Rotating-wave approximation
- Pulse area and π and π/2 pulses (essential for gate design)

### 4.6 Adiabatic theorem and Berry phase
- Slowly varying Hamiltonians
- Adiabatic following and its conditions
- Geometric (Berry) phases and holonomic gates (overview)

### 4.7 Sudden approximation and quantum control (overview)
- Sudden vs. adiabatic limits
- Optimal control and pulse shaping (introduction)

## Materials

### Free
- **MIT OCW 8.06** (Harrow, Spring 2016), lectures on perturbation theory, WKB, and time-dependent problems. Includes the lecture notes that cover the Ramsauer–Townsend effect and the WKB approximation.
- **MIT OCW 8.05** (Zwiebach), perturbation theory and time-dependent problems
- **Susskind**, *The Theoretical Minimum* QM lectures on approximation methods
- **IBM Quantum Learning**, *Quantum computing in practice* and *Variational algorithm design* (both apply these ideas directly to circuits)

### Textbooks
- **Sakurai & Napolitano**, Chapters 5 (approximation methods) and 5.8 onwards (time-dependent perturbation)
- **Griffiths & Schroeter**, Chapters 6 (perturbation) and 10 (time-dependent)
- **Shankar**, Chapters 15–18
- **Cohen-Tannoudji**, Vol. 2, Chapters XI and XII (advanced reference)

### Papers (free on arXiv)
- Berry, "Quantum Phase Factors Accompanying Adiabatic Changes" (1984). Read the abstract and main argument; the original paper is short.

## Milestones (self-check)

- [ ] Derive the second-order energy correction for a non-degenerate perturbation
- [ ] Apply the variational principle to estimate the ground state of the harmonic oscillator with a trial Gaussian
- [ ] State the conditions under which WKB is valid
- [ ] Derive Fermi's golden rule from time-dependent perturbation theory
- [ ] Explain why a $\pi$ pulse exchanges the populations of two levels, in the Rabi picture

## Connection to your HPC background

Time-dependent Schrödinger simulations, pulse-level control, and variational algorithms are all compute-heavy workloads. Build a small simulator for a driven two-level system (using NumPy first, then CuPy on a GPU). Measure the speedup and note where it saturates. This will be your first real experience of simulation as an HPC job.
