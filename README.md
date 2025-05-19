This repository contains a MAGMA implementation of the NOVA signature scheme, a multivariate polynomial-based post-quantum cryptographic system. The code follows the algorithms as specified in the NOVA specification document, implementing key generation, signing, and signature verification.

Overview: 

NOVA is a Unbalanced Oil and Vinegar (UOV) scheme enhanced with certain structural components to improve efficiency and compactness. This MAGMA implementation covers:

Parameter setup: Finite field extension and matrix definitions
Key generation: public and private
Signature generation and verification
Internal cryptographic transformations (hash emulation via randomness, central map evaluation, etc.)

We implements all the core algorithms from the NOVA specification https://snova.pqclab.org/#page-resources

Supports different parameter sets (ell, v, o) — currently hardcoded for ell = 2, v = 6, o = 4
Uses MAGMA’s pseudorandom number generation to emulate SHAKE256/AES for testing purposes
Modular and readable design

