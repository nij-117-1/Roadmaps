# Role 2: Topics

## 1. Quantum programming models
- Circuit IR, parameterised circuits, and classical control flow
- Qiskit primitives (Sampler, Estimator) and sessions
- CUDA-Q kernels in Python and C++, and their compilation path (MLIR, QIR)
- Mapping and transpilation as software problems

## 2. Simulation engineering
- State-vector, density-matrix, tensor-network, and stabiliser simulation: trade-offs
- Noise models and shot-based sampling
- GPU kernels for gate application and tensor contraction
- Benchmarking and regression testing for simulators

## 3. Workflow orchestration
- Directed acyclic graphs for hybrid workloads
- Dependent Slurm jobs and job arrays for parameter sweeps
- Event-driven workflows (for calibration and feedback)
- Retry, checkpointing, and idempotency for long variational loops

## 4. Interfaces and APIs
- REST and gRPC services for QPU access
- Authentication and authorisation for shared quantum resources
- Serialisation of circuits, results, and calibration data
- Versioning of SDKs and runtime APIs

## 5. Latency and real-time software
- Latency budgets for feedback loops
- Real-time threads, lock-free queues, and batching
- CUDA-Q Realtime and NVQLink (overview; check current documentation)

## 6. Software engineering practice
- Testing: unit tests, simulator-based integration tests, golden-result tests
- CI/CD for SDK integrations and container images
- Packaging (Python wheels, C++ installers)
- Code review and documentation for external users

## 7. Quantum concepts that affect code
- Measurement collapses state: consequences for result handling
- Shot noise and statistical error: how many shots are enough
- Noise and drift: why results from the same circuit change over time
- Gate and readout errors: how to apply error mitigation in software

## Tools to learn
- Python (advanced), C++ (intermediate), Rust (optional)
- Qiskit, CUDA-Q, PennyLane (for comparison), Cirq (optional)
- Slurm API and Python bindings
- Docker, Apptainer, and CI tools (GitHub Actions or GitLab CI)
- Profilers: Nsight Systems and Nsight Compute
