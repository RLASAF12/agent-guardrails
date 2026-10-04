# FixLoop ⟳

**Turn AI agent corrections into system prompt rules.**

Paste conversations where you had to correct your AI agent. Get exact text to patch your system prompt — nothing to install, no SDK, no account required.

---

## The Problem

Your agent keeps making the same mistake.
You correct it. The session ends.
Next session: same mistake again.

The correction was lost. Your system prompt didn't change.

## How FixLoop Works

```
1. Paste correction snippets
   (conversations where you said "no, I meant..." or "stop doing that")

2. Click Analyze
   (Gemini 2.5-flash diagnoses the instruction gap)

3. Copy the patch
   (exact text ready to append to your system prompt)
```

## Features

- **Root cause classification** — missing constraint, wrong assumption, unclear scope, format issue, and more
- **Before/After preview** — see exactly how the rule changes the agent's behavior  
- **PATCH BLOCK output** — all new rules formatted and ready to copy-paste
- **Zero setup** — bring your own Gemini API key (free at aistudio.google.com)

## Live Demo

🔗 **[rlasaf12.github.io/fixloop/](https://rlasaf12.github.io/fixloop/)**

Enter your [Gemini API key](https://aistudio.google.com/app/apikey) in the top-right corner.

## Use Cases

- You used Claude Code / Cursor and had to repeat yourself 3 times
- Your customer-facing AI agent keeps misinterpreting "recent"
- You corrected an agent's format 10 sessions in a row and want it to stop
- You're building a new system prompt and want to patch in lessons from old sessions

## Stack

- Single HTML file — no build step, no dependencies
- Gemini 2.5-flash via REST API
- Tailwind CSS (CDN)
- User's own API key — no server, no cost to you

## Related

Built by [Ben](https://github.com/RLASAF12) as part of the nightly prototype loop.
See also: [FlowDraft](https://rlasaf12.github.io/flowdraft/), [AgentAudit](https://github.com/RLASAF12/agent-audit)

---

*FixLoop doesn't store your conversations. Everything runs in your browser.*
