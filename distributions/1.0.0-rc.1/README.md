# KEY Core 1.0.0-rc.1 — Binary edition

Native KEY compiler and command-line tools for **Windows x64**, with example programs and an inventory demonstration. Copyright © 2026 Ali Muhnad.

The [proprietary binary license](LICENSE.md) permits free use for learning and application development, including commercial applications, and permits distributing your compiled applications with their embedded runtime. Compiler/tool implementation source is not distributed. See the license for the exact permissions.

Extract the ZIP into a writable directory, open a terminal there, and run:

```bat
key.cmd version
key.cmd test
key.cmd run examples\core1\text.key
key.cmd build examples\core1\generics.key -o example.exe
example.exe
```

No Python, C++, LLVM, assembler or external linker is required to build ordinary KEY executables or KEY DLLs. Linking a COFF/OBJ into a foreign host uses that host's linker.

The public commands are `build`, `run`, `check`, `test`, `fmt`, `version`, and `help`. The delivered native executable also lists compiler-development commands, but `generate` and compiler self-rebuilding require private development inputs which are not part of this edition.

Core 1 includes explicit generics, tagged enums and exhaustive match, immutable UTF-8 Text, modules, ownership/borrows/destructors, transactional worlds, and the documented native foreign interface. There is no bundled standard library, network library, GUI or package manager.

Run `inventory.cmd` from a directory where you want the demonstration's data saved. Instructions are in [the Arabic guide](USER_GUIDE_AR.md).

**Experimental candidate. Stable approval remains blocked.** Read [validation and known limits](VALIDATION.md). The binaries are unsigned. SHA256 checks identify file bytes; they do not authenticate the publisher. Independent release review and two historical soak investigations remain open.

Report reproducible, non-sensitive defects at [GitHub Issues](https://github.com/alimuhnad/KEY/issues). Include the KEY version, compiler SHA256 from `PACKAGE-MANIFEST.json`, Windows version, command, minimal source, exit code and diagnostic. Use the owner's contact in the repository for sensitive security coordination.

[دليل الاستخدام بالعربية](USER_GUIDE_AR.md) · [License](LICENSE.md) · [Validation](VALIDATION.md)
