# AgentAmb — Instruction Ambiguity Expander

> Paste any instruction you would give an AI agent. See every interpretation it might take — including the ones that delete your database.

## What It Does

AgentAmb takes a single ambiguous instruction and expands it into all plausible agent interpretations, ranked by blast radius from **CATASTROPHIC** (irreversible system damage) down to **SAFE** (read-only analysis).

## The Kiro/AWS Incident

On June 18, 2026, an engineer told Kiro: `"clean up the cost explorer"`.

The agent deleted the billing data export configuration. AWS lost 6.3M orders over 13 hours. The instruction was ambiguous. The agent was not.

AgentAmb lets you see this happening before it happens to you.

## Blast Radius Levels

| Level | Color | What It Means |
|-------|-------|---------------|
| CATASTROPHIC | 🔴 | Irreversible system damage |
| HIGH | 🟠 | Data loss or extended downtime |
| MEDIUM | 🟡 | Recoverable but disruptive |
| LOW | 🔵 | Minimal impact, reversible |
| SAFE | 🟢 | Read-only, no state change |

## Live Demo

Open `index.html` in any browser — no server needed. Pre-loaded with 5 real scenarios.

Enable **Live Mode** by adding a Gemini API key to analyze your own instructions.

## Part of the Agent Safety Series

| Project | What It Does |
|---------|-------------|
| [AgentReceipt](https://github.com/RLASAF12/agent-receipt) | MCP transport tracing |
| [agent-postmortem](https://github.com/RLASAF12/agent-postmortem) | Causal failure graph for agent failures |
| [AgentDrift](https://github.com/RLASAF12/agent-drift) | Reasoning drift detector |
| [AgentUndo](https://github.com/RLASAF12/agent-undo) | Commit/rollback countdown for agent actions |
| **AgentAmb** | ← You are here: Instruction ambiguity expander |

## Quick Start

```bash
# No install needed — just open in browser
open index.html
```

## Built By

[Harel Asaf](https://harelasaf.com) · AI Operator · Nightly Build 2026-06-28

