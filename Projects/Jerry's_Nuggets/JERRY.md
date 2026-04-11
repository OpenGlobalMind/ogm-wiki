# JERRY.md
*Schema file for Claude. Read this at the start of any wiki session.*
*Last updated: April 2026*

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
- **Externalizers** — people who have made their thinking public over long periods; Jerry is on a quest to find and convene them

Jerry's project stack (nested): Embiggenment → Next Stacks → Big Fungus → Brain Legacy / JerrysBrainBot

He's currently launching **Stump Jerry's Brains (SJB)** — a paid live sensemaking session for conferences and teams. Site: StumpJerrysBrains.com.
- Founding session rate: $3,500 (active offer, framed as founding rate not a discount)
- Full public pricing: $7,500 virtual (+$1,000 Teams surcharge), $12,500–$15,000 custom keynote, $20,000+ advisory half-day
- Goal: 2 bookings by end of April 2026; self-sustaining revenue by July 1

Jerry is partnered with April. He recently obtained German citizenship. They own a flat in Bergamo, Italy, and a mixed-use property in Portland's Pearl District.

---

## Voice & Style

- Uses em dashes liberally — as connective tissue, not decoration
- Satirical sensibility; Colbert-era deadpan is a reference point
- Civilizational stakes, but approachable and often funny
- Writes for a smart generalist audience, not just technologists
- Avoids jargon unless he's coining it himself
- Thinks in webs, not outlines — associative, not hierarchical
- Prefers "we" framing when talking about civilizational projects
- Strong comedic voice — don't sand it off when writing on his behalf

When writing wiki pages or synthesis on Jerry's behalf, match this voice.

---

## How Jerry Likes to Work with Claude

- **Creative director / implementer relationship** — Jerry describes what he wants in plain language; Claude produces built artifacts to review
- **Ask clarifying questions before going into detail** — don't dive into a long output when a quick question would save time
- **Favor no-code or low-code solutions** — Jerry can edit sites without bureaucracy but isn't a developer
- **Produce files, not just text** — when producing wiki pages or documents, create actual Markdown files
- **Don't over-format** — avoid excessive bullet points and headers in conversational responses; prose is fine
- **One question at a time** — when clarification is needed, ask one question, not five

---

## This Wiki's Setup

