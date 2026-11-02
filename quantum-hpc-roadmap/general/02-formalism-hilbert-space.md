# Phase 2: Formalism and Hilbert Space

**Duration:** 4–5 weeks
**Goal:** Move from wavefunctions to the abstract formalism: states as vectors, observables as operators, measurement, and dynamics. This is the language used by quantum information and quantum engineering.

## Topics and subtopics

### 2.1 State space
- Kets, bras, inner products (Dirac notation)
- Completeness and orthonormal bases
- Position and momentum representations; Fourier transform between them

### 2.2 Operators
- Linear operators, adjoints, Hermitian and unitary operators
- Projectors and spectral decomposition
- Functions of operators (exponentials, for time evolution)

### 2.3 Observables and measurement
- Postulates of quantum measurement
- Expectation values, variance, and standard deviation
- Compatible observables and commuting operators
- Commutators and the general uncertainty relation
- Projective measurement vs. generalised (POVM) measurement (overview)

### 2.4 Time evolution
- Schrödinger picture: $i\hbar\,\partial_t |\psi\rangle = H|\psi\rangle$
- Unitary evolution operator $U(t) = e^{-iHt/\hbar}$
- Heisenberg picture and Heisenberg equations of motion
- Conserved quantities and symmetries (Noether's theorem in QM form)

### 2.5 Position and momentum operators
- Canonical commutation relation $[x, p] = i\hbar$
- Translation operators and generators
- Energy eigenstates in position basis

### 2.6 Two-level systems (critical for qubits)
- Spin-½ as a two-level system
- Rabi oscillations and resonance
- Bloch sphere representation of pure states
- Preview of why this maps directly to a qubit

## Materials

### Free
- **MIT OCW 8.05** Quantum Physics II (Zwiebach, Fall 2013 or similar). Lectures and problem sets on the formalism.
- **MIT OCW 8.321** Quantum Theory I (Todadri, graduate; lecture notes and problem sets)
- **IBM Quantum Learning**, *Basics of quantum information and computation*, the Single systems and Multiple systems sections (uses the same formalism with Qiskit)
- **Preskill's Caltech Ph219 notes**, Chapter 2 (Quantum information; free PDF)

### Textbooks
- **Sakurai & Napolitano**, *Modern Quantum Mechanics* (3rd ed.), Chapters 1–2 (primary text for this phase)
- **Shankar**, *Principles of Quantum Mechanics* (2nd ed.), Chapters 1–4 (the mathematical treatment)
- **Cohen-Tannoudji, Diu & Laloë**, *Quantum Mechanics* Vol. 1, Chapters I–III (reference)

### Optional
- **Zettili**, *Quantum Mechanics: Concepts and Applications* (2nd ed.), for extra worked examples

## Milestones (self-check)

- [ ] Write the Dirac-notation form of a spin-½ state and compute its expectation value of $\sigma_z$
- [ ] Prove that $U(t)$ is unitary when $H$ is Hermitian
- [ ] Explain why non-commuting observables cannot have simultaneous definite values
- [ ] Derive the Heisenberg equation of motion from the Schrödinger equation
- [ ] Map a generic qubit state $\alpha|0\rangle + \beta|1\rangle$ onto a point on the Bloch sphere and explain what each angle means

## Connection to your HPC background

Time evolution with $U(t)=e^{-iHt}$ is a matrix exponential. Numerically, this is where you will meet Krylov methods, Trotterisation, and GPU-accelerated linear algebra. Start a notebook that computes the matrix exponential for a small Hamiltonian using NumPy and SciPy, and compare with eigendecomposition. This prepares you for the simulators in Phase 9.
