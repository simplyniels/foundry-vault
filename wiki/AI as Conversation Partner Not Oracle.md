Type: #type/concept
Area: #area/craft/ai
Keyword: #keyword/llms #keyword/ai-tools #keyword/prompting
Date created: [[2026-04-23]]
Sources: [[ChatGPT Lernen]], [[Clever Gefragt, Prompt Gelöst]], [[Wie KI Dein Leben Besser Macht]], [[Ideen Auf Knopfdruck]], [[Content Creation Mit KI]], [[ChatGPT U. Co.]]
Related: [[Two-layer knowledge systems]], [[Agentic AI as Workforce]]

---

## What it is

Large language models generate statistically probable next tokens — they do not understand, reason, or retrieve facts. The correct mental model is conversational partner: set context, iterate, verify. The incorrect mental model is oracle: ask once, accept output as truth.

## Why it matters

Most poor AI results trace back to a wrong mental model. Treating AI as a search engine produces confident wrong answers with no indication of uncertainty. Treating it as a dialogue partner — one that needs context, feedback, and iteration — produces outputs that compound into real work.

## Key points

- GPT = Generative Pre-trained Transformer: it generates text, it does not retrieve truth
- AI distinguishes statistically probable from improbable — not true from false
- Same prompt, different session → different output (non-reproducible by design)
- Context is everything: feed the AI the text to read before asking questions about it
- "Ask the AI what it needs" — prompt it to interview you before answering; a metacognitive move that front-loads context
- Four-block prompt structure: Role / Task / Context / Output — each block reduces ambiguity
- Thread continuity matters: the session is the work; same conversation = richer context
- Custom Instructions / system prompts: encode what the AI should always know; persistent context reduces re-explanation overhead
- Scale does not equal accuracy: GPT-4's 25,000-word context didn't make it less probabilistic — bigger context, same statistical nature

## Evidence across sources

- [[ChatGPT Lernen]] (Kraus): transformer architecture explained; "ask the AI what it needs"; thread continuity as a feature
- [[Clever Gefragt, Prompt Gelöst]]: four-block framework (Role/Task/Context/Output); context as the primary quality lever
- [[Wie KI Dein Leben Besser Macht]] (Himpsl & von Gehlen): "thinking machine" concept; AI already embedded in daily life before most users noticed
- [[Ideen Auf Knopfdruck]] (Hoffman): GPT-4 as statistical prediction engine; sharp analogy — treat it as a powerful tool not a sentient oracle
- [[Content Creation Mit KI]] (Berens & Bolk): GPT-4 multimodality and context-window scale at launch — still probabilistic
- [[ChatGPT U. Co.]] (Hattenhauer): practical tips; English prompts for image AI; context matters even in image generation

## Open questions

- As context windows expand to millions of tokens, does the "feed it text first" principle still hold, or does the model handle context-finding autonomously?
- Where is the productive boundary between iteration (improving output) and simply compensating for a weak model?
- Does the oracle misunderstanding get worse as AI fluency improves — because confident wrong answers become harder to catch?

## Prompts

- What would your prompting practice look like if you treated every AI session as a dialogue rather than a command? Rewrite your three most common prompts as openings to a conversation.
- The context question: what does your AI not know about your work that it should? Write that as a system prompt.
