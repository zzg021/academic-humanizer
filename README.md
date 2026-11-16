# Academic Humanizer for Quantitative Methods

A personal adaptation of
[AIScientists-Dev/academic-humanizer](https://github.com/AIScientists-Dev/academic-humanizer)
for psychometrics and quantitative methods, especially methodological and
simulation papers. The skill name remains `academic-humanizer`.

The default review covers clarity, paragraph organization, and argument flow.
It preserves statistical meaning and supplied evidence, with a provisional
reference voice informed by selected Konold–Sanders papers. Version: **0.4.0**.

## What the editor does

- Tightens repetition and empty emphasis while retaining useful explanation.
- Connects the methodological question, design, comparisons, and conclusions.
- Suggests paragraph moves, merges, and splits with reasons.
- Preserves notation, equations, numbers, citations, uncertainty, and scope.
- Flags unsupported claims, ambiguous quantities, and missing reporting details.
- Separates stylistic changes from proposals that change scientific interpretation.

The editor uses supplied evidence. If a comparison lacks a result or an evidence
pointer, it identifies the gap. It does not create numbers, references, diagnostics,
or findings to complete the prose. It reports what it checked and what remains
unverified. It does not require rerunning analyses for an ordinary editing pass.

## Use

Provide the manuscript or a section and describe its purpose. For example:

```text
Use academic-humanizer to revise this simulation-results section.
Review paragraph organization and argument flow, preserve all reported results,
and list substantive concerns separately. Use the reference voice profile.
```

For a narrower pass:

```text
Copyedit only. Keep paragraph order and claim strength unchanged.
Flag substantive concerns in comments.
```

For comments without a rewrite:

```text
Review this introduction's argument. Explain which paragraphs should move,
which transitions need work, and whether the study question follows from the
prior literature. Do not edit the manuscript file.
```

When editing files, point the agent at `SKILL.md` and the relevant manuscript.
The instructions can also be supplied directly to an agent that accepts Markdown
instructions. The skill contains no executable helpers or external dependencies.

## Install from this fork

For Codex, place the repository contents in a discoverable skill directory:

```bash
git clone https://github.com/zzg021/academic-humanizer ~/.codex/skills/academic-humanizer
```

For Claude Code:

```bash
git clone https://github.com/zzg021/academic-humanizer ~/.claude/skills/academic-humanizer
```

Keep the supporting directories alongside `SKILL.md`. For an existing installation,
review local changes before updating it. Editing this repository does not update
an installed copy automatically.

## How the reference voice is used

The [voice profile](references/voice-profile.md) identifies three initial anchors
and four additional comparison papers, with DOI links and Zotero item keys. It
describes section-specific editorial choices: explaining mechanisms, motivating
design decisions, reporting conditional comparisons, and connecting findings to
analysts' decisions.

The profile is qualitative and provisional. It represents selected coauthored
writing, not the user's established personal style or an individual author's
contribution. Explicit preferences and the user's own samples take precedence.
Future passage-level feedback can refine it. Ordinary editing works from the
profile without Zotero or network access.

The repository contains original editorial notes and constructed examples.
It does not redistribute the reference papers or extracted full text, and it
does not transfer those papers' methods or recommendations into a new manuscript.

## Contents

- [SKILL.md](SKILL.md): editing contract, workflow, and response guidance.
- [Methodological safeguards](references/methodological-safeguards.md): relevant
  distinctions for simulation, psychometric, and Bayesian or frequentist writing.
- [Voice profile](references/voice-profile.md): sources, section-specific choices,
  and guidance for further calibration.
- [Before/after examples](examples/before-after.md): constructed demonstrations
  that preserve supplied evidence and make substantive proposals visible.

Funding-proposal guidance and its examples have been removed from this adaptation.
Sentence length, punctuation, paragraph count, citation count, and selection of
ranges versus averages are judged in context.

## Attribution and disclosure

Adapted from **AIScientists-Dev/academic-humanizer**, which credits
[blader/humanizer](https://github.com/blader/humanizer) for its general writing-pattern
catalog and [koaeraser/ARMS](https://github.com/koaeraser/ARMS) for informing its
claim–evidence and numerical-precision emphasis. The original copyright and
[MIT license](LICENSE) are retained. Reference papers have their own rights;
the repository license does not license those papers.

Use this as an editing aid and follow the submission venue's disclosure policy.
It makes no promise about AI detection or authorship attribution.
