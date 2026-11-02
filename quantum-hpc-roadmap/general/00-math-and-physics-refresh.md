# Phase 0: Math and Physics Refresh

**Duration:** 4–6 weeks (part-time)
**Goal:** Rebuild the mathematical and classical-physics tools that quantum mechanics uses every day.

## Topics and subtopics

### 0.1 Linear algebra (most important)
- Vector spaces over complex numbers, inner products, norms, orthogonality
- Linear operators, matrices, eigenvalues and eigenvectors, diagonalisation
- Hermitian, unitary, and normal operators; spectral theorem
- Tensor (Kronecker) products and partial trace
- Projectors and completeness relations
- Singular value decomposition (needed later for entanglement)

### 0.2 Calculus and analysis
- Partial derivatives, multiple integrals, change of variables
- Complex numbers, Euler's formula, complex exponentials
- Fourier series and Fourier transforms; the Dirac delta function
- Gaussian integrals and integrals with Gaussians

### 0.3 Differential equations
- First- and second-order linear ODEs, power-series solutions
- Eigenvalue problems for ODEs (Sturm–Liouville idea)
- Special functions that appear in QM: Hermite, Legendre, Laguerre, spherical harmonics

### 0.4 Classical mechanics
- Newtonian mechanics, energy and momentum conservation
- Lagrangian and Hamiltonian formulations
- Poisson brackets (the classical analogue of commutators)
- Canonical transformations and action-angle variables (overview)

### 0.5 Electromagnetism (overview only)
- Maxwell's equations at the level needed for atoms and light–matter interaction
- Electric and magnetic dipoles, Larmor precession (used later for spin)

### 0.6 Experimental basis of quantum mechanics
- Blackbody radiation and Planck's constant
- Photoelectric effect
- Compton scattering and the de Broglie hypothesis
- Double-slit experiment and single-photon interference
- Stern–Gerlach experiment (the origin of spin)

## Materials

### Free
- **MIT OCW 18.06** Linear Algebra (Gilbert Strang), lectures and problem sets
- **3Blue1Brown**, *Essence of Linear Algebra* (YouTube, visual intuition)
- **MIT OCW 8.01** Physics I: Classical Mechanics (Lewin's lectures)
- **MIT OCW 18.04** Complex variables with applications (Fourier and complex analysis)
- **Susskind**, *The Theoretical Minimum* lectures (YouTube, Stanford, classical mechanics and QM intuition)

### Textbooks (recommended)
- **Strang**, *Introduction to Linear Algebra* (5th ed.)
- **Taylor**, *Classical Mechanics* (for Lagrangian and Hamiltonian formulations)
- **Griffiths**, *Introduction to Electrodynamics* (Chapters on EM basics only, if needed)
- **Boas**, *Mathematical Methods in the Physical Sciences* (reference)

### Optional paid
- Coursera or edX courses on linear algebra (only if you want a graded certificate)

## Milestones (self-check)

- [ ] Compute eigenvalues and eigenvectors of 2×2 and 3×3 Hermitian matrices by hand
- [ ] Explain why eigenvalues of a Hermitian operator are real and eigenvectors of different eigenvalues are orthogonal
- [ ] Write the Kronecker product of two qubit states and explain it in words
- [ ] Derive the Lagrangian equations of motion for a simple pendulum
- [ ] Explain in one paragraph why the photoelectric effect supports quantized light

## Connection to your HPC background

Linear algebra is also the basis of the numerical libraries you already run (BLAS, LAPACK, cuBLAS). Use that: when you read a matrix diagonalisation routine, recognise the same operations you have benchmarked on GPUs.
