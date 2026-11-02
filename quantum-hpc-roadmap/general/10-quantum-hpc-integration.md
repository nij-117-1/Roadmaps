# Phase 10: Quantum–HPC Integration

**Duration:** 4–6 weeks (after Phases 6, 7, and 9)
**Goal:** Connect quantum hardware and simulators to classical HPC infrastructure: scheduling, orchestration, data movement, monitoring, and user support. This is your strongest route into the field.

## Topics and subtopics

### 10.1 Architecture of hybrid systems
- Classical–quantum workflow patterns (sequential, iterative, streaming)
- Quantum processing units (QPUs) as accelerators, similar to GPUs
- Access nodes, control systems, and cryostat networks
- Latency and bandwidth budgets for different workloads

### 10.2 Scheduling quantum resources
- Modelling QPUs as schedulable resources in Slurm (GRES, partitions, reservations)
- Queueing policies for shared QPUs
- Mixing simulator and hardware jobs in one scheduler
- Preemption, fairness, and accounting for quantum jobs

### 10.3 Orchestration and middleware
- Qiskit Runtime sessions and batching
- CUDA-Q hybrid workflows and the CUDA-Q Realtime interface (NVQLink, announced October 2025; the cudaq-realtime API was released at GTC 2026)
- REST and gRPC APIs for quantum services
- Containerised quantum workloads (Docker, Singularity or Apptainer) on HPC clusters

### 10.4 Data movement and real-time paths
- Data flows between readout hardware, FPGAs, GPUs, and storage
- Low-latency interconnects (InfiniBand, RDMA) and their role in real-time decoding
- Storage for experiment and calibration data

### 10.5 Calibration and operations
- Automated calibration as a scheduled workflow
- Detecting calibration drift and triggering recalibration
- Coordinating quantum calibration with classical maintenance windows

### 10.6 Monitoring and observability
- Metrics for QPUs: $T_1$, $T_2$, gate and readout fidelity over time
- Facility metrics: cryostat temperatures, pump status, power, cooling water flow
- Dashboards with Prometheus and Grafana (or your site's existing tooling)
- Alerting and incident response

### 10.7 User support and onboarding
- Expert users vs. domain users (as in the LRZ onboarding model)
- Documentation, runbooks, and training material
- Access control and quotas for shared quantum resources

### 10.8 Security and compliance (overview)
- Export controls on quantum hardware and software
- Access policies for remote quantum services
- Post-quantum cryptography migration (overview)

## Materials

### Free
- **arXiv:2509.12949**, "First Practical Experiences Integrating Quantum Computers with HPC Resources" (LRZ and IQM). Read in full. Operations, monitoring, and user support sections are directly relevant.
- **IBM Quantum Learning**, *Integrating Quantum and High-Performance Computing* (free, about 6 hours). Covers computing resources and their management, programming models, and SQD and SKQD workflows.
- **NVIDIA CUDA-Q docs**: MPI plugin, multi-GPU platforms, and the Realtime documentation (nvidia.github.io/cuda-quantum)
- **NVIDIA quantum computing resources hub** (free blogs, GTC session recordings, whitepapers)
- **Slurm documentation** (free, slurm.schedmd.com): GRES, partitions, and job arrays; apply these to quantum job types
- **Qiskit Runtime documentation** (free)

### Practical (use what you already have)
- Your existing Slurm cluster: create a partition for simulator jobs and test accounting for GPU-hours per quantum job
- Prometheus and Grafana: monitor a simulator cluster, then add mock QPU metrics as a dashboard exercise

### Paid (optional)
- Vendor integration training (IQM, Quantum Machines, Q-CTRL, NVIDIA) where offered; check current programmes

## Milestones (self-check)

- [ ] Draw the data path for one hybrid workload from user submission to QPU and back, and mark the latency budget at each step
- [ ] Describe how you would represent a QPU in Slurm (GRES, partition, reservation) and justify the choice
- [ ] Write a runbook for a QPU recalibration event, including who is notified and what is checked
- [ ] Build a Grafana dashboard that shows at least three QPU or facility metrics over time (simulated data is acceptable)
- [ ] Explain the difference between batch and real-time workloads, with one example of each

## Connection to your HPC background

This phase uses almost everything you already know: scheduler design, GPU resource management, storage, networking, monitoring, and user support. The new part is learning which quantum-specific constraints (calibration, cryogenics, latency budgets) change those decisions. Make this phase your portfolio centre-piece.
