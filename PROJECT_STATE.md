# Project State

## KEY — Reality Execution Kernel

- Creator: **Ali Muhnad (علي مهند)**
- Location: Baghdad, Iraq
- Degree: M.Sc. Electrical and Computer Engineering
- Repository: `alimuhnad/KEY`
- Target: Windows x64 native execution
- Public status: Research / active development
- Current verified roadmap baseline: **v0.4.0 — Immutable World Snapshot Capture**
- Next candidate: **v0.4.1 — Immutable World Snapshot Fork**

## Verified development direction

KEY has verified implementation slices covering:

- Systems IR encoding and verification
- Windows x64 native PE emission
- Scalar values and checked arithmetic
- Generation-checked references
- Native heap pages
- Precise graph tracing and live sweep
- Initial source grammar and typed semantic IR
- First bounded source-to-native compiler slice
- World / Entity / Immutable State
- Atomic Transactions and Receipts
- WorldVersion Lineage
- Explicit Time and Temporal Lineage
- World Events and Event Logs
- Event Causality Graph
- Deterministic Replay
- Authority Grants / Revocations / Decisions
- Authority Decision Evidence and Explanation
- Authority-enforced transaction and replay publication path
- Immutable World Snapshot Capture

## Explicit limitations

The project is **not yet a finished general-purpose language**.

Still incomplete or future work includes:

- General typed-IR-to-native lowering
- Full source language coverage
- Production compiler/runtime integration
- Compiler root discovery for GC
- Full Rules / Knowledge / Evidence kernels
- Snapshot Fork and Simulation stack
- Persistence and crash recovery
- Standard library
- Tooling maturity
- Self-hosting
- Multi-platform backends
