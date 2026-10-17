<!--
OpenRTL-Header-Begin
OpenRTL — Open-source hardware accelerators.
Organization: https://github.com/OpenRTL-Lab
Website: https://openrtl.top/

Project: OpenZK
An index of standalone MIT-licensed zero-knowledge hardware accelerator repositories.
Repository: https://github.com/OpenRTL-Lab/OpenZK
File: docs/source-headers.en.md

SPDX-FileCopyrightText: 2026 ZK Hardware Accelerator contributors
Copyright applies to original project contributions only.
SPDX-License-Identifier: MIT
See LICENSE and applicable third-party notices.
OpenRTL-Header-End
-->

# Original-file headers

[简体中文](source-headers.md)

This policy explains OpenRTL organization/project notices, copyright boundaries and complete file coverage, so that source attribution remains traceable when code is copied outside the repository.

## Scope and attribution

Original code and documentation carry a short organization/project/license header. Branding does not transfer copyright: existing project holders are retained. Shared designs authored within this accelerator series remain original implementations, even under a vendor or common directory. Upstream parameter tables retain their source and license; mixed files identify both original contributions and upstream parameters. Canonical license texts are preserved without claiming authorship of their wording.

## Formats and generation

Code uses native comments; Markdown uses an invisible HTML comment. Interpreter, encoding and Mill launcher directives remain first. VERSION, JSON, compiler file lists and preserved parameter-only tables use adjacent .license files; keep companions when copying those files. This catalogue contains no hardware RTL or Scala emission entry. For generated SV notices and stamping commands, use the source-header policy in the specific accelerator repository; do not treat this index as a product-generation project.

## Coverage checks

Run `python3 tools/source_headers.py` and `python3 tools/test_source_headers.py`. The exact inventory classifies file formats and attribution; unknown files are rejected. These checks cover source notices, not hardware behavior or performance.
