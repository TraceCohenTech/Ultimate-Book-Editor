# The Ultimate Book Editor

An autonomous editorial engine for [Claude Code](https://claude.ai/code). Not a simple grammar checker — a full editorial workflow that captures your intent, researches your market, builds an editorial roadmap, performs multi-pass editing, stress-tests your manuscript, and designs reader engagement elements.

Works on fiction, nonfiction, memoir, hybrid, and workbooks.

## How It Works

The skill operates in structured phases, just like a professional editorial team:

| Phase | What It Does |
|---|---|
| **Intent Capture** | Builds a Taste Profile — your voice, audience, goals, style preferences |
| **Research** | Deploys specialized agents for market data, narrative analysis, voice consistency |
| **Roadmap** | Presents an editorial plan and waits for your approval before editing |
| **Execution** | Multi-pass editing: developmental, line, copy/proof |
| **Production** | Formatting cleanup — quotes, dashes, heading hierarchy, print/Kindle readiness |
| **Engagement** | Designs exercises, prompts, puzzles, and structural devices for retention |
| **Red Team** | Stress-tests the manuscript — finds what critics would attack |

Every phase is optional. The skill runs what's needed based on your manuscript and request.

## Install

```bash
# Personal (available in all projects)
mkdir -p ~/.claude/skills/ultimate-book-editor
cp SKILL.md ~/.claude/skills/ultimate-book-editor/SKILL.md
```

Or for a specific project:

```bash
mkdir -p .claude/skills/ultimate-book-editor
cp SKILL.md .claude/skills/ultimate-book-editor/SKILL.md
```

## Usage

Full editorial review:

```
/ultimate-book-editor manuscript.md
```

Edit a directory of chapters:

```
/ultimate-book-editor ./chapters/
```

Focus on a specific area:

```
/ultimate-book-editor manuscript.md dialogue
/ultimate-book-editor manuscript.md pacing
/ultimate-book-editor manuscript.md character
/ultimate-book-editor manuscript.md engagement
```

Run a specific phase:

```
/ultimate-book-editor manuscript.md intent
/ultimate-book-editor manuscript.md roadmap
/ultimate-book-editor manuscript.md dev-edit
/ultimate-book-editor manuscript.md line-edit
/ultimate-book-editor manuscript.md copyedit
/ultimate-book-editor manuscript.md production
/ultimate-book-editor manuscript.md redteam
```

## The Phases

### Phase 1 — Intent Capture

Before touching a word, the editor builds a **Taste Profile** — understanding your book type, genre, audience, voice, sentence style, emotional targets, and format. If anything is unclear, it runs a **Clarification Quiz** with precise questions like:

- If a reader remembers one idea from this chapter, what should it be?
- Are you optimizing for elegance or accessibility?
- What book would you never want to be compared to?

No heavy edits proceed without directional clarity.

### Phase 2 — Research Agents

Deploys specialized agents when external knowledge would improve quality:

| Agent | Purpose |
|---|---|
| **Market Agent** | Industry trends, comp titles, positioning (nonfiction) |
| **Narrative Agent** | Trope risk, structural alternatives, archetype analysis (fiction) |
| **Voice Agent** | Rhythm, cadence, tone consistency across chapters |
| **Cognitive Load Agent** | Confusion points, density, friction — clarity without dumbing down |
| **Engagement Architect** | Context-aware exercises, puzzles, prompts |

### Phase 3 — Editorial Roadmap

Presents a structured plan before making changes: direction summary, key risks, proposed research, engagement strategy, and pass sequence. Asks for your approval before proceeding.

### Phase 4 — Execution Passes

Three distinct editorial passes, deployed as needed:

**Pass A — Developmental**: Structure, arc, pacing, stakes, character arcs, argument logic. Delivers a prioritized editorial memo with concrete revision steps.

**Pass B — Line Edit**: Sentence clarity, rhythm, voice, show vs. tell, word-level fixes. Delivers clean edits plus 5-10 repeatable writing patterns.

**Pass C — Copyedit/Proof**: Grammar, punctuation, consistency, continuity. Delivers corrections grouped by type with style sheet updates.

### Phase 5 — Production & Formatting

Catches formatting issues: double spaces, heading hierarchy, smart quotes, em/en dashes, orphan/widow risk. Provides format-specific guidance for Word, Kindle, Print, or Markdown.

### Phase 6 — Engagement Architect

Designs reader retention elements that fit your voice and content:

- **Tier 1**: Reflection prompts, micro-summaries, "pause & apply" moments
- **Tier 2**: Decision forks, mini scenarios, spot-the-flaw challenges
- **Tier 3**: Recurring frameworks, chapter-end rituals, workbook inserts, logic puzzles

### Red Team & Integrity Check

Stress-tests the manuscript. Challenges weak claims, flags logical gaps, detects redundancy. Delivers a **Red Team Summary**: the top 3 things a critic would attack, with fixes.

## Focus Areas

| Focus | What It Covers |
|---|---|
| `structure` | Arc, chapter flow, narrative engine |
| `pacing` | Slow sections, rushed beats, rhythm |
| `character` | Arcs, motivation, voice distinctiveness |
| `dialogue` | Authenticity, voice, exposition in speech |
| `prose` | Sentence-level clarity, rhythm, word choice |
| `consistency` | Names, timelines, settings, POV |
| `engagement` | Exercises, prompts, structural devices |

## Philosophy

- Edits within the author's voice, never toward the editor's
- Honest but respectful — assumes the author cares deeply
- Praises specifically, criticizes specifically
- Won't invent problems to seem thorough
- Separates Must-Fix from Optional in every deliverable
- Explains what the manuscript gains from every suggested cut
- Maintains a persistent style sheet across chapters

## License

MIT

## Author

[Trace Cohen](https://x.com/Trace_Cohen)
