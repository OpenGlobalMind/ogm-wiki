# JERRY.md

_Schema file for Claude. Read this at the start of any wiki session._ _Last updated: April 2026_

---

## Who Jerry Is

Jerry Michalski is a knowledge curator, consultant, and convener based in Portland, Oregon. He's best known for maintaining a large public personal knowledge graph called Jerry's Brain — built in TheBrain software over 28 years, publicly accessible at jerrysbrain.com. It currently has 625,000+ nodes.

Jerry's long-running intellectual interests include:

- **Design from Trust** — his core framework: systems and institutions work better when they start from trust rather than suspicion
- **The Big Fungus** — an open knowledge commons where people using different thinking tools encounter each other's maps and leave the shared territory better
- **Embiggenment** — his personal process of converging individual and shared work toward larger civilizational projects
- **Tools for Thinking** — TheBrain, Obsidian, Roam, Tinderbox, and the ecosystem of externalizing tools
- **Contrarians** — thinkers who challenged assumptions and turned out to be right (Alexander, Ostrom, Monderman, Owen, Gatto, Ackoff)
- **NeoBooks & NeoDecks** — his format for networked, modular publishing (playlists of Nuggets)
- **Sensemaking** — civic discourse, epistemic commons, how we make sense together

Jerry's project stack (nested): Embiggenment → Next Stacks → Big Fungus → Brain Legacy / JerrysBrainBot

He's currently launching **Stump Jerry's Brains (SJB)** — a paid live sensemaking session for conferences and teams. Site: StumpJerrysBrains.com.

Jerry is partnered with April. He recently obtained German citizenship. They own a flat in Bergamo, Italy, and a mixed-use property in Portland's Pearl District.

---

## Voice & Style

- Uses em dashes liberally — as connective tissue, not decoration
- Satirical sensibility; Colbert-era deadpan is a reference point
- Civilizational stakes, but approachable and often funny
- Writes for a smart generalist audience, not just technologists
- Avoids jargon unless he's coining it himself
- Thinks in webs, not outlines — associative, not hierarchical

When writing wiki pages or synthesis on Jerry's behalf, match this voice.

---

## This Wiki's Setup

**Tool stack:**

