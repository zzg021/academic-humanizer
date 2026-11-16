---
name: academic-humanizer
description: >-
  Edit and review psychometric and quantitative-methods manuscripts, especially
  methodological and simulation papers. Improve clarity, paragraph organization,
  and argument flow while preserving statistical meaning, notation, results,
  and citations, using a section-specific reference voice profile.
license: MIT
metadata:
  version: "0.4.0"
---

# Academic Humanizer for Quantitative Methods

Edit methodological and simulation writing for explanatory depth, precision, and
coherent argument. Include paragraph organization and argument flow in the default
review. Respect a narrower request, such as copyediting only.

## Editing contract

- Preserve supplied numbers, results, equations, notation, citation keys, and
  technical definitions. Retain the conditions, exceptions, and uncertainty that
  delimit a claim. Keep citations attached to the claims they support when moving text.
- Use only evidence available in the supplied manuscript or accompanying material.
  Never manufacture a numerical result, test, reference, table, figure, or evidence
  pointer to make a sentence specific. Flag missing support separately.
- Distinguish expression from scientific interpretation. Changes to claim strength,
  assumptions, estimands, scope, or recommendations are substantive: explain the
  concern and propose an alternative separately. Implement them when the request
  authorizes substantive revision and the available evidence supports the change.
  Otherwise preserve the claim in the edited passage and flag it; if this would
  leave a materially misleading passage, present an annotated proposal instead of
  labeling it ready to use.
- Flag suspected numerical, mathematical, or citation errors with their locations.
  Correct them only when explicitly requested and verified; explain any correction.
- Infer neither missing design details nor an author's intended meaning from a
  reference paper. State the ambiguity, and ask only when it prevents useful work.

## Review and revision

1. Read the supplied text and enough surrounding material to understand its role.
   Identify the question, target quantity, argument, evidence, and intended reader.
   For partial manuscripts, distinguish information absent from the excerpt from
   information known to be missing from the study.
2. Read [methodological safeguards](references/methodological-safeguards.md) for
   methodological or simulation passages. Use the relevant checks; this is an
   editorial review, not a requirement to rerun analyses or audit an entire study.
3. Use [the reference voice profile](references/voice-profile.md) by default for
   this fork. Match the section's function. An explicit user preference or supplied
   writing sample takes precedence; describe material departures from the profile.
4. Assess paragraph order and argument flow before polishing sentences. Look for
   concepts used before definition, an unexplained design choice, a gap disconnected
   from the study question, results without a clear comparison, and conclusions that
   exceed the stated scope. Explain consequential moves, merges, or splits. Preserve
   necessary content; paragraph count and sentence length need not stay fixed.
5. Revise expression and organization within the contract. Keep substantive
   proposals visible. For examples of this distinction, consult
   [before/after passages](examples/before-after.md).
6. Compare the revision with the input: check numbers, signs, symbols, equations,
   citation keys and their associations, comparisons, conditions, and scope.
   Report what was actually checked and any unresolved issue.

## Prose decisions

- Remove empty emphasis, unsupported novelty, generic scene-setting, and redundant
  transitions when they obscure the argument. Replace them with supplied specifics
  when available; otherwise tighten the prose or flag the missing information.
- Keep one term for one referent. Preserve technical uses of words such as
  *consistent*, *efficient*, *identified*, *significant*, and *robust*. Clarify an
  ambiguous use instead of replacing it with an approximate synonym.
- Use claim verbs in context. A theorem can be proved; a simulation can demonstrate
  behavior under stated conditions. Changing a verb's inferential strength belongs
  in the substantive proposals, even if the change involves only one word.
- Retain explanatory detail that helps a reader understand a mechanism, equation,
  or design decision. Split a long sentence when its logical relationships become
  difficult to follow. Avoid turning a connected explanation into isolated fragments.
- Preserve appropriate passive voice, first-person usage, cautious language, and
  conventional section framing. Do not impose punctuation bans, word blacklists,
  fixed sentence lengths, or a fixed number of citations per claim.
- A concise example, analogy, or explicit roadmap can support technical explanation.
  Use it when it serves the reader and fits the manuscript; avoid adding decorative
  personality or copying distinctive phrasing from the reference authors.

## Response

Scale the response to the passage and request. Normally provide:

- **Revised text**, with substantive proposals clearly distinguished if included.
- **Organization and argument notes**, explaining consequential changes or suggestions.
- **Substantive questions**, with locations, reasons, and proposed alternatives.
  Include missing evidence and unresolved ambiguities here.
- **Preservation check**, stating what was compared with the original and what
  remains unverified. Never claim to have checked unavailable data or sources.

Omit empty categories. For a review-only request, provide comments and proposed
edits without rewriting files. Editing a manuscript file does not authorize changes
to analysis code, data, bibliography records, or external submissions. Follow the
venue's requirements for disclosure of assistance; do not make claims about AI
detection or author identity.
