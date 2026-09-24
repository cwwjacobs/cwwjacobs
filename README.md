# Corey Jacobs

I build evidence-first infrastructure for AI systems: observable agent runs, deterministic verification, bounded authority, reproducible proof, and local-first tooling.

The common thread is simple: **probabilistic systems should leave deterministic evidence behind.**

## Upstream contributor — kimi-k3-in-c

I contribute to [FareedKhan-dev/kimi-k3-in-c](https://github.com/FareedKhan-dev/kimi-k3-in-c), a low-level C inference project where checkpoint integrity, buffer ownership, streaming, and memory behavior can directly affect model correctness.

Two of my changes have been merged upstream:

- **[PR #6 — verify checkpoint downloads against Hub checksums](https://github.com/FareedKhan-dev/kimi-k3-in-c/pull/6)** — repaired the downloader around the supported Hugging Face CLI, pinned immutable Hub revisions, and added checksum verification so a same-size corrupted checkpoint cannot silently pass size-only validation. The verification path was explicitly tested by changing a byte without changing file size and confirming the corruption was rejected. Merged August 6, 2026.
- **[PR #13 — synthetic trunk streaming regression coverage](https://github.com/FareedKhan-dev/kimi-k3-in-c/pull/13)** — added checkpoint-free regression coverage for one-slot and two-slot trunk streaming, asynchronous prefetch isolation, ring wraparound, slot ownership, and failed-read publication safety. A mutation test deliberately defeats the one-slot guard and must fail, proving the regression test can actually detect the ownership error it protects against. Merged August 26, 2026.

Both changes turn silent correctness risks into explicit, testable invariants: **byte integrity at the checkpoint boundary and buffer ownership at the streaming boundary.**

## Selected work

### [cindermote](https://github.com/cwwjacobs/cindermote)
Collapse-ready runtime for untrusted agent material inside disposable Firecracker microVMs. Every run is bounded, observed, and burnable: receipts at the boundary, nothing persistent by default. Apache-2.0.

### [Local Eval Foundry](https://github.com/cwwjacobs/local-eval-foundry)
Deterministic, provenance-bound AI evaluation infrastructure. Sealed scoring, reproducible benchmark packs, and auditable run receipts — evals that can be replayed, challenged, and verified instead of trusted.

### [Agent Flight Recorder](https://github.com/cwwjacobs/agent-flight-recorder)
Local-first observability for tool-using agents. Captures model calls, tool activity, state, checkpoints, replay evidence, exports, regression cases, and eval seeds.

### [Terminus Release Protocol](https://github.com/cwwjacobs/terminus-release-protocol)
Evidence-backed release machinery for AI capabilities. Runs controlled baseline/augmented pairs, admits claims through deterministic proof, and only renders release media after the evidence survives independent verification.

### [Zero Authority Witness](https://github.com/cwwjacobs/zero-authority-witness)
A receipt-bearing intake boundary for untrusted content. Converts external input into evidence-only data before LLM reasoning or action, with explicit authority and action gates.

### [Card Forge](https://github.com/cwwjacobs/Card-Forge)
Reusable workflow Cards, Stacks, Decks, Runs, and Receipts for AI-assisted work. Built around bounded instructions, provenance, operator approval, and portable execution packets.

### [Terminus XI Protocol](https://github.com/cwwjacobs/terminus-xi-protocol)
Deterministic watchdogs and admission rules for probabilistic systems. XI evaluates evidence against named boundaries and emits explicit ADMIT / REJECT outcomes with integrity receipts.

### [LocalParse](https://github.com/cwwjacobs/LocalParse)
A local-first JSON and JSONL browser tool. No backend, no account, no telemetry, and no upload path: files stay in the browser while you inspect, navigate, and export them.

## What I care about

- Evidence before claims
- Untrusted context as data, never implicit authority
- Reproducible receipts instead of plausible completion narratives
- Explicit failure states instead of silent scope expansion
- Local-first and operator-controlled workflows
- Systems that can be inspected, replayed, challenged, and verified

## Contact

**Corey Jacobs**  
Commercial licensing / project inquiries: **coresynth@gmail.com**

Most current releases are source-available under the PolyForm Noncommercial license (cindermote is Apache-2.0). Repository-specific license files control permitted use.
