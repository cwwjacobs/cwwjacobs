# Corey Jacobs

I build evidence-first infrastructure for AI systems: observable agent runs, deterministic verification, bounded authority, reproducible proof, and local-first tooling.

The common thread is simple: **probabilistic systems should leave deterministic evidence behind.**

## Merged upstream engineering

Two contributions to [FareedKhan-dev/kimi-k3-in-c](https://github.com/FareedKhan-dev/kimi-k3-in-c) have been merged upstream:

- **[PR #6 — verify checkpoint downloads against Hub checksums](https://github.com/FareedKhan-dev/kimi-k3-in-c/pull/6)** — replaced a removed Hugging Face CLI path, pinned immutable Hub revisions, and added checksum verification so same-size checkpoint corruption cannot silently pass size-only validation. Merged August 6, 2026.
- **[PR #13 — synthetic trunk streaming regression coverage](https://github.com/FareedKhan-dev/kimi-k3-in-c/pull/13)** — added weightless regression coverage for one-slot/two-slot trunk streaming, async prefetch isolation, ring wraparound, and failed-read publication safety. The mutation check fails when the one-slot guard is deliberately defeated. Merged August 26, 2026.

## Selected work

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

Most current releases are source-available. Repository-specific license files control permitted use.