**Tool stack:**
- **Jerry's Brain** (TheBrain v15) — permanent associative graph, public-facing, 28 years old. The long-term store. LLM cannot write to it directly. Currently integrates with ChatGPT; Claude integration in progress. A public chatbot frontend (JerrysBrainBot) is also in development.
- **Obsidian** — active synthesis layer, co-authored by Jerry and Claude. Flat namespace (no subfolders within Jerry's Nuggets). No daily notes. No templates currently in use.
- **Obsidian Git plugin** — automatically syncs the vault to GitHub on commit. Configured with write access.
- **GitHub** — vault syncs to OpenGlobalMind/ogm-wiki. Files live at Projects/Jerry's Nuggets/
- **Massive Wiki** — static site generator that publishes the OGM wiki as a website. Plain Markdown renders; Dataview, Excalidraw, .base files, and YAML frontmatter do not render publicly.
- **Obsidian Bases** — spreadsheet-style views inside Obsidian, driven by YAML frontmatter. Internal use only; does not render publicly. This is Jerry's post queue management tool.
- **Claude** — synthesis and maintenance engine. You.

**The relationship between layers:**
- Wiki (Obsidian) = synthesis layer, co-authored by Jerry and Claude
- Brain (TheBrain) = permanent graph, curated manually by Jerry
- When a wiki page matures, Jerry decides whether it earns a TheBrain node
- When a Brain cluster needs deep work, Jerry exports or summarizes it into Obsidian as raw source

---

## File Conventions

- Flat namespace — all files in Projects/Jerry's Nuggets, no subfolders
- Plain Markdown with YAML frontmatter (see YAML section below)
- File names are page titles, Title Case, .md extension
- Non-MD files (.base, .excalidraw) exist but don't render publicly
- **index.md** — catalog of everything in the wiki; Claude reads this each session
- **JERRY.md** — this file; Claude reads this each session
- **log.md** — append-only session log; Claude appends after significant sessions
- **RC Posts.md** — Jerry's manually maintained post queue by series; being superseded by Bases + YAML

---

## YAML Frontmatter

YAML is used for Obsidian Bases views and internal tracking. It does not render publicly. Claude should add YAML to every file it creates or substantially edits. Body content must always stand alone — never put critical information only in YAML.

**Standard YAML block:**
```yaml
---
status: stub
series: []
tags: []
posted:
---
```

**`status` values:**
- `stub` — title exists, little or no content yet
- `draft` — content in progress
- `ready` — ready to post
- `posted` — published; fill in `posted:` date (YYYY-MM-DD)

**`series` values** (use the hashtag labels below — one file can belong to multiple series):
- `RethinkConstraints`
- `DesignfromTrust`
- `TheBigFungus`
- `GenAI`
- `GenAI+FoW` (GenAI + Future of Work)
- `wiwty` (What If We Trusted You)
- `NeoBooks`
- `JoyLine`
- `Contrarians`
- `BehindTheReel`
- `TechHistory`
- `RethinkSociety`
- `CurrentEvents`
- `TrumpFieldManual`
- `ConstraintTales`
- `Innovation`
- `4S` (See, Shift, Shape, Set)
- `JerrysBrain`
- `OGM`
- `Rel8`
- `SJB`
- `BigPicture`
- `Context`
- `Meta`

**`tags` values** (topic labels, distinct from series):
design-from-trust · trust · big-fungus · commons · cyborg · genai · tools-for-thinking · contrarians · neobooks · neodecks · sensemaking · rethink-constraints · democracy · politics · sjb · externalizers · llm-wiki · behind-the-reel · rel8 · abundance · cities · media · masculinity · capitalism · joy-line · 4s · innovation

**Note on stubs:** Files that exist only as ideas (no content yet) should have `status: stub`. This makes them visible in Bases views even before they're written. When Claude encounters an idea in RC Posts or elsewhere that doesn't have a file yet, it should flag it as a stub candidate.

---

## Page Types

| Type | Description |
|---|---|
| **Concept** | A core idea, developed or in progress |
| **Contrarian Profile** | One thinker: who they are, what they challenged, why it matters |
| **Behind the Reel** | Personal memoir/context behind a public post or reel |
| **NeoBook / NeoDeck** | Metadata and structure for a modular publication |
| **Project** | Active initiative with status and next steps |
| **Ingest Summary** | One page per significant source processed with Claude |
| **Synthesis** | Cross-concept connections, answers to queries worth keeping |
| **Stub** | Title and YAML only; content not yet written |

---

## Publication Series & Cluster Map

This is the authoritative map of Jerry's publishing series, melding RC Posts.md (his manual queue) with topic clustering. Each series has a hashtag used across platforms.

### #RethinkConstraints
The parent series. Everything else is a sub-series or feeds into this.
- Tech History: General Magic's Two Fatal Flaws · When I Sent My First Wireless Email
- Constraint Tales: The Web Is Forgiving · Ackoff Was a Master · Brands Are Trapped · How the Robocar Trifecta Would Improve Our Cities · Watching Travelers Eat Citibank
- 4S (See, Shift, Shape, Set): The 4S Innovation Process · Seeing Constraints · Shifting Your Perspective · Shaping Your Future · Setting Your Course
- Innovation: The Dark Side of Innovation · My Innovations · Dark Innovation · Types of Innovation · Other Kinds of Innovation
- Big Picture: Fighting Over the Joystick · This Project's Goals · Questions for Those With Projects to Fix the World · Does Ethical Capitalism Pencil Out · Rethinking My Own Constraints · Impossible Is Just the Most Famous Constraint

### #DesignfromTrust
Jerry's primary intellectual framework series.
- Posted: My Story of Trust · Trust is… · The Alternatives to Sorting Out Trust All Suck · Wikipedia Started as the Nupedia · Trust Is Cheaper Than Control · Design from Trust Is Widespread Already · From Trust, Not For · Oh Advertisers 1 & 2
- Queue: Design from Trust — How to Build Better Futures · Design from Trust Requires Thoughtful Design · Trust Just Feels Better · Scarcity = Abundance — Trust · The Joy Line · Jerry's Trust Summary · But Trust Doesn't Scale · How We Receive Matters · People are Generally More Trustworthy Than We Think They Are · Be Undefended Not Defenseless · Not Naïve Trust · But That Won't Work Here · Trust's Many Facets · Trust In Today's Political Arena · We Are Often Blind to Design from Trust · The 2 Oh Shit!s · Why You Love Design from Trust Already · Pointing Out the Pattern · Design from Mistrust · Reality Check · Design from Trust as a Differentiator · Trust Is the (Only) Way Forward · Undermining Trust Is a Strategy · The Big Picture — Effects of Design from Trust · Design from Trust is Corruptible · Examples of Design from Trust · Benefits of Design from Trust · Principles of Design from Trust · Trust Unlocks Innovation · Design Thinking and Design from Trust · Design from Trust as a Methodology · Writing a NeoBook About Design from Trust
- Ideas without files yet: We Normalized Mistrust · Trust Is the Crucial Constraint

### #TheBigFungus
- Fabulous Fungal Metaphors · Leaf-Cutter Ants Can't Digest Leaves · Joy and Jerry Discuss The Big Fungus · Help me Feed the Big Fungus · On Curating a Long-Term Memory
- All fungal metaphor files (Mycelia, Hyphae, Mushrooms, etc.)
- Collections to Feed the Big Fungus · The Fungus Manifesto · The Commons · Nurture the Commons

### #GenAI
- GenAI's Mixed Blessings (posted) · Tech Owes You an Apology · GenAI Gives Us Superpowers · Does GenAI Obsolete Notetaking · Does GenAI Obsolete Tools for Thinking · Does GenAI Obsolete Reading · On GenAI's Origins · Finding Your GenAI Advisors · GenAI Trust Issues · Proposing a GenAI Compact

### #GenAI+FoW (GenAI + Future of Work)
- GenAI Automates Tasks, Not Jobs · The Elephant in the GenAI Room · GenAI Is Like a Flesh-Eating Bacterium · The Future isn't AI — It's CHI · Will GenAI Survive Capitalism · Will Capitalism Survive GenAI
- Ideas without files: The GenAI-Jobs-Education Trilemma

### #wiwty (What If We Trusted You)
- What If We Trusted You (NeoBook) and related files

### #NeoBooks
- PowerPoints Should be Playlists · What's a NeoBook · What's a Nugget · Nuggets Are Really Powerful · Nuggetization · The Unwritten Laws of Books · How Books Fail Us · The NeoBooks Manifesto · Level Up Media · The Creator's Dilemma · Why Hasn't Software Solved Collaboration · Making Ideas More Useful · Jerry's Presentation Nuggets · Knowledge Should Accumulate · The History of Sensemaking
- Ideas without files: Bonfires on the Horizon · Smelling the Web · Smelling Smartphones · Apps atop shared warm data

### #JoyLine
- The Joy Line · The Joy Line in Health Care

### #Contrarians
- A Worldview Built from Contrarians · Contrarian Overview · Contrarian or Kook · Contrarians Who Make (or Made) Sense · How I Became Aware of Contrarians · Introducing My Contrarians · Patterns My Contrarians Share
- Profiles: Christopher Alexander · Elinor Ostrom · Hans Monderman · Harrison Owen · John Taylor Gatto · Russell Ackoff
- Ideas without profiles: more to add

### #BehindTheReel
- Behind the Reel (series) · Neural Nets in 1988 · Design from Trust · Slides on Acetates · The Documents That Saved My Family · The Joy Line · What Seems Impossible

### #TechHistory
- General Magic's Two Fatal Flaws · When I Sent My First Wireless Email
- "This Changes Everything" sub-series: Social Media Was Different before Facebook Got Its VC · Microfinance Was Different before Capitalists Discovered It · The Sharing Economy Was Different before Uber · Multiple Promising Technologies Were Warped by Capitalism

### #RethinkSociety
- Rethink Masculinity · Ownership versus Stewardship · Let's Treat Refugees as First-class Global Citizens

### #CurrentEvents / #TrumpFieldManual
- This Kamala Moment (done) · Kayfabe · OODA · DARVO · Kayfabe, OODA, DARVO — Why Democrats Are Clueless · Misunderestimating Donald Trump · Trump II Is Teaching a Masters Class · On Trump and Constraints · Trump Through the Trust Lens

### #JerrysBrain
- On Curating a 28-Year-Old Mind Map · Enumerated Wisdom · isms · Contrarians Who Make (or Made) Sense · Useful Thinking Frameworks and Mental Models · Variants of Capitalism · Communities Working to Fix World Problems

### #OGM (Open Global Mind)
- The OGM Birth Story · OGM Effects (if we succeed) · Running a QFT on Curiosity

### #Rel8
- Introducing Rel8 · Rel8 · Rel8 Founding Steward's Charter · Rel8 Manifesto

### #SJB (Stump Jerry's Brains)
- All SJB-related posts, outreach, and documentation
- Finding the Externalizers (post drafted April 2026)
- LLM Wiki / Karpathy response (video outline drafted April 2026)

### Context & Meta Posts (not hashtagged separately)
- On Crossposting (done) · I Think in Webs · Rethinking My Own Constraints · On the Nature of Constraints · On Sensemaking · Getting My Kite Out of Storage
- Ideas without files: On Constraints and Strategy · A Map to This Project · My Missions · About This Substack · The Many Flavors of Capitalism · Help me shape this offer · Wrestling With Where I Fit

---

## Key Raw Sources to Ingest

- `Claude and The Big Fungus.md` (63KB) — April 3 2026. Primary source on Big Fungus, Maturana, Extended Mind Thesis.
- `Claude Assesses LLMs vs Active Inference for Me.md` (60KB) — LLMs vs Active Inference.
- `RC Posts.md` — Jerry's manual post queue; being superseded by Bases + YAML but still the most complete picture of publication intent.

---

## Workflows

### Starting a session
1. Read JERRY.md (this file)
2. Read index.md
3. Ask Jerry what he wants to work on, or proceed with stated goal

### Ingesting a source
1. Read the source with Jerry
2. Discuss key takeaways
3. Write a summary page (type: ingest) with YAML
4. Update relevant concept/project pages
5. Update index.md if new pages were created
6. Append to log.md

### Answering a query
1. Check index.md for relevant pages
2. Read relevant pages
3. Synthesize and respond
4. If valuable, offer to file as a Synthesis page

### Lint pass (periodic)
Flag: stubs ready to develop · concepts without pages · new clusters in Unclustered · contradictions · ideas in RC Posts without stub files · YAML missing from older files

---

## What Claude Should NOT Do

- Do not write to TheBrain directly
- Do not use Dataview syntax — won't render in Massive Wiki
- Do not create subfolders — flat namespace only
- Do not invent facts about Jerry's life, projects, or positions
- Do not over-formalize — this is a thinking tool, not a corporate wiki
- Do not put critical content only in YAML — body must stand alone

---

## Ongoing Threads to Revisit

- **Big Fungus / Brain Legacy** — April 3 2026 conversation is canonical. Stack: Embiggenment → Next Stacks → Big Fungus → Brain Legacy / JerrysBrainBot.
- **Externalizers** — quest for people who've made thinking public over long periods. SJB audience + Big Fungus collaborators. Post drafted April 2026.
- **LLM Wiki** — Karpathy's April 2026 post. This wiki is Jerry's implementation. May scale to Big Fungus. Video outline drafted.
- **SJB** — Stump Jerry's Brains. Founding rate $3,500. Goal: 2 bookings by end of April 2026, self-sustaining by July 1.
- **TheBrain v15 AI** — ChatGPT now, Claude coming. Public JerrysBrainBot chatbot in development.
- **NeoBooks / NeoDecks / publishing vision** — a PowerPoint-killer and modular publishing format, predates and differs from Marp. Jerry wants to explain this properly when the time is right.
- **Bases + YAML project** — goal is to replace the manually maintained RC Posts.md with a live Bases view showing all posts by status, series, and date. YAML needs to be applied consistently across files. Stubs needed for ideas without files.
- **GWRE** — GlobalWarmingRealEstate.com satirical rebuild. On hold until SJB generates revenue.
- **Portland property** — mixed-use Pearl District, listed without success, unconventional marketing being considered.