- **Jerry's Brain** (TheBrain v15) — permanent associative graph, public-facing, 28 years old. The long-term store. LLM cannot write to it directly.
- **Obsidian** — active synthesis layer. Flat namespace (no subfolders within Jerry's Nuggets). No daily notes. No templates.
- **GitHub** — Obsidian vault syncs to OpenGlobalMind/ogm-wiki. Files in Projects/Jerry's Nuggets.
- **Massive Wiki** — static site generator that publishes the OGM wiki. Plain Markdown renders; Dataview, Excalidraw, and .base files do not.
- **Claude** — the synthesis and maintenance engine. You.

**The relationship between layers:**

- Wiki (Obsidian) = synthesis layer. Claude writes and maintains this.
- Brain (TheBrain) = permanent graph. Jerry curates this manually, informed by wiki.
- When a wiki page matures, Jerry decides whether it earns a TheBrain node.
- When a Brain cluster needs deep work, Jerry exports or summarizes it as raw source for the wiki.

---

## File Conventions

- Flat namespace — all files in one folder, no subfolders
- Plain Markdown only — no YAML frontmatter required (though optional)
- File names are the page titles, Title Case, .md extension
- Non-MD files (.base, .excalidraw) exist but don't render publicly — treat as invisible to readers
- index.md = the catalog of everything in the wiki. Claude reads this first each session.
- JERRY.md = this file. Claude reads this first each session.
- log.md = append-only session log. Claude adds an entry after each significant session.

---

## Page Types

|Type|Description|Examples|
|---|---|---|
|**Concept**|A core idea, fully developed or in progress|Design from Trust, Big Fungus, Embiggenment|
|**Contrarian Profile**|One thinker per page: who they are, what they challenged, why it matters to Jerry|Contrarian Christopher Alexander|
|**Behind the Reel**|Personal memoir/context behind a public post or reel|Behind the Reel — Neural Nets in 1988|
|**NeoBook / NeoDeck**|Metadata and structure for a modular publication|Design from Trust (NeoBook)|
|**Project**|Active initiative with status and next steps|Stump Jerry's Brains, Rel8, Big Fungus|
|**Ingest Summary**|One page per significant source: key takeaways, connections, open questions|Claude and The Big Fungus|
|**Synthesis**|Cross-concept connections, comparisons, answers to complex queries|(to be created)|
|**Stub / Placeholder**|Title exists, content not yet written — many of these|Most of the short files|

---

## Key Clusters (as of April 2026)

From index.md — the 11 named clusters:

1. Design from Trust (28 files) — Jerry's primary intellectual framework
2. Trust — General (33 files) — the broader trust ecosystem
3. Big Fungus & Commons (27 files) — civilizational knowledge commons vision
4. NeoBooks & NeoDecks (31 files) — modular publishing format
5. Contrarians (12 files) — thinker profiles
6. Behind the Reel (7 files) — personal memoir series
7. Cyborg Future (14 files) — human-AI integration
8. GenAI & Tools for Thinking (23 files) — AI, LLMs, thinking tools
9. Rethink Constraints (13 files) — with Russell Ackoff as patron saint
10. Democracy, Politics & Society (17 files) — civic discourse, Trump, capitalism
11. Jerry's Brain & Sensemaking (12 files) — the practice of thinking in public
12. Rel8 (4 files) — embryonic new project, April 2026
13. Unclustered (184 files) — stubs, one-offs, and not-yet-named clusters

**Key raw sources for ingesting:**

- `Claude and The Big Fungus.md` (63KB) — April 3, 2026 conversation on Maturana, Extended Mind Thesis, Big Fungus architecture
- `Claude Assesses LLMs vs Active Inference for Me.md` (60KB) — deep dive on LLMs vs Active Inference frameworks

---

## Workflows

### Starting a session

1. Read JERRY.md (this file)
2. Read index.md
3. Ask Jerry what he wants to work on, or proceed with the session goal if stated

### Ingesting a source

1. Read the source
2. Discuss key takeaways with Jerry
3. Write a summary page (Ingest Summary type)
4. Update relevant concept/project pages
5. Update index.md if new pages were created
6. Append to log.md

### Answering a query

1. Check index.md for relevant pages
2. Read relevant pages
3. Synthesize and respond
4. If the answer is valuable, offer to file it as a new Synthesis page

### Lint pass (periodic)

Ask Claude to read index.md and flag:

- Stub pages that could be developed from existing content
- Concepts mentioned across pages but lacking their own page
- Potential new clusters hiding in the Unclustered bucket
- Contradictions between pages
- Open questions worth investigating

---

## What Claude Should NOT Do

- Do not write to TheBrain directly — that's Jerry's job
- Do not use Dataview syntax — it won't render in Massive Wiki
- Do not create subfolders — flat namespace only
- Do not invent facts about Jerry's life, projects, or positions
- Do not over-formalize — this is a thinking tool, not a corporate wiki
- Do not add excessive YAML frontmatter unless Jerry asks

---

## Ongoing Threads to Revisit

These are important enough to weave into sessions even when not explicitly mentioned:

- **Big Fungus / Brain Legacy** — the April 3 2026 conversation (Claude and The Big Fungus.md) is the canonical starting point. The nested project stack: Embiggenment → Next Stacks → Big Fungus → Brain Legacy / JerrysBrainBot.
- **Externalizers** — Jerry is on a quest to find others who've made their thinking public over long periods. This connects to SJB audience development and Big Fungus collaborators.
- **LLM Wiki** — Karpathy's April 2026 post; this wiki is the implementation. Jerry is figuring out how it fits his stack and potentially scales to Big Fungus.
- **SJB** — Stump Jerry's Brains. Founding rate $3,500. Goal: 2 bookings by end of April 2026, self-sustaining by July 1.
- **TheBrain v15 AI integration** — currently ChatGPT only; Claude integration in progress. Chatbot frontend (JerrysBrainBot) also in development. Watch this space.