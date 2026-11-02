# Phase 3: Angular Momentum, Spin, and Atoms

**Duration:** 4 weeks
**Goal:** Master angular momentum algebra, spin, and the hydrogen atom. These are the building blocks for atomic physics, spin qubits, and quantum control.

## Topics and subtopics

### 3.1 Angular momentum algebra
- Commutation relations $[J_i, J_j] = i\hbar\epsilon_{ijk}J_k$
- Raising and lowering operators $J_\pm$
- Eigenvalues $j(j+1)\hbar^2$ and $m\hbar$; multiplicities $2j+1$
- Representations of SU(2) and SO(3) (overview; deeper in Phase 4 if you go further)

### 3.2 Orbital angular momentum
- $L = r \times p$ in quantum form
- Spherical harmonics $Y_\ell^m$ as eigenfunctions of $L^2$ and $L_z$
- Central potentials and separation of variables in spherical coordinates

### 3.3 Spin
- Spin-½ and Pauli matrices
- Spin-1 and general spin-$s$ representations
- Spin precession in magnetic fields (Larmor precession)
- Magnetic moments and the gyromagnetic ratio

### 3.4 Addition of angular momenta
- Coupling two angular momenta: $\vec{J} = \vec{J}_1 + \vec{J}_2$
- Clebsch–Gordan coefficients and the coupled basis
- Applications: two spin-½ particles (singlet and triplet states)

### 3.5 The hydrogen atom
- Radial equation and effective potential
- Quantum numbers $n$, $\ell$, $m$ and their degeneracies
- Energy levels $E_n = -13.6\,\text{eV}/n^2$
- Radial wavefunctions and the Bohr radius
- Selection rules (overview)

### 3.6 Fine structure (overview)
- Spin–orbit coupling
- Relativistic corrections and the Dirac equation (preview)
- Lamb shift and hyperfine structure (overview)

## Materials

### Free
- **MIT OCW 8.05** (Zwiebach), angular momentum and hydrogen lectures
- **MIT OCW 8.06** Quantum Physics III (Harrow, Spring 2016), angular momentum and spin topics
- **Susskind**, *The Theoretical Minimum* QM lectures, angular momentum and spin
- **Fowler (UVa)**, *Graduate Quantum Mechanics* lecture notes (free online), Chapters on angular momentum and the hydrogen atom

### Textbooks
- **Sakurai & Napolitano**, *Modern Quantum Mechanics* (3rd ed.), Chapters 3 and 5 (primary)
- **Griffiths & Schroeter**, Chapters 4 and 6 (hydrogen and spin, more accessible)
- **Shankar**, Chapters 12–14 (angular momentum and hydrogen)
- **Cohen-Tannoudji**, Vol. 1, Chapters VI and VII (reference)

## Milestones (self-check)

- [ ] Derive the eigenvalues of $J^2$ and $J_z$ using only the commutation relations
- [ ] Write the singlet and triplet states of two spin-½ particles
- [ ] Explain why the hydrogen energy depends only on $n$ and not on $\ell$ (and what this implies for degeneracy)
- [ ] Describe the Larmor precession of a spin in a magnetic field, using the Heisenberg equation
- [ ] Explain why spin-orbit coupling splits hydrogen energy levels

## Connection to your HPC background

Angular momentum coupling and Clebsch–Gordan coefficients appear in quantum chemistry codes and in the Hilbert-space dimensions that limit classical simulation. Note how the dimension of a coupled Hilbert space grows: this is the first concrete example of why quantum systems are hard to simulate classically, and why GPUs help up to a point.
