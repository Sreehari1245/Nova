This repository contains a MAGMA implementation of the NOVA signature scheme, a multivariate polynomial-based post-quantum cryptographic system. The code follows the algorithms as specified in the NOVA specification document, implementing key generation, signing, and signature verification.

Overview: 

NOVA is a Unbalanced Oil and Vinegar (UOV) scheme enhanced with certain structural components to improve efficiency and compactness. This MAGMA implementation covers:

1. Parameter setup: Finite field extension and matrix definitions
2. Key generation: public and private
3. Signature generation and verification
4. Internal cryptographic transformations (hash emulation via randomness, central map evaluation, etc.)

We implements all the core algorithms from the NOVA specification https://snova.pqclab.org/#page-resources

Our code supports different parameter sets (ell, v, o) — currently hardcoded for ell = 2, v = 6, o = 4

Uses MAGMA’s pseudorandom number generation to emulate SHAKE256/AES for testing purposes

Modular and readable design


