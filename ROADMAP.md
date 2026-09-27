# KEY Roadmap

KEY is developed in small verified increments. Each micro-version has a single objective and must pass its acceptance target before advancement.

**Verified through: v0.4.4**  
**Next candidate: v0.4.5 — Fork-Local WorldVersion Envelope**

## 0.0.x — Native foundation
- Systems IR and verifier
- Windows x64 native emitter
- Values and references
- Native heap
- Precise tracing / live sweep
- Lexer / parser / typed IR
- First bounded source-to-native slice

## 0.1.x — World / Entity / State / Transactions
- World identity
- Entity identity registry
- Immutable entity state
- Atomic state transition
- Bounded multi-change transaction
- Provenance receipt
- WorldVersion envelope
- WorldVersion lineage / lineage chain

## 0.2.x — Time / Events / Causality / Replay
- Explicit Time
- Commit Time binding
- Temporal lineage / temporal chain
- World Event / Event Log
- Causal link / causal graph
- Deterministic replay plan
- Replay cursor

## 0.3.x — Authority-enforced execution path
- Grants
- Operation permits
- Revocations
- Multi-revocation decisions
- Decision evidence / evidence log
- Deterministic decision explanation
- Authority-enforced transaction
- Authority-enforced receipt
- Authority-enforced WorldVersion
- Authority-enforced commit Time
- Authority-enforced World Event
- Authority-enforced Event Log append
- Authority-enforced causal link
- Authority-enforced causal graph
- Authority-enforced replay plan
- Authority-enforced replay cursor
- Authority-enforced replay first step
- Authority-enforced replay completion

## 0.4.x — Snapshot / Fork / Simulation

Verified:

- **v0.4.0** — Immutable World Snapshot Capture
- **v0.4.1** — Immutable World Snapshot Fork
- **v0.4.2** — Fork-Local Immutable State Derivation
- **v0.4.3** — Fork-Local Multi-Change Transaction
- **v0.4.4** — Fork Transaction Receipt

Next:

- **v0.4.5** — Fork-Local WorldVersion Envelope

Remaining direction:

- Fork-local version lineage
- Fork isolation verification
- Effect replay
- Simulation
- World comparison
- Merge
- Conflict reporting

## 0.5.x — Persistence / Recovery / Historical Explanation

Planned:

- Canonical persistence format
- Commit / history log
- Truncation and corruption detection
- Recovery
- Historical explanation

## 0.x — Language completion

Planned:

- General native compiler
- General typed-IR-to-KISA lowering
- Standard library
- Tooling
- Production runtime integration
- Self-hosting
- Bootstrap fixed-point evidence

## 1.0 — Closed Reality Kernel 1.0

The 1.0 scope is complete only when every mandatory subsystem is implemented and verified together.

Target integrated concepts include:

- World
- Entity / Identity
- Immutable State
- Relations
- Transactions
- Time
- Bitemporal History
- Events
- Causality
- Rules
- Constraints / Invariants
- Knowledge / Evidence
- Authority
- Snapshot / Fork
- Replay
- Simulation
- Comparison / Merge
- Persistence
- Historical Explanation

Security, determinism, resource bounds, and provenance are cross-cutting requirements throughout development.
