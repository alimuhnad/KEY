# KEY roadmap

The current public release is **KEY Core 1.0.0-rc.1 for Windows x64**. This roadmap describes the priorities for moving the candidate toward a stable release. It is a direction of work, not a promise of dates or features already delivered.

## Current foundation

The binary edition includes a native compiler, command-line tools, selected language examples and an inventory demonstration. It supports EXE, DLL and COFF/OBJ output, explicit generics, tagged enums, modules, UTF-8 text, ownership and transactional worlds.

The compiler and development tools are self-hosted internally. Public users run the supplied binaries. See the [distribution guide](distributions/1.0.0-rc.1/README.md) for installation and the [validation summary](distributions/1.0.0-rc.1/VALIDATION.md) for tested scope.

## Priorities before a stable release

| Priority | Work | Evidence needed |
|---|---|---|
| Reliability | Investigate the two unresolved long-running failures and extend persistence and recovery testing | Reproducible findings, documented fixes where required, and repeated runs with retained failure evidence |
| Independent review | Review ownership, security boundaries and native ABI behavior | Findings resolved and independent signoffs recorded |
| Platform coverage | Expand testing across the supported Windows environments | A documented platform matrix and reproducible package checks |
| Distribution | Establish publisher signing and review the delivery process | Verified signed artifacts and documented installation and update procedures |
| Developer experience | Refine diagnostics and documentation using reported programs | Clear examples and regression coverage for confirmed defects |

Stable approval remains pending until the release requirements are satisfied. A successful test campaign alone does not close an unresolved investigation.

## Direction after Core 1

Standard-library coverage, networking, package management, editor tooling and additional platforms are candidates for future work. Their scope and order will be chosen from concrete application needs and validation results. They are not included in the current distribution.

Propose a use case through [GitHub Issues](https://github.com/alimuhnad/KEY/issues/new/choose). Include a small program or workflow, its current limitation and the behavior you need.
