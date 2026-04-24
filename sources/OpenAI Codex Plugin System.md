Type: #type/source
Area: #area/craft/ai
Keyword: #keyword/ai-tools #keyword/mcp
Date created: [[2026-04-23]]
Source: https://stadt-bremerhaven.de/openai-codex-erhaelt-plugins/

---

**Summary**
OpenAI added a plugin system to Codex that bundles reusable workflows, skills, app integrations, and MCP servers into installable packages. The structure requires only a `plugin.json` manifest; optional components include skills, `.app.json`, `.mcp.json`, and assets. Native integrations at launch include Slack, Figma, Notion, and Gmail. Aimed at teams that don't want to rebuild their environment setup on every project.

**Key points**
- Codex plugins bundle: workflows + skills + app integrations + MCP servers → one installable package
- Required: `.codex-plugin/plugin.json` manifest; rest is optional
- Launch integrations: Slack, Figma, Notion, Gmail
- Install via Codex UI or CLI via `/plugins`
- Designed for teams needing reproducible, shareable environments

**Claude's notes**
The Codex plugin format essentially standardises how agentic coding environments are packaged and distributed — similar to how VS Code extensions work but for AI agent capabilities. The inclusion of MCP server bundling means plugins can extend the agent's reach to arbitrary external systems. This is the tooling layer that enables agentic workflows to be shared and reproduced across teams, rather than living in one person's terminal config.
