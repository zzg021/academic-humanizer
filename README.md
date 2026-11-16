# Academic Humanizer for Quantitative Methods

A personal adaptation of
[AIScientists-Dev/academic-humanizer](https://github.com/AIScientists-Dev/academic-humanizer)
for methodological and simulation papers in psychometrics and quantitative
methods. The skill name remains `academic-humanizer`.
Version: **0.4.0**.

The aim is to make the paper's intellectual contribution clear: what the problem
is, where it comes from, how the paper addresses it, and what that changes.
Framing, paragraph organization, and argument flow are part of the default edit.

## Editorial priorities

- Bring the research problem and contribution forward.
- Explain the mechanism behind the problem and the idea behind the response.
- Connect theory, simulation, and interpretation into a coherent argument.
- Select and place technical detail according to its role in that explanation.
- Tighten repetitive, defensive prose and state supported findings directly.

A methodological paper can contain substantial mathematics and a reproducible
simulation design while keeping the research question in view. Routine settings
and secondary checks belong where readers need them. Qualifications should
explain a meaningful boundary; repeating them should not obscure the finding.

The editor preserves the study's meaning and supplied evidence as a background
responsibility. Its usual output is revised prose and a brief explanation of
important editorial decisions.

## Use

```text
Use academic-humanizer to revise this introduction.
Bring the research problem and the idea behind our response into focus.
Suggest changes to paragraph order and cut details that interrupt the argument,
indicating where they should go.
```

```text
Revise these simulation results around the findings that answer our research
question. Help readers understand the pattern and its explanation, and move
routine condition-by-condition reporting into a table or supporting passage.
```

You can also request comments only or a narrower copyedit. Point the agent at
`SKILL.md` and the manuscript, or supply the Markdown instructions directly.

## Reference voice

The [voice profile](references/voice-profile.md) draws on selected Konold–Sanders
papers in the user's Zotero library. Its emphasis is their narrative reasoning:
make a methodological difficulty intelligible, explain its source, develop the
response, and connect the evidence to what researchers should understand.

It identifies three initial anchors and four additional papers, with DOI links
and Zotero item keys. The profile is provisional and can be refined through edits
of the user's writing. It works without Zotero or network access; article full
text is not included in the repository.

## Install from this fork

For Codex:

```bash
git clone https://github.com/zzg021/academic-humanizer ~/.codex/skills/academic-humanizer
```

For Claude Code:

```bash
git clone https://github.com/zzg021/academic-humanizer ~/.claude/skills/academic-humanizer
```

Keep the supporting directories alongside `SKILL.md`. Review local changes before
updating an existing installation. This skill contains no executable helpers or
external dependencies.

## Contents

- [SKILL.md](SKILL.md): editorial priorities and workflow.
- [Voice profile](references/voice-profile.md): narrative choices and reference papers.
- [Editing examples](examples/before-after.md): constructed illustrations of framing,
  interpretation, and detail placement.

## Attribution

Adapted from **AIScientists-Dev/academic-humanizer**, which credits
[blader/humanizer](https://github.com/blader/humanizer) for its writing-pattern
catalog and [koaeraser/ARMS](https://github.com/koaeraser/ARMS) for informing its
claim–evidence and numerical-precision emphasis. The original copyright and
[MIT license](LICENSE) are retained. Reference papers have their own rights.

Follow the submission venue's policy on disclosure of assistance.
