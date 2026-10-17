<!--
OpenRTL-Header-Begin
OpenRTL — Open-source hardware accelerators.
Organization: https://github.com/OpenRTL-Lab
Website: https://openrtl.top/

Project: OpenZK
An index of standalone MIT-licensed zero-knowledge hardware accelerator repositories.
Repository: https://github.com/OpenRTL-Lab/OpenZK
File: README.zh-CN.md

SPDX-FileCopyrightText: 2026 ZK Hardware Accelerator contributors
Copyright applies to original project contributions only.
SPDX-License-Identifier: MIT
See LICENSE and applicable third-party notices.
OpenRTL-Header-End
-->

# OpenZK

[English](README.md)

本仓库索引 OpenRTL 的 11 个独立、采用 MIT 许可证的零知识证明硬件加速器仓库，覆盖 Goldilocks 域运算、多项式变换与折叠、Sumcheck 与多线性扩展求值、Poseidon2 哈希与 Merkle 树，以及 BN254-G1 多标量乘法。各仓库提供 Chisel 源码与生成的 SystemVerilog，供 ASIC 或 FPGA 设计集成；这里索引的是计算模块，不是完整证明器。

- **NTT / INTT**：通过数论变换及其逆变换，在 Goldilocks 域上的多项式系数与求值之间转换。 [goldilocks-ntt-intt](https://github.com/OpenRTL-Lab/goldilocks-ntt-intt/blob/main/README.zh-CN.md)

- **陪集低度扩展**：计算 Goldilocks 域上的低度扩展，从多项式系数或求值出发，得到扩展陪集上的求值。 [coset-lde-goldilocks](https://github.com/OpenRTL-Lab/coset-lde-goldilocks/blob/main/README.zh-CN.md)

- **FRI 折叠**：根据挑战值，对 Goldilocks 域上的求值表进行二元折叠，用于 FRI 的折叠步骤。 [fri-fold-goldilocks](https://github.com/OpenRTL-Lab/fri-fold-goldilocks/blob/main/README.zh-CN.md)

- **Goldilocks 素域向量运算**：提供 Goldilocks 素域上的向量加、减、乘、乘加、线性组合和点积。 [prime-field-vector-goldilocks](https://github.com/OpenRTL-Lab/prime-field-vector-goldilocks/blob/main/README.zh-CN.md)

- **Goldilocks 批量求逆**：计算 Goldilocks 域上的批量求逆与批量除法，适用于需要大量域元素倒数或商的计算。 [batch-inversion-goldilocks](https://github.com/OpenRTL-Lab/batch-inversion-goldilocks/blob/main/README.zh-CN.md)

- **Goldilocks 二次扩域向量运算**：提供 Goldilocks 二次扩域上的向量加、减、乘、平方、求逆、乘加和点积，处理的不是素域元素。 [extension-field-vector-goldilocks](https://github.com/OpenRTL-Lab/extension-field-vector-goldilocks/blob/main/README.zh-CN.md)

- **Sumcheck / MLE**：计算 Goldilocks 域上的单轮 Sumcheck 系数、多线性表折叠及多线性扩展求值，不是完整的 Sumcheck 协议实现。 [sumcheck-mle-goldilocks](https://github.com/OpenRTL-Lab/sumcheck-mle-goldilocks/blob/main/README.zh-CN.md)

- **BN254-G1 多标量乘法**：计算 BN254-G1 上的多标量乘法，即椭圆曲线点的标量加权和，而非 Goldilocks 域运算。 [bn254-msm](https://github.com/OpenRTL-Lab/bn254-msm/blob/main/README.zh-CN.md)

- **Poseidon2 置换**：提供 Goldilocks 域上的 Poseidon2 状态置换，适用于直接集成置换核、而非消息哈希接口的设计。 [poseidon2-goldilocks](https://github.com/OpenRTL-Lab/poseidon2-goldilocks/blob/main/README.zh-CN.md)

- **Poseidon2 海绵哈希**：提供 Goldilocks 域上基于 Poseidon2 的消息哈希与双摘要压缩，而不只是底层状态置换。 [poseidon2-sponge](https://github.com/OpenRTL-Lab/poseidon2-sponge/blob/main/README.zh-CN.md)

- **Poseidon2 Merkle 树运算**：提供基于 Goldilocks 域 Poseidon2 的叶子哈希、二叉 Merkle 树构建和认证路径验证，用于树承诺。 [merkle-goldilocks](https://github.com/OpenRTL-Lab/merkle-goldilocks/blob/main/README.zh-CN.md)
