---
title: "Quantum Genetic Optimization"
date: 2020-05-02T17:30:32-06:00
draft: false
---

**Update:** Simulation available [here](https://github.com/pointlander/qgo).

In [Quantum Computing with the Human Brain](/posts/quantum-computing-with-the-human-brain) I introduce the idea of quantum genetic optimization:

> Genetic optimization uses simulated evolution to solve problems. For instance, it could be used to factor numbers. In this case the genome is two numbers: a & b, and the fitness function is |n - (a * b)|. In the case of a quantum implementation the genome would be the quantum computer configuration. The configuration would be evolved until the number is factored. This system searches for a quantum program that factors the number."

To clarify, some qubits of the quantum system would be selected for solution readout. The candidate solution would be read out, and the fitness function would be applied to it. In a fully connected system the particular qubits selected doesn't matter. The number to be factored isn't mapped to qubits in the quantum computer.

Compressed solutions would allow for a smaller number of qubits to be used for solving an optimization problem. After reading the solution qubits out they would be fed into a decompression algorithm, and then the fitness function would be applied. The search then happens in a compressed space.

Using compressed solutions a meta search can be efficiently implemented. With meta search the quantum computer generates its own configuration. In a fully connected 4 qubit system there are 6 connections, so there are more connections than qubits. This make using the output of the qubits to configure the system problematic. If the 4 qubits are decompressed, then there might be enough information to configure the connections.

Using the qubit states in compressed form to configure the entanglements of the quantum computer is perhaps how the universe works as a feedback system. This idea makes me think of the [holographic principle](https://en.wikipedia.org/wiki/Holographic_principle). It should be noted entropy of a black hole ~ r^2 ~ n(n-1)/2 = the number of entries in an adjacency matrix with symmetric connections.
