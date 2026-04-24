Type: #type/concept
Area: #area/craft/ai
Keyword: #keyword/ai-agents #keyword/llms #keyword/productivity
Date created: [[2026-04-23]]
Sources: [[Boris Cherny Parallel Claude Agents Workflow]], [[Claude Cowork Agentic Tool for Non-Developers]], [[Claude Cowork Dispatch Research Preview]], [[Claude Code Telegram Remote Control]], [[Gemini Task Automation Galaxy S26]], [[Samsung Galaxy AI Multi-Agent Ecosystem]], [[Peter Steinberger Leaves Europe for OpenAI]], [[Claude Advisor Tool for Cost-Efficient Agents]], [[Claude Code Builds Claude Cowork in 1.5 Weeks]]
Related: [[Two-layer knowledge systems]], [[AI as Conversation Partner Not Oracle]]

---

## What it is

AI agents are not assistants you type queries to. They are workers you brief, delegate to, and check in on. The shift is from AI as enhanced autocomplete to AI as managed labour — briefable via natural language, executable in parallel, controllable remotely, and constrained by explicit approval gates before irreversible actions.

## Why it matters

The productivity multiplier from treating AI as parallel workforce rather than conversational tool appears to be 3–10x per knowledge worker (Cherny's one-developer team). The mental model shift — from "I tell it what to write" to "I tell it what to do" — is the unlock. The tools already exist; the adoption lag is conceptual.

## Key points

- Run multiple agents simultaneously on independent work tracks; manage by notification, not by babysitting (Cherny: 5 terminal tabs + 5-10 browser sessions)
- The bottleneck is human correction time, not token speed — a smarter model needing less steering is faster end-to-end
- CLAUDE.md pattern: encode every agent mistake as a rule; institutional memory compounds across sessions and teams
- Approval-gate architecture: AI maximises autonomy up to the irreversible step, then pauses for human confirmation (Cowork, Dispatch, Gemini task automation)
- Self-verification: agent tests its own outputs via browser automation, test suites, bash commands — improves quality 2–3x (Cherny)
- Subagent specialisation: code-simplifier, end-to-end verifier, researcher run in parallel as specialised personas
- Dispatch/remote control: brief from phone → AI executes locally → return to completed work
- OS-level orchestration: Galaxy AI coordinates multiple specialised agents across apps (Samsung) — the platform play
- "Software writes software": Claude Code wrote Claude Cowork; the loop has closed

## Evidence across sources

- [[Boris Cherny Parallel Claude Agents Workflow]]: most detailed data point — 1 human, 5-10 agents, Opus 4.5 always, CLAUDE.md institutional memory, self-verification via Chrome extension
- [[Peter Steinberger Leaves Europe for OpenAI]]: OpenClaw as the consumer proof of concept — full computer control via WhatsApp
- [[Samsung Galaxy AI Multi-Agent Ecosystem]]: OS-level orchestration; 80% of users already use 2+ AI agents; Galaxy AI as coordinator
- [[Claude Cowork Agentic Tool for Non-Developers]], [[Claude Cowork Dispatch Research Preview]], [[Claude Code Telegram Remote Control]]: the mobile-to-desktop execution chain
- [[Gemini Task Automation Galaxy S26]]: the consumer-facing execution proof — Gemini orders your Uber
- [[Claude Advisor Tool for Cost-Efficient Agents]]: routing pattern for sustainable agentic economics
- [[Claude Code Builds Claude Cowork in 1.5 Weeks]]: agentic velocity empirical data point

## Open questions

- What is the right human-to-agent ratio? Cherny runs 1:10. Does it scale linearly, or does coordination overhead cap it?
- Where does the approval-gate pattern break down? At what task frequency does "pause for review" become the bottleneck?
- What does the CLAUDE.md pattern look like at team scale? Who owns the rules?
- European regulatory friction (Steinberger): structural disadvantage or temporary lag?

## Prompts

- Map your current workday to the agentic model: what are you doing today that an agent could do without you? What is the first thing to delegate?
- The CLAUDE.md question: what are the three rules your current AI sessions keep forgetting that you could encode today — and what would that compounding look like in six months?
- Write the briefing doc you'd give a new AI agent joining your workflow, the way you'd brief a junior hire on day one.
