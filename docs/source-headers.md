<!--
OpenRTL-Header-Begin
OpenRTL — Open-source hardware accelerators.
Organization: https://github.com/OpenRTL-Lab
Website: https://openrtl.top/

Project: OpenZK
An index of standalone MIT-licensed zero-knowledge hardware accelerator repositories.
Repository: https://github.com/OpenRTL-Lab/OpenZK
File: docs/source-headers.md

SPDX-FileCopyrightText: 2026 ZK Hardware Accelerator contributors
Copyright applies to original project contributions only.
SPDX-License-Identifier: MIT
See LICENSE and applicable third-party notices.
OpenRTL-Header-End
-->

# 原创文件Header规范

[English](source-headers.en.md)

本文说明OpenRTL组织与项目标识、版权边界和逐文件覆盖规则，确保代码脱离仓库后仍可追溯来源。

## 来源与归属

原创代码和文档使用简短组织／项目／许可Header。品牌展示不等于版权转让，现有持有人保持不变。本加速器系列原创的共享硬件即使位于common或vendor目录也不误归上游；上游参数表保留来源及许可，混合文件同时标明原创部分和参数归属。标准许可证原文不改，也不对其措辞主张原创。

## 格式与生成

代码用原生注释，Markdown用不可见HTML注释；解释器、编码及Mill启动指令保持首部。VERSION、JSON、编译清单及保留的纯参数表使用相邻.license文件，单独复制时也须携带伴随文件。本目录没有硬件RTL或Scala生成入口；生成SV的来源声明和添加命令以具体算子仓库的Header规范为准，不把本索引当作产品生成工程。

## 覆盖检查

运行 `python3 tools/source_headers.py` 和 `python3 tools/test_source_headers.py`。精确清单说明文件格式与归属，未知文件被拒绝。检查范围是来源声明，不是硬件行为或性能。
