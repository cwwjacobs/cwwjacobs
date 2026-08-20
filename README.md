# Corey Jacobs

I build evidence-first systems for tool-using agents: capture what happened, preserve provenance, test adversarial failure modes, and keep operator authority explicit.

Current focus: **agent security, context injection, evaluation infrastructure, reproducible execution evidence, and local-first tooling**.

**GTDataworks** is the main line of work: an evidence pipeline for consequential agent runs, from captured execution to sealed evidence, evaluation receipts, and derived products.  
[gtdataworks.com](https://gtdataworks.com)

## Selected work

- **[Agent Flight Recorder](https://github.com/cwwjacobs/agent-flight-recorder)** — local-first recording for observable tool-using agent runs: model calls, tool calls/results, state snapshots, checkpoints, exports, regression cases, and eval seeds.
- **[Crumple Zone](https://github.com/cwwjacobs/crumple-zone)** — Firecracker-based bounded agent exercises with host-owned mediation, quarantined raw output, trusted event streams, replay, and evidence verification.
- **[GTDataworks Portlock](https://github.com/cwwjacobs/gtdataworks-portlock)** — shipped Linux USB mass-storage policy tool with soft/hard locking, session-lock behavior, attempt logging, `.deb` packaging, and a public apt repository.
- **[DIF Defense](https://github.com/cwwjacobs/dif-defense)** — experimental behavioral prompt-injection detection that evaluates recorded agent behavior against a frozen set of forbidden actions.
- **[GTDataworks-Labyrinth](https://github.com/cwwjacobs/GTDLabyrinth)** — public runtime architecture for captured and sealed agent execution, including a separately constrained range model for cyber environments.

## Open-source contributions

- **[Kimi K3 in C — PR #6](https://github.com/FareedKhan-dev/kimi-k3-in-c/pull/6)** — merged checkpoint-integrity work introducing immutable Hugging Face revision pinning and checksum verification so same-size corruption cannot pass size-only validation. The upstream first-run consolidation later retained and further hardened this path.
- **[Kimi K3 in C — PR #13](https://github.com/FareedKhan-dev/kimi-k3-in-c/pull/13)** — open regression-test contribution for synthetic trunk streaming, including one-slot async-prefetch corruption, ring wraparound, slot isolation, and failed-read publication safety.

## Honorable mentions

- **[Omega Harness](https://github.com/cwwjacobs/omega-harness)** — receipt-bearing, operator-authorized runtime sessions with tamper-evident lineage.
- **[OpenAI Safety Hunt](https://github.com/cwwjacobs/oai-safety-hunt)** — scoped canary-only research harness for indirect prompt injection, MCP/tool-output poisoning, and reproducibility receipts.
- **[Card Forge](https://github.com/cwwjacobs/Card-Forge)** — bounded card/deck workflow tooling with explicit operator approval and provenance rules.
- **[Constellation](https://github.com/cwwjacobs/ixc-constellation)** — local evidence mapping and planned-vs-actual drift receipts for agent-assisted work.

## Working principles

- Evidence before claims.
- Preserve primary artifacts; derive downstream products with lineage.
- Treat untrusted context as data, not authority.
- Make failure states explicit instead of silently widening scope.
- Prefer reproducible receipts over plausible completion narratives.
