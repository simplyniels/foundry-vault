Type: #type/source
Area: #area/craft/ai
Keyword: #keyword/ai-tools #keyword/mcp
Date created: [[2026-04-23]]
Source: https://stadt-bremerhaven.de/claude-code-mit-telegram-steuern/

---

**Summary**
An official Claude Code plugin routes a Telegram bot as an MCP server, forwarding messages to a running Claude Code session. This enables mobile control of Claude Code from anywhere — replies, reactions, and message editing are all supported. Limitations: Telegram's Bot API provides no message history or search, so older context must be manually re-supplied.

**Key points**
- Official plugin: Telegram bot → MCP server → Claude Code session bridge
- Supports replies, emoji reactions, editing sent messages
- Photos saved locally and directly processable by Claude
- Limitation: no message history or search via Telegram Bot API — stale context must be pasted manually
- Commentary: Claude Code + Dispatch + Telegram ≈ a commercialised OpenClaw-style product

**Claude's notes**
The Telegram integration is the mobile arm of the Dispatch pattern: persistent AI session running locally on a machine, controllable remotely from a phone. The journalist's observation — "with Dispatch, Telegram and Co., Claude Code is becoming a commercialised OpenClaw" — is astute. Anthropic is assembling the same capability stack that Steinberger built as a weekend project, but at enterprise scale and with a better UX surface.
