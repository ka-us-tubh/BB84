# BB84 Protocol
<img src="BB84-quantum-key-distribution.png">
<h5>Figure available via license: Creative Commons Attribution 4.0 International</h5>

This repository contains a basic implementation of the BB84 protocol using Python and Qiskit.

## Overview

The BB84 protocol is a quantum key distribution (QKD) protocol proposed by Charles Bennett and Gilles Brassard in 1984. It enables two parties, Alice and Bob, to establish a secure key for encrypting and decrypting messages using the principles of quantum mechanics.

## BB84 Protocol

In the BB84 protocol:
- Alice generates a random sequence of binary digits and encodes each bit as a photon using either the horizontal/vertical or diagonal polarization basis.
- Bob randomly chooses a basis for measuring each photon he receives from Alice and records the outcome as either 0 or 1.
- After exchanging a sufficient number of photons, Alice and Bob publicly compare a subset of their measurement bases and discard any bits that were not measured using the same basis to estimate the error rate caused by Eve, the potential eavesdropper.
- To ensure the security of the key, Alice and Bob perform privacy amplification by hashing a smaller number of the remaining bits to generate a shorter, secure key.

## Files

- **BB84.ipynb**: This Jupyter Notebook contains the implementation of the BB84 protocol using Python and Qiskit.

## Contributors

- **ka-us-tubh**: Creator of the project and primary contributor.
