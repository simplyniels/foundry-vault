Type: #type/concept
Area: #area/craft/ai
Keyword: #keyword/llms #keyword/ai-agents
Date created: [[2026-04-23]]
Sources: [[Boris Cherny Parallel Claude Agents Workflow]], [[Claude Advisor Tool for Cost-Efficient Agents]], [[Artificial Analysis Intelligence Index v4.0]]
Related: [[Agentic AI as Workforce]], [[AI as Conversation Partner Not Oracle]]

---

## What it is

The optimal AI agent strategy is not always-cheapest or always-best-model — it is intelligent routing: small models handle routine execution cheaply, large models are invoked only at decision points that genuinely require their reasoning quality. The key insight is that quality comes from fewer corrections, not from raw generation speed.

## Why it matters

Frontier model costs make fully-agentic pipelines economically marginal when every step uses Opus-class reasoning. Intelligent routing makes them economically viable at scale. The Advisor pattern (Anthropic's platform primitive) makes this server-side with no developer orchestration overhead.

## Key points

- Advisor pattern: Sonnet/Haiku executor → calls Opus only when blocked on a decision → Opus provides plan, correction, or stop signal in the background
- Server-side routing within a single API request — developers get near-Opus quality without orchestration overhead
- Cherny's counterpoint: Opus 4.5 always, because "less steering needed = faster end-to-end than a smaller model" — the correction-time argument
- The bottleneck is human correction time and model self-correction quality, not raw token generation speed
- Benchmark convergence: GPT-5.2 (50pts), Claude Opus 4.5 (49pts), Gemini 3 Pro (48pts) — 2 points separates #1 and #3 across 4 categories
- At frontier convergence, cost-per-quality-unit becomes the primary differentiator — not raw capability
- Cherny and the Advisor pattern are not contradictory: Cherny optimises for single-developer throughput (always use best); Advisor optimises for pipeline cost at scale (route to best only when needed)

## Evidence across sources

- [[Boris Cherny Parallel Claude Agents Workflow]]: human correction time as the real bottleneck; Opus with thinking always; self-verification loop
- [[Claude Advisor Tool for Cost-Efficient Agents]]: formal Advisor pattern; server-side routing; near-Opus quality at fraction of cost
- [[Artificial Analysis Intelligence Index v4.0]]: frontier convergence data — 2 points separates top 3 models; cost table; agent category now benchmarked

## Open questions

- Is Cherny's "always Opus" thesis sustainable as pipeline scale grows? At what point does the cost arithmetic force routing?
- As frontier models converge, does model selection matter less, and orchestration/routing quality more?
- What is the right abstraction for routing rules: task type, confidence threshold, token budget, or something else?

## Prompts

- Map your current AI usage: where are you paying for Opus-level reasoning on Haiku-level tasks? Where are you under-powering decision-critical steps?
- The routing question: if you had to design a router that decided when to call Opus vs. Sonnet vs. Haiku, what signals would it use?
