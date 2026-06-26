# AgentUndo 🔄

**Commit/rollback safety net for irreversible AI agent actions.**

Every agentic system eventually does something that can't be undone — sends an email to 500 customers, deletes production rows, drops a DB column. AgentUndo intercepts those actions and gives you a countdown window to commit or roll back before the irreversible happens.

---

## 🧪 Live Demo

👉 **[rlasaf12.github.io/agent-undo](https://rlasaf12.github.io/agent-undo/)**

---

## What It Does

| Feature | Detail |
|---|---|
| **Action interception** | Queues agent actions before they execute |
| **Risk classification** | Low / Medium / High based on reversibility |
| **Countdown timers** | SVG ring timer — auto-commits if you don't act |
| **Rollback prevention** | Blocks the action and logs exactly what was prevented |
| **Transaction log** | Full audit trail with timestamps |
| **Pre-scripted scenarios** | Email blast, DELETE rows, ALTER TABLE, Slack post, S3 delete, webhooks |

---

## 🎮 Scenarios

```
📧 Email blast → 500 recipients         (HIGH · 120s timer)
🗑️ DELETE 2,412 DB rows                 (HIGH · 120s timer)
🧬 ALTER TABLE in production            (HIGH · 120s timer)
💬 Post to #company-all (890 members)   (MED  · 60s timer)
📁 Delete S3 bucket (12 GB)             (MED  · 60s timer)
🔔 Trigger outbound webhook             (LOW  · 30s timer)
```

---

## 📂 What's Inside

```
agent-undo/
└── index.html     # Complete interactive demo (812 lines, zero dependencies)
```

Single-file. No build step. No backend. Runs on GitHub Pages.

---

## 🚀 Quick Start

```bash
git clone https://github.com/RLASAF12/agent-undo
cd agent-undo
open index.html   # or just double-click it
```

Or fork and deploy to GitHub Pages in one click.

---

## 💡 Why This Exists

The conversation about AI agent trust has focused on **prevention** (don't let the agent do X) and **detection** (alert when X happens). But there's a gap nobody's filling: the window *between* "agent decided to act" and "action executed."

AgentUndo sits in that gap. It's not a firewall. It's a commit log.

> "The bottleneck in agentic workflows isn't code generation speed — it's verification capacity."  
> — HN consensus, June 2026

---

## 🏗️ Agent Trust Layer Series

This is Build #8 in the series:

| # | Tool | Category |
|---|------|----------|
| 1 | AgentGate | Prevention |
| 2 | AgentSentinel | Detection |
| 3 | AgentReceipt | Accountability |
| 4 | agent-breaker | Containment |
| 5 | pr-flood | Containment |
| 6 | agent-postmortem | Diagnosis |
| 7 | AgentDrift | Detection |
| **8** | **AgentUndo** | **Recovery** |

---

Built by [@RLASAF12](https://github.com/RLASAF12) · Security checklist passed 2026-06-27
