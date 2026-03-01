# Top Book Editor

A professional-grade book editing skill for [Claude Code](https://claude.ai/code). Get developmental and line-level editorial feedback on your manuscripts — fiction, non-fiction, memoir, or genre writing.

## What It Does

Run `/top-book-editor` on any manuscript file and get a full editorial report covering:

- **Developmental editing** — structure, arc, pacing, character, argument
- **Line editing** — prose clarity, rhythm, voice, show vs. tell, word-level fixes
- **Consistency checking** — names, timelines, settings, POV, tone
- **Priority revision list** — ranked top-5 fixes ordered by reader impact

Every note quotes the relevant passage and offers a concrete suggestion. No vague feedback.

## Install

Copy the `SKILL.md` file into your Claude Code skills directory:

```bash
# Personal (available in all projects)
mkdir -p ~/.claude/skills/top-book-editor
cp SKILL.md ~/.claude/skills/top-book-editor/SKILL.md
```

Or for a specific project:

```bash
mkdir -p .claude/skills/top-book-editor
cp SKILL.md .claude/skills/top-book-editor/SKILL.md
```

## Usage

```
/top-book-editor manuscript.md
```

Edit a specific chapter:

```
/top-book-editor chapter-03.md
```

Edit a full book directory:

```
/top-book-editor ./chapters/
```

Focus on a specific area:

```
/top-book-editor manuscript.md dialogue
/top-book-editor manuscript.md pacing
/top-book-editor manuscript.md character
```

## What You Get Back

A structured editorial report:

1. **Overall Assessment** — What's working, what's the biggest issue, how close is it
2. **Strengths** — What NOT to change
3. **Developmental Notes** — Big-picture issues by chapter with specific fixes
4. **Line Edit Highlights** — 15-25 impactful prose improvements with before/after
5. **Consistency Issues** — Continuity errors checklist
6. **Priority Revision List** — Top 5 things to fix first

## Focus Areas

Pass a second argument to go deep on one area:

| Focus | What It Covers |
|---|---|
| `structure` | Arc, chapter flow, narrative engine |
| `pacing` | Slow sections, rushed beats, rhythm |
| `character` | Arcs, motivation, distinctiveness |
| `dialogue` | Authenticity, voice, exposition in speech |
| `prose` | Sentence-level clarity, rhythm, word choice |
| `consistency` | Names, timelines, settings, POV |
| `show-vs-tell` | Emotional/motivational telling patterns |

## Philosophy

- Edits within the author's voice, never toward the editor's
- Honest but respectful — assumes the author cares deeply
- Praises specifically, criticizes specifically
- Won't invent problems to seem thorough
- Explains what the manuscript *gains* from every suggested cut

## License

MIT

## Author

[Trace Cohen](https://x.com/Trace_Cohen)
