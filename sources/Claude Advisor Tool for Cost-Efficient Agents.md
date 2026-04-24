Type: #type/source
Area: #area/craft/ai
Keyword: #keyword/llms #keyword/ai-agents
Date created: [[2026-04-23]]
Source: https://stadt-bremerhaven.de/claude-advisor-tool-soll-agenten-guenstiger-machen/?utm_source=caschysxlink&utm_medium=social&utm_campaign=Twitter&utm_id=1

---

**Summary**
Anthropic added an Advisor tool to the Claude platform that pairs a smaller executor model (Sonnet or Haiku) with Opus as an advisor. The executor handles the work and calls Opus only when stuck on a decision. Opus provides a plan, correction, or stop signal in the background. The interaction is server-side within a single API request — no extra developer orchestration needed. Claims near-Opus quality at significantly lower cost.

**Key points**
- Pattern: Sonnet/Haiku executes → calls Opus only when blocked → Opus advises in background
- Single API request, server-side orchestration — no developer overhead
- Claims near-Opus intelligence at fraction of cost
- Available as Beta as of April 2026
- Use case: long-running agents where Opus-level reasoning is needed intermittently

**Claude's notes**
The Advisor pattern formalises what many developers already do manually: route hard sub-tasks to a larger model. Making this a platform primitive removes a layer of engineering overhead and normalises hybrid-model agents. The cost implication is significant: if you only pay for Opus on the hard decisions, agentic pipelines become economically viable at much larger scale. This is the infrastructure-level equivalent of Cherny's "use Opus because less steering is faster" insight, applied to cost optimisation.
