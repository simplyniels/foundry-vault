Type: #type/source
Area: #area/craft/ai
Keyword: #keyword/llms #keyword/ai-agents #keyword/ai-tools
Date created: [[2026-04-23]]
Source: https://share.google/SQkx45uhiYNGJkYDS

---

**Summary**
Boris Cherny, creator of Claude Code, revealed a workflow running 5+ Claude instances in parallel — one per terminal tab — turning a single developer into the output equivalent of a small engineering team. The key components are a shared CLAUDE.md for persistent institutional memory, exclusive use of Opus 4.5 with thinking, and subagents for specialised tasks (code simplifier, end-to-end verifier). Every mistake gets encoded back into CLAUDE.md, creating a self-correcting system over time.

**Key points**
- Cherny runs 5 Claude instances in parallel in his terminal, numbered by tab, using system notifications to manage handoffs
- Also runs 5–10 Claudes on claude.ai concurrently, with a "teleport" command to move sessions between browser and local machine
- Uses Opus 4.5 with thinking exclusively — slower but requires less steering, making it faster end-to-end than smaller models
- CLAUDE.md in the git repo captures every mistake as a rule; the longer the team works together, the smarter the agent becomes
- Subagents handle specialised phases: a code-simplifier for architecture cleanup and a verify-app agent for end-to-end testing
- Claude opens a browser, tests the UI via the Chrome extension, and iterates until code and UX both pass — self-verification improves output quality "2–3x"
- The bottleneck is human correction time, not token generation speed; a smarter model that needs less steering is faster in practice
- Developer community reaction described this as a shift from "AI as autocomplete" to "AI as an operating system for labour"

**Claude's notes**
This is a real-world existence proof that agentic parallelism works at the individual-developer level today. The CLAUDE.md as institutional memory is elegant: it externalises context that LLMs lose between sessions and compounds over time. The self-verification loop (agent tests its own work) is the structural move that makes quality sustainable at scale. Connects directly to the broader theme of AI as collaborative workforce rather than typing assistant — compare with the multi-agent ecosystem trend appearing across Samsung, OpenAI, and Google products in this same ingest batch.
