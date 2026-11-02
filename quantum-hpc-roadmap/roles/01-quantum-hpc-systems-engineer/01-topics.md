# Role 1: Topics

## 1. Quantum workload fundamentals (for operators)
- Circuit anatomy: qubits, gates, depth, shots, measurement
- Why circuits are compiled (transpilation) and what that does to resource use
- Simulator vs. QPU: when each is used and what each costs
- Quantum job lifecycle: submit, queue, compile, execute, post-process

## 2. Scheduling quantum and classical resources
- Modelling QPUs and simulators as Slurm resources (GRES, partitions, reservations)
- Mixing GPU simulation jobs and hardware jobs in one scheduler
- Fair-share, quotas, and accounting for shared QPU time
- Maintenance windows that coordinate with calibration cycles

## 3. GPU and simulator platform engineering
- GPU cluster design for state-vector and tensor-network simulation
- Memory sizing: state-vector memory grows as $2^n$ complex amplitudes
- Multi-GPU and MPI-based simulators (CUDA-Q, cuQuantum)
- Container images for quantum SDKs on HPC (Apptainer or Singularity, Docker)

## 4. Networking and data paths
- Latency and bandwidth requirements of quantum–classical loops
- InfiniBand and RDMA for low-latency paths
- Storage for experiment data, calibration logs, and job outputs
- Separation of control, management, and data networks

## 5. Vendor integration
- Site acceptance tests and bring-up checklists
- Interfaces to control systems and access nodes (APIs, SSH, REST, gRPC)
- Firmware and software lifecycle for QPU control stacks
- Ticketing and escalation with vendors

## 6. Observability and reliability
- Metrics: queue wait time, simulator throughput, QPU availability, calibration age
- Prometheus and Grafana dashboards
- Incident response and post-incident reviews
- Capacity planning for simulator and QPU demand

## 7. Quantum concepts you must explain to others
- Superposition, entanglement, measurement (as operational concepts)
- Why coherence time matters for scheduling
- Noise and fidelity as service-level metrics
- Why quantum error correction changes future capacity planning

## Tools to learn
- Slurm (advanced configuration, GRES, accounting)
- CUDA-Q and Qiskit (running, not developing)
- Apptainer or Singularity, Docker
- Prometheus, Grafana, and your existing monitoring stack
- Python for automation and API integration
