Ingest raw material into the Foundry vault.

**Before doing anything**, read `CLAUDE.md` at the vault root for the full rules of engagement. The summary below is a prompt, not the source of truth.

### What to ingest

1. Check `inbox/` for anything unprocessed. Files can be:
   - Raw `.md` clippings from Obsidian Web Clipper
   - PDFs — extract text
   - Plain URLs in a `.md` file — fetch them
   - Pasted text — treat as an article

2. If `$ARGUMENTS` contains a URL or path, ingest that specifically instead of scanning the inbox.

### For each item

1. **Normalise into a source note** at `sources/<Title>.md`. Title is Title Case of the source.
2. **Fill front-matter** per CLAUDE.md:
   - `Type: #type/source`
   - `Area:` — use your best judgment (e.g. `#area/craft/<subarea>` or another top-level area from the taxonomy)
   - `Keyword:` — **read the Keywords section of `wiki/_meta/index.md` first**. Reuse existing keywords. If adding a new one, register it there with a one-line definition.
   - `Date created: [[YYYY-MM-DD]]` — today
   - `Source:` — URL or canonical reference
3. **Write a concise summary** — what's the source saying in 3-5 sentences? What's the core claim?
4. **Extract key points** as a bulleted list — 5-10 items maximum. Be tight.
5. **Add Claude's notes** — one short paragraph on what's interesting, where it connects, what it contradicts. This is where the compile loop will look later.
6. **Create a people page** if the source has an author and no page exists in `wiki/` yet. Keep it thin — a connector node, not an essay. See CLAUDE.md for the three-tier rule.
7. **Cross-reference the companion vault** (if one is configured in CLAUDE.md): scan for notes on the same topic. If any match, mention them in Claude's notes using `[[VaultName/Path/Title]]` style links. Never write into the companion vault.
8. **Clear the inbox**: remove the original once the source note is written.

### Logging

Append to `wiki/_meta/log.md`:

```
## [YYYY-MM-DD] ingest | <one-line descriptor>
- Sources: [[Title]] — one-line descriptor
- Noticed: anything surprising — candidate themes, unusual keywords, contradictions with existing notes
```

Also update the relevant sections of `wiki/_meta/index.md`:
- Add the new source to the Sources catalog
- Increment keyword counts
- If a recurring theme appeared across 2+ sources, add it to Candidates for the compile loop to promote

### Hard rules

- Never write into the companion vault (if configured). Read only.
- Don't create concept articles in this command — that's the compile loop's job. Just get the source notes in clean.
- If the inbox is empty and no argument is given, say so and stop. Don't invent work.

### Arguments

`$ARGUMENTS` — optional. A URL, file path, or keyword. If present, ingest that specific thing. If empty, scan the inbox.
