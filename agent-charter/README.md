# AgentCharter ⚖️

**AI Deployment Governance Charter Generator**

> Answer the question nobody is asking until it's too late: *Who authorized this agent to act? Who owns the outcome? What triggers human review?*

[**→ Launch AgentCharter**](https://rlasaf12.github.io/agent-charter)

---

## What It Does

AgentCharter is a 5-step web wizard that generates a formal **AI Deployment Governance Charter** — a print-ready document that defines accountability for any AI agent your organization deploys.

**The 5 steps:**
1. **Agent Profile** — name, purpose, systems accessed, autonomous actions
2. **Risk Classification** — Low / Medium / High / Critical + data types handled
3. **Accountability Map** — who authorized it, who owns it, who answers for it
4. **Human Checkpoints** — mandatory escalation triggers, SLAs, fallback actions
5. **Generate** — one-click produces a formatted, print-ready governance document

**Output includes:**
- Named owners with roles
- Hard limits (what the agent can never do)
- Escalation triggers + response SLAs
- Auto-generated governance commitments based on risk level
- Legal disclaimer
- Sign-off section with signature lines

---

## Why It Exists

Five sources confirmed this gap in June 2026:

- "Your AI Agent Made a Decision. Nobody Authorised It. But You Are Still Liable." — [lawandkoffee.substack.com](https://lawandkoffee.substack.com), Jun 24 2026
- "Who Owns the Agent's Mistake?" — [latentmesh.ai](https://latentmesh.ai), Apr 4 2026
- "Who's Liable When Your AI Agent Acts? Founder's Guide" — [njbusiness-attorney.com](https://njbusiness-attorney.com), Jun 16 2026
- "Multi-Agent AI is Outpacing Liability Frameworks" — Berkeley Technology Law Journal, Jun 2 2026
- "Legal Accountability for AI Agents" — Baker McKenzie, Jun 1 2026

Organizations are deploying AI agents that send emails, update records, trigger payments, and make decisions — without any formal accountability structure. When something goes wrong, nobody knows who authorized the agent, who owns the outcome, or what was supposed to trigger human review.

AgentCharter fixes that in 5 minutes.

---

## Tech

Single-file HTML application. No backend. No tracking. No dependencies.

- Pure HTML/CSS/JS
- Print-to-PDF built in (Ctrl+P / Cmd+P)
- Dark UI, works on mobile

---

## Quick Start

```bash
# Option 1: Open directly
open index.html

# Option 2: Deploy anywhere (it's one file)
cp index.html ~/Desktop/AgentCharter.html
```

Or just use the live version: **[rlasaf12.github.io/agent-charter](https://rlasaf12.github.io/agent-charter)**

---

## Who Is This For

- **AI Operators** deploying agents inside their organizations
- **Founders** building AI-powered products
- **Legal / compliance teams** being asked "what governance exists for this agent?"
- **CTOs / VPs of Engineering** who want accountability before something breaks

---

*Built by Ben (prototype builder) as part of the [ABC-TOM](https://github.com/RLASAF12) AI workspace.*
