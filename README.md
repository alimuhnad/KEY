# KEY

**A native programming language for Windows x64.**

KEY combines explicit ownership, typed programming and transactional worlds with direct native code generation. Its compiler produces Windows executables, dynamic libraries and COFF object files. The compiler and development tools are written in KEY and maintained through an internal self-hosted build process.

Created by **Ali Muhnad — علي مهند**, Baghdad, Iraq.

[**Download for Windows x64**](distributions/1.0.0-rc.1/KEY-Core-Binary-1.0.0-rc.1-windows-x64.zip?raw=true) · [Getting started](distributions/1.0.0-rc.1/README.md) · [دليل الاستخدام بالعربية](distributions/1.0.0-rc.1/USER_GUIDE_AR.md) · [Examples](distributions/1.0.0-rc.1/examples)

## Current release

| | KEY Core |
|---|---|
| Version | **1.0.0-rc.1** |
| Platform | Windows x64 |
| Status | Experimental release candidate |
| Distribution | Compiler, command-line tools, examples and inventory demo |
| License | Proprietary; free use for learning and application development under the [binary license](distributions/1.0.0-rc.1/LICENSE.md) |

This repository distributes the public binary edition and its documentation. Compiler implementation sources and development inputs remain private. The candidate is available for evaluation; stable production approval remains pending.

## Language and toolchain

| Area | Available in Core 1 |
|---|---|
| Native output | EXE, DLL and COFF/OBJ for Windows x64 |
| Types | Structs, explicit type and function generics, tagged enums and exhaustive statement matching |
| Resources | Affine ownership, borrowing and destructors |
| Text | Immutable UTF-8 text with byte indexing |
| Organization | Modules, imports and public declarations |
| State | Transactional worlds and resource transfers |
| Interoperability | Windows foreign-function interface within the supported ABI contracts |
| Tools | Build, run, check, test and format commands |

Ordinary EXE and direct DLL builds run with the supplied tools, without Python, C++, LLVM, an assembler or an external linker. Linking a COFF object into a foreign host uses that host's linker.

Use the candidate to explore native command-line programs, typed data models, resource management and transactional state. The included inventory application demonstrates transfers, persistence and restart recovery with test data.

## Get started

Download the ZIP, extract it into a writable directory and open PowerShell in that directory:

```powershell
.\key.cmd version
.\key.cmd test
.\key.cmd run examples\core1\text.key
.\key.cmd build examples\core1\generics.key -o example.exe
.\example.exe
```

The text example prints UTF-8 text. The generics example checks its results with assertions and exits successfully without printing output.

To try the inventory demo, run `.\inventory.cmd` and follow the [Arabic walkthrough](distributions/1.0.0-rc.1/USER_GUIDE_AR.md). The package includes nine example source files: eight runnable examples and one imported module.

The download's [SHA256 checksum](distributions/1.0.0-rc.1/KEY-Core-Binary-1.0.0-rc.1-windows-x64.zip.sha256) and the archive's file manifest let you check file integrity. The binaries are currently unsigned.

## Validation and release scope

The matching compiler passed **1,276 native language, application and tool cases**. A continuous Core 1 run completed **30 minutes and 297,609,000 iterations**. The public archive passed **12 extracted-package checks**, with **five additional packaging allowlist regressions**.

These results describe the tested candidate. Independent reviews and two investigations from earlier long-running workloads remain open. Full evidence summaries and known limitations are documented in [Validation and limits](distributions/1.0.0-rc.1/VALIDATION.md).

Core 1 does not bundle a standard library, networking library, GUI framework or package manager. General concurrency, a general exception model and support for other operating systems are outside this release. See the [roadmap](ROADMAP.md) for current priorities.

## License

The [KEY Core Binary Distribution License](distributions/1.0.0-rc.1/LICENSE.md) permits free use for learning and application development, including commercial applications. It also permits distribution of your compiled applications with their embedded KEY runtime and adaptation of the supplied examples under its terms.

Redistributing or modifying the compiler and development tools requires additional permission. KEY is proprietary. The [repository license](LICENSE.md) and [ownership notice](IP_NOTICE.md) cover the remaining project materials.

## Feedback and contact

Submit reproducible, non-sensitive defects through [GitHub Issues](https://github.com/alimuhnad/KEY/issues/new/choose). Include the KEY version, compiler SHA256, Windows version, exact command, minimal example and full diagnostic. Feature proposals should describe a concrete program and the behavior it needs.

For sensitive reports, follow the [security reporting policy](SECURITY.md).

**Ali Muhnad — علي مهند**, creator and principal developer · Baghdad, Iraq.

[@alimuhnad](https://github.com/alimuhnad) · [alimuhnad72@gmail.com](mailto:alimuhnad72@gmail.com)

Copyright © 2026 Ali Muhnad. All rights reserved except as expressly granted in the applicable license.
