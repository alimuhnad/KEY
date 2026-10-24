# Security reporting

KEY Core **1.0.0-rc.1 for Windows x64** is an experimental release candidate. Independent security review and stable production approval remain pending.

## Report a vulnerability

Send sensitive reports privately to **Ali Muhnad** at [alimuhnad72@gmail.com](mailto:alimuhnad72@gmail.com), with the subject `KEY security report`. Please coordinate disclosure before posting vulnerability details in a public issue.

Include the information needed to reproduce and assess the issue:

- KEY version and SHA256 of `bin/keyc.exe`.
- Windows version and architecture.
- Affected compiler, tool or runtime component.
- Minimal source and exact commands.
- Expected behavior, actual behavior and full diagnostics.
- Potential impact and any relevant logs, with private data removed.

For ordinary bugs and feature requests, use [GitHub Issues](https://github.com/alimuhnad/KEY/issues/new/choose).

## Scope and boundaries

Ownership and borrowing checks apply within the supported language model. Raw pointers, unsafe operations and foreign DLL code are outside that safe ownership model. The compiler is not a sandbox for hostile source.

The distributed binaries are unsigned. Published SHA256 values identify file bytes; they do not authenticate the publisher. Candidate test results are not a security certification.

See [Validation and limits](distributions/1.0.0-rc.1/VALIDATION.md) for the current platform, ABI and runtime boundaries and open investigations.
