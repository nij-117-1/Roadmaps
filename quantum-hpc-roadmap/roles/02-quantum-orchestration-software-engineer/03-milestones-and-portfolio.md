# Role 2: Milestones and Portfolio

## Milestones (self-check)
- [ ] Explain the difference between a Qiskit Sampler and an Estimator, and when you would use each
- [ ] Write a parameterised circuit and a classical optimiser loop from memory
- [ ] Explain why a state-vector simulator's runtime depends on the number of gates as well as qubits
- [ ] Design a dependent Slurm workflow for a 200-iteration variational run, including checkpoints
- [ ] Describe how you would test a simulator integration without access to hardware
- [ ] Explain shot noise and how many shots give a given standard error in an expectation value
- [ ] Describe three ways a result can change between runs of the same circuit on hardware

## Portfolio projects
1. **Hybrid workflow engine:** a small Python tool that runs a parameter sweep as Slurm arrays, collects results, and restarts from checkpoints.
2. **CUDA-Q or Qiskit backend adapter:** a thin layer that submits circuits to a simulator on your cluster with a common interface.
3. **Simulator regression suite:** golden-result tests for a set of circuits, run in CI on a GPU runner.
4. **Result pipeline:** serialisation of circuits and results to a versioned format, with a schema and tests.
5. **Latency study:** measure round-trip time for a simulated feedback loop on a local cluster and report the bottlenecks.

## Interview preparation
- **Coding:** implement a small job queue, a retry policy, or a circuit serialiser in Python within an hour.
- **Systems design:** design a service that lets 50 researchers submit hybrid jobs to a shared QPU and simulator pool.
- **Physics fundamentals:** explain measurement, entanglement, and noise, and how each affects software design.
- **Debugging:** a variational run diverges after 40 iterations on hardware but not in simulation. Walk through the diagnosis.

## Application checklist
- [ ] Public GitHub repositories with tests and CI for at least two portfolio projects
- [ ] Contributions to an open-source quantum SDK (documentation fixes count)
- [ ] CV section "Hybrid Quantum–HPC Software" with languages, SDKs, and project links
- [ ] Apply to software engineering roles at Quantinuum, NVIDIA, IBM, IonQ, and D-Wave
