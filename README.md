<!--
OpenRTL-Header-Begin
OpenRTL — Open-source hardware accelerators.
Organization: https://github.com/OpenRTL-Lab
Website: https://openrtl.top/

Project: OpenZK
An index of standalone MIT-licensed zero-knowledge hardware accelerator repositories.
Repository: https://github.com/OpenRTL-Lab/OpenZK
File: README.md

SPDX-FileCopyrightText: 2026 ZK Hardware Accelerator contributors
Copyright applies to original project contributions only.
SPDX-License-Identifier: MIT
See LICENSE and applicable third-party notices.
OpenRTL-Header-End
-->

# OpenZK

[简体中文](README.zh-CN.md)

This repository indexes 11 standalone, MIT-licensed zero-knowledge hardware accelerator repositories from OpenRTL. They cover Goldilocks field arithmetic, polynomial transforms and folding, Sumcheck and multilinear-extension evaluation, Poseidon2 hashing and Merkle trees, and BN254-G1 multi-scalar multiplication. Each repository provides Chisel sources and generated SystemVerilog for ASIC or FPGA integration. These are compute blocks, not a complete prover.

- **NTT / INTT**: Converts between polynomial coefficients and evaluations over Goldilocks using forward and inverse number-theoretic transforms. [goldilocks-ntt-intt](https://github.com/OpenRTL-Lab/goldilocks-ntt-intt)

- **Coset-LDE**: Computes low-degree extensions over Goldilocks, starting from polynomial coefficients or evaluations and producing evaluations on an extended coset. [coset-lde-goldilocks](https://github.com/OpenRTL-Lab/coset-lde-goldilocks)

- **FRI Fold**: Performs challenge-driven binary folding of Goldilocks evaluation tables for FRI folding steps. [fri-fold-goldilocks](https://github.com/OpenRTL-Lab/fri-fold-goldilocks)

- **Goldilocks prime-field vectors**: Provides vector addition, subtraction, multiplication, multiply-add, linear combinations, and dot products over the Goldilocks prime field. [prime-field-vector-goldilocks](https://github.com/OpenRTL-Lab/prime-field-vector-goldilocks)

- **Goldilocks batch inversion**: Computes batch inverses and batch divisions over Goldilocks for workloads that need many field reciprocals or quotients. [batch-inversion-goldilocks](https://github.com/OpenRTL-Lab/batch-inversion-goldilocks)

- **Goldilocks quadratic-extension vectors**: Provides vector addition, subtraction, multiplication, squaring, inversion, multiply-add, and dot products over a quadratic extension of Goldilocks rather than the prime field itself. [extension-field-vector-goldilocks](https://github.com/OpenRTL-Lab/extension-field-vector-goldilocks)

- **Sumcheck / MLE**: Computes single-round Sumcheck coefficients, multilinear-table folds, and multilinear-extension evaluations over Goldilocks; it is not a complete Sumcheck protocol implementation. [sumcheck-mle-goldilocks](https://github.com/OpenRTL-Lab/sumcheck-mle-goldilocks)

- **BN254-G1 MSM**: Computes multi-scalar multiplication on BN254-G1: a scalar-weighted sum of elliptic-curve points, rather than Goldilocks field arithmetic. [bn254-msm](https://github.com/OpenRTL-Lab/bn254-msm)

- **Poseidon2 permutation**: Provides the Goldilocks Poseidon2 state permutation for designs that need the permutation core directly, rather than a message-hashing interface. [poseidon2-goldilocks](https://github.com/OpenRTL-Lab/poseidon2-goldilocks)

- **Poseidon2 sponge**: Provides Poseidon2-based message hashing and two-digest compression over Goldilocks, rather than only the underlying state permutation. [poseidon2-sponge](https://github.com/OpenRTL-Lab/poseidon2-sponge)

- **Poseidon2 Merkle operations**: Provides Goldilocks Poseidon2 leaf hashing, binary Merkle-tree construction, and authentication-path verification for tree commitments. [merkle-goldilocks](https://github.com/OpenRTL-Lab/merkle-goldilocks)
