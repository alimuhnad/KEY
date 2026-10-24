# Current project state

Public delivery: **KEY Core 1.0.0-rc.1, Windows x64, binary edition**.

- Distribution: [distributions/1.0.0-rc.1/](distributions/1.0.0-rc.1/README.md).
- Publication policy: proprietary binaries, selected examples and user documentation; implementation source remains private.
- Compiler/tool implementation is self-hosted internally. Ordinary public use needs the supplied Windows binaries.
- Candidate validation: 1,276 native language/application/tool cases; one 1,800.003-second Core 1 process with 297,609,000 iterations. Separate matrix, ABI, fuzz and memory evidence is summarized in the distribution.
- Public archive: 12 extracted-package checks passed; five packaging allowlist regressions passed.
- Stable approval: **BLOCKED** pending independent reviews and unresolved historical soak investigations.
- Publisher signing: not configured.
- No standard library, network library, GUI, package manager or broad multi-platform support is claimed.

The earlier v0.4.4 Reality Kernel roadmap and its 1,800-check claim are historical project records, not this candidate's acceptance count. See [the preserved public profile](docs/history/PROJECT_PROFILE_before_Core1.md).
