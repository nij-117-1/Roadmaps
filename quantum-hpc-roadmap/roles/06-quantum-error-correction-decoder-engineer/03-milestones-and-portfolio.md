# Role 6: Milestones and Portfolio

## Milestones (self-check)
- [ ] Write the stabilisers of a small stabiliser code and identify its logical operators from the stabiliser group
- [ ] Explain why a syndrome identifies an error without revealing the logical state
- [ ] Describe one surface-code syndrome cycle, including what each ancilla measures
- [ ] Explain why decoding must keep up with the syndrome rate, and what happens if it does not
- [ ] Compare MWPM and union-find on accuracy, speed, and memory, in your own words
- [ ] Explain how you would estimate a logical error rate by Monte Carlo sampling, and how many samples you need for a given confidence
- [ ] Describe a latency budget for a decoder in a real-time loop and where the time goes

## Portfolio projects
1. **Repetition and Steane code simulation:** use Stim to simulate a code under bit-flip and depolarising noise and plot the logical error rate.
2. **Surface-code threshold study:** simulate surface codes at several distances and noise rates, and estimate the threshold from the crossing point.
3. **Decoder benchmark:** compare PyMatching and a second decoder on the same syndrome data, reporting accuracy, throughput, and memory.
4. **GPU batch decoder experiment:** decode many independent syndrome streams in parallel on a GPU and report throughput against batch size.
5. **Latency model:** a simple model of a real-time decoding pipeline (readout, transfer, decode, feedback) with a latency budget table.

## Interview preparation
- **Theory:** derive the stabiliser conditions for a small code on a whiteboard. Explain syndrome decoding in words.
- **Systems:** a decoder falls behind by 20% at a given code distance. Walk through the options: algorithm change, batching, hardware, or code distance change.
- **Analysis:** you have 10,000 Monte Carlo samples and see zero logical errors. What can you say, and what can you not say?
- **HPC:** how would you schedule decoder jobs on a GPU cluster that also runs simulation jobs, with a hard latency requirement?

## Application checklist
- [ ] Public repositories with Stim and decoder projects, with clear READMEs and plots
- [ ] Contributions to an open-source QEC tool (documentation and tests count)
- [ ] CV section "Quantum Error Correction and Real-Time Decoding" with GPU and latency results
- [ ] Apply to decoder, QEC software, and quantum–HPC roles at NVIDIA, Quantinuum, IBM, and QPU vendors with QEC programmes
