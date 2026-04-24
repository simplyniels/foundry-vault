Type: #type/concept
Area: #area/craft/ai
Keyword: #keyword/mcp #keyword/ai-tools #keyword/ai-agents
Date created: [[2026-04-23]]
Sources: [[ChatGPT Adds Full MCP App Support]], [[Todoist MCP Integration With ChatGPT]], [[OpenAI Codex Plugin System]], [[Claude Code Telegram Remote Control]], [[Samsung Browser Windows With Perplexity AI]]
Related: [[Agentic AI as Workforce]], [[AI as Conversation Partner Not Oracle]]

---

## What it is

The Model Context Protocol (MCP), originally developed by Anthropic, has become the de facto open standard for connecting AI models to external tools, data sources, and services. OpenAI, Samsung, Todoist, and others have adopted it — signalling cross-industry convergence on a single connectivity layer between AI and the software ecosystem.

## Why it matters

Open protocols create network effects. As more tools expose MCP interfaces, every AI model that speaks MCP gains access to all of them — including models from competing vendors. This is the TCP/IP moment for AI-to-tool connectivity: the plumbing layer that makes the rest of the agentic stack composable.

## Key points

- MCP originated at Anthropic; OpenAI's ChatGPT adoption signals standardisation rather than fragmentation
- Build once (MCP server) → accessible to any MCP-compatible AI model across vendors
- ChatGPT supports MCP app UIs natively; developers can build integrations that work in ChatGPT without ChatGPT-specific code
- Codex Plugins bundle MCP servers + workflows + skills + app integrations into installable packages — shareable environments for teams
- Todoist MCP: natural language → structured task creation, update, review — AI as the interface layer over existing tools
- Claude Code Telegram: Telegram bot as MCP bridge to local agent session — mobile access without custom API work
- Samsung Browser: Perplexity integrated via system-level connection; page context fed into AI agent without user routing it manually
- The convergence pattern: ChatGPT MCP + Codex Plugins + Todoist MCP + Samsung all point to MCP as the integration assumption, not the exception

## Evidence across sources

- [[ChatGPT Adds Full MCP App Support]]: Anthropic-originated protocol adopted by OpenAI — the standardisation signal
- [[Todoist MCP Integration With ChatGPT]]: end-user value: natural language replaces task-manager UI
- [[OpenAI Codex Plugin System]]: MCP servers packaged and distributed as team-shareable bundles
- [[Claude Code Telegram Remote Control]]: MCP as the glue in a mobile-to-local agent bridge
- [[Samsung Browser Windows With Perplexity AI]]: system-level MCP integration; AI understands browsing context without user input

## Open questions

- Will MCP fragment into profiles or dialects as more vendors implement extensions?
- What is the security model at scale? An AI with broad MCP access has read/write capability across many systems — what are the blast-radius implications?
- Does MCP standardisation accelerate or complicate vendor differentiation? (If every AI uses the same protocol, the differentiator shifts entirely to model quality and orchestration)

## Prompts

- Which tools in your current workflow could be MCP-connected? What would natural-language access to your task manager, calendar, or notes vault actually unlock for how you work?
- The security question: if an AI agent had MCP access to every tool you use, what is the worst single mistake it could make? Is your current approval-gate design sufficient?
