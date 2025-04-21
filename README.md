# Quantum-Assisted Graph Coloring with Grover’s Algorithm

This repository contains the full codebase and documentation for the paper "Quantum-Assisted Graph Coloring: Solving the Graph Coloring Problem with Grover’s Algorithm in Qiskit" by Abde Manaaf Ghadiali and Rahul Simha (George Washington University).

The project implements a quantum solution to the NP-hard graph coloring problem using Grover’s search algorithm in Qiskit. Unlike traditional approaches that explore all possible colorings, this method restricts the quantum state space to only valid color pairings, enabling more efficient amplitude amplification. The oracle and diffusion operators are custom-built to handle constraint checking and iterative amplification of correct solutions.

## Features
 - Qiskit-based quantum circuits for small graph coloring instances (2-node and 3-node graphs)
 - Custom encoding and state-restriction circuits for efficient initialization
 - Oracle construction using quantum logic (CX, OR, SIM_OP, and MCX gates)
 - Diffusion operator design aligned with Grover’s original formulation
 - Adaptive Grover iteration strategy for unknown solution counts
 - Simulations using Qiskit AER with detailed result interpretation

## Contents:
 - `notebooks/`: Jupyter notebooks for quantum circuit design and execution
 - `docs/`: Extended methodology and background derived from the paper

### Notebook: `06-general-graph-coloring-grover-search.ipynb`

This notebook presents a quantum algorithm for solving the Graph Coloring Problem using Grover's Search in Qiskit. It showcases how quantum amplitude amplification can be used to identify valid vertex colorings in a graph while minimizing conflicts across connected nodes. The solution involves encoding node colors into qubit pairs, constructing a custom oracle to detect color clashes, and applying the Grover diffusion operator to amplify valid solutions. Two approaches are explored: searching across the full state space and using a restricted initialization that excludes invalid color patterns (e.g., the "11" encoding). The implementation supports flexible iteration counts based on problem parameters, and includes utilities for visualization, entanglement detection, and state preparation. Simulations are performed on small graph instances to illustrate the efficiency and correctness of the algorithm. This notebook serves as a modular and extensible foundation for experimenting with quantum search applied to constraint-based optimization problems.

## Reference
Ghadiali, A. M., & Simha, R. (2025). Quantum-Assisted Graph Coloring: Solving the Graph Coloring Problem with Grover’s Algorithm in Qiskit. George Washington University.