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
 - `src/`: Core Python modules implementing Grover’s search and oracle logic
 - `docs/`: Extended methodology and background derived from the paper
 - `experiments/`: Sample graphs, test cases, and simulation results

## Reference
Ghadiali, A. M., & Simha, R. (2025). Quantum-Assisted Graph Coloring: Solving the Graph Coloring Problem with Grover’s Algorithm in Qiskit. George Washington University.