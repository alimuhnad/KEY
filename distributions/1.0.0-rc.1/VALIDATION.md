# Candidate validation and limits

These results describe the supplied compiler bytes. They are engineering evidence, not a security certification or a guarantee for all programs.

- Compiler SHA256: `ac5263e5e035a3793369630134e91c16de877a2561eb0429d8eec94106760f42`.
- Native Windows language/application/tool cases: **1,276 / 1,276**.
- Separate generated lifetime/borrow matrices: **384 / 384** and **360 / 360**; bounded malformed-source checks: **1,024 / 1,024**.
- Memory validation: 24 workload families at 100,000 and 1,000,000 iterations.
- One continuous Core 1 process: **1,800.003 seconds**, **297,609,000 iterations**, **297,609 save/load cycles**, successful final cleanup. Checkpoint private memory grew from 581,632 to a peak of 733,184 bytes in that campaign.
- Additional release-tool checks: 33 gate regressions and two packaging regressions. Eleven controlled replays exercise archived save failures and current handling of file contention.

Compiler and development tools were built natively from KEY sources and reproduced in self-build checks. The source-based development proof and internal test harnesses are retained privately under the binary-only publication policy. The public package has its own extracted-package checks; its file manifest binds the delivered bytes.

## Open investigations

A historical 0.12.1 workload exited after 89.84 seconds without a diagnostic. A later Core 1 workload stopped after 1,082.198 seconds with an F11 save failure. Controlled Windows sharing conflicts reproduce both symptoms. Current storage retries bounded transient conflicts and preserves previous data on persistent failure. The exact external causes of the historical incidents were not captured and remain unconfirmed. Subsequent successful runs do not close those investigations.

## Supported scope

Windows x64 is the target. Native execution was measured on a Windows 11 machine; a broad Windows-version matrix has not been independently approved. Ordinary EXE and direct DLL generation need no external toolchain. COFF/OBJ linking in a foreign host needs its linker.

There is no bundled standard/network/GUI library or package manager. Text is immutable UTF-8 with byte indexing. Generics require explicit arguments; no inference or traits. Enum payloads and match have documented limits represented by the examples. Module visibility is not process isolation. Raw pointers, unsafe operations and foreign DLL code are outside the safe ownership model. Foreign callbacks are constrained to the supported thread and ABI contracts. General C++/SEH exception crossing, general concurrency and full debug support are not provided.

This package is **unsigned** and **not production approved**. Independent security, ownership, ABI, platform, distribution and long-duration signoffs remain outstanding. No eight-hour run, power-loss safety or formal proof is claimed. Runtime error locations are not stack traces. The compiler is not a sandbox for hostile source.
