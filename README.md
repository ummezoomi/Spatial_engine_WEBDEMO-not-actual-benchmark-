U.M.E.R Spatial Engine – Demo & Visualization Repository

This repository contains simulation outputs, benchmark videos, and visualization artifacts for the research work:

U.M.E.R: A Deterministic Sort Free Architecture for High Density Physical & Agentic Systems
Author: Muhammad Umer
DOI: https://doi.org/10.21203/rs.3.rs-9848255/v1

Overview

U.M.E.R (Uniform Memory Encoded Representation) is a GPU-oriented spatial simulation architecture designed for high-density physical and agentic systems. The framework replaces traditional hierarchical spatial structures (BVH, Octrees) with a deterministic, sort-free, scan-based pipeline optimized for temporal coherence and cache efficiency.

This repository serves as the visual and experimental companion to the research paper, showcasing real-time simulations, benchmarks, and comparative evaluations.

Key Research Contributions (Summary)
Sort-free spatial hashing via parallel prefix-sum pipeline
Temporal coherence exploitation using Delta Histogram updates
O(N) spatial mapping without full topology rebuilds
Unified execution model for physics + agentic navigation
GPU-optimized Structure of Arrays (SoA) memory layout
High-density simulation scaling up to 500,000–1,000,000 agents
Repository Contents
🧠 Core Simulations
UMER_Boids(3).mp4
Emergent flocking behavior using U.M.E.R agentic dynamics
UMER_vs_ASTAR_Final.mp4
Comparative benchmark: U.M.E.R spatial navigation vs classical A*
demo1_splitscreen (1).mp4
Side-by-side visualization of algorithmic behavior and performance
demo2_dambreak_telemetry.mp4
High-density fluid/particle simulation with telemetry output
umer_showcase.mp4
General demonstration of engine capabilities and system behavior
📊 Visual & Analytical Outputs
crossover_paradox.png
Spatial transition visualization under dynamic redistribution conditions
🌐 Web Demonstration
webgpudemo.html
Browser-based GPU simulation demo illustrating core spatial engine principles
Performance Highlights (from paper)
Up to 1.52× speedup over NVIDIA Warp in controlled benchmarks
Sustained 125 FPS at 500,000 agents (agentic simulation mode)
~99.7% reduction in atomic memory operations via delta histogram updates
21,000+ MCELL/s throughput on GPU spatial workloads
Deterministic execution across 100+ identical simulation runs
Design Philosophy

This system is built around three core principles:

Deterministic Execution
Identical inputs produce bitwise identical outputs across runs.
Memory Coherence First Design
Cache behavior and memory layout are treated as first-class constraints.
Sort-Free Spatial Computation
Eliminates traditional sorting and tree rebuild overhead in favor of scan-based linearization.
Relationship to Paper

This repository does not replace the research paper.
It provides:

Visual validation of experimental claims
Real-time simulation outputs
Reproducible demo artifacts
System-level behavioral evidence

For full methodology, proofs, and formal benchmarking, refer to the DOI above.

License & Notes

This project is part of ongoing research work.
Some components are experimental and may evolve over time.
