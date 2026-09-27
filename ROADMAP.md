# KEY Roadmap

KEY is developed in small verified increments. Each micro-version has a single objective and must pass its acceptance target before advancement.

## Completed / current macro path

### 0.0.x — Native foundation
- Systems IR
- Verifier
- Windows x64 emitter
- Values
- References
- Heap
- Tracing / GC
- Lexer / parser / typed IR
- First source-to-native slice

### 0.1.x — World / Entity / State / Transactions
- World identity
- Entity identity registry
- Immutable state
- Atomic state transitions
- Bounded transactions
- Provenance receipt
- WorldVersion envelope
- Version lineage and lineage chain

### 0.2.x — Time / Events / Causality / Replay
- Explicit Time
- Commit Time binding
- Temporal lineage
- World Events
- Event Log
- Causal links
- Causal graph
- Deterministic replay plan
- Replay cursor

### 0.3.x — Authority-enforced execution path
- Authority Grants
- Operation permits
- Revocation
- Deterministic authority decisions
- Decision Evidence
- Decision Explanation
- Authority-enforced transactions
- WorldVersion publication
- Time publication
- Event publication
- Event Log append
- Causal graph append
- Replay plan and replay completion

### 0.4.x — Snapshot / Fork / Simulation
Current verified baseline:

**v0.4.0 — Immutable World Snapshot Capture**

Next candidate:

**v0.4.1 — Immutable World Snapshot Fork**

Planned direction:
- Fork isolation
- Effect replay
- Simulation
- World comparison
- Merge
- Conflict reporting

### 0.5.x — Persistence / Recovery / Historical Explanation
Planned:
- Canonical storage
- Commit log
- Recovery
- Corruption handling
- Historical explanation

### 0.x — Language completion
Planned:
- General compiler
- Standard library
- Tooling
- Self-hosting
- Fixed-point bootstrap evidence

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
