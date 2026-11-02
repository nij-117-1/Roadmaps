# Role 6: Topics

## 1. Stabiliser codes
- Pauli group, stabiliser groups, and logical operators
- Syndrome extraction and error identification
- CSS codes and the Steane code
- Code distance and the number of logical qubits

## 2. Surface code
- Lattice layout, data and ancilla qubits
- Syndrome extraction cycles and their timing
- Logical error rate scaling with code distance
- Lattice surgery and logical operations (overview)

## 3. Decoding algorithms
- Minimum-weight perfect matching (MWPM)
- Union-find decoders
- Belief propagation and other message-passing decoders
- Neural-network decoders and learned priors (overview)
- Trade-offs: accuracy, speed, and memory

## 4. Real-time decoding systems
- Data rates from readout and syndrome streams
- Latency budgets (microseconds per cycle)
- GPU decoders and batching across logical qubits
- FPGA and ASIC decoders for the tightest latency
- Pipelining and back-pressure in streaming systems

## 5. Noise modelling and simulation
- Circuit-level noise models
- Stim and stabiliser-circuit simulation
- Monte Carlo estimation of logical error rates
- Pre-trajectory sampling with batch execution (PTSBE, overview; check current CUDA-Q documentation)

## 6. Threshold and performance analysis
- Threshold theorem and what it assumes
- Estimating threshold from simulation data
- Sensitivity to noise parameters
- Confidence intervals for rare events

## 7. Integration with control and HPC
- Interfaces between readout hardware, decoders, and feedback
- Scheduling decoder workloads on GPU clusters
- Monitoring decoder latency and throughput in production
- Fault handling when a decoder falls behind

## 8. Quantum concepts that drive QEC design
- Why logical error rates must fall below physical error rates
- Why measurement errors also need correction
- Magic-state distillation and why T gates are expensive (overview)
- Gate and readout error budgets

## Tools to learn
- Python (NumPy, SciPy, numba or CuPy for performance)
- CUDA (kernel-level programming for decoders)
- Stim and PyMatching (open-source tools; check their current documentation)
- CUDA-Q QEC (NVIDIA)
- C++ for real-time decoder implementation
