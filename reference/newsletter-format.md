# Newsletter Format Reference

*Last updated: 2026-03-23*
*Status: Active, early-stage. Expect this document to evolve as issues are published and patterns confirm or change.*

---

## What This Document Is

The structural and editorial rules for 'the newsletter,' the founder's bi-weekly newsletter for PMs and designers at web-first B2B SaaS companies navigating the AI transition.

This document governs how the newsletter is built – section types, structural arcs, data framing, sourcing rules. Voice, tone, and language rules live in the founder-voice skill and style-observations skill. Those take precedence on anything related to how it sounds. This document takes precedence on anything related to how it's structured.

---

## Format Overview

**Cadence:** Bi-weekly
**Audience:** PMs and product designers at web-first B2B SaaS companies (same ICP as LinkedIn content)
**Length:** 2,000–4,000 words total across all sections
**Posture:** Peer, not guru. Field notes from someone doing the work, not commentary from above it.

### Section Types

**Feature sections (2–3 per issue).** Long-form analytical pieces, 600–1,200 words each. These carry the issue. Each one makes a single argument grounded in data and real observations from the founder's discovery calls, design partner relationships, or direct experience.

**Three More Things (1 per issue, always last before sign-off).** Three short observations, 80–150 words each. Direct, compressed, no arc required. These are the place for sharp observations that don't need a full section to land.

**Sign-off.** the founder's name, the company reference, cadence reminder, invitation to reply.

### Standard Issue Structure

1. Feature section 1
2. Feature section 2
3. Feature section 3 (optional – two strong sections are better than three weak ones)
4. Three More Things
5. Sign-off
6. Source Verification Log (not for publication – the founder's review only)
7. Field Note Source Log (not for publication – the founder's review only)

---

## Feature Section Structure: Field Note → Pattern → Field Note

Each feature section follows a three-part arc. This is the default structural skeleton, not a rigid template. If a section works better without the arc – because the data leads naturally or because there's no real field note available – skip it rather than forcing it. The arc exists to serve the reader, not the format.

### Part 1: Open with a field note

A specific person, a specific moment, a specific observation. One scene. 2–4 sentences. The reader should see themselves in it before any data or argument arrives.

**Sources for field notes (in order of preference):**
1. A direct quote or paraphrased observation from a real discovery call, design partner conversation, or meeting (source from your own call transcripts or meeting notes)
2. An anonymised observation from the founder's direct experience – something he saw, heard, or noticed in a real interaction
3. An editorial inference built from real material – a constructed scene that accurately represents a documented pattern, clearly sourced in the Field Note Source Log

**What the opening is not:**
- A statistic (stats arrive second, as context for what the reader already felt)
- A category statement ('The PM landscape is shifting')
- A transition from the previous section ('Building on that idea…')
- A fabricated story or composite character presented as a single person

### Part 2: Zoom out to the pattern

Introduce the industry-level data, the trend, the argument. This is where statistics, research, and analysis live. The field note earned the reader's attention. The pattern earns their trust.

**Data framing rule:** Never present a data point without framing it in terms the reader already understands. Translate numbers into the reader's daily reality – a workflow moment, a team dynamic, a feeling they recognise.

Examples of the translation:
- '76-point gap between speed and confidence' → 'the distance between "I shipped it" and "I'd bet my job on it"'
- '40% of designers don't trust AI outputs fully' → 'four out of ten people on your design team checking the work by hand'

The frame is not a dollar-to-object equivalent (that's macro-scale technique for macro-scale numbers). PM-scale data is already at human scale. The frame names what the number feels like in the reader's working life.

### Part 3: Return to the specific

Close by returning to the person or observation from the opening. One sentence, sometimes two. The reader arrives at the conclusion themselves. Do not explain what the section meant. Do not state the takeaway. Let the return to the specific do the closing work.

**What the close is not:**
- A thesis statement ('That's the job for a lot of PMs right now')
- A call to action
- A hedge ('Time will tell')
- A new idea introduced at the last moment

---

## Three More Things – Structure

Three short, independent observations. Each one:
- Opens with a bolded topic sentence
- Makes one point in 80–150 words
- Stands alone – no arc, no callback, no structural obligation
- Can reference data, trends, or observations – but the compression is the point

These are the place for ideas that are sharp enough to include but don't need 800 words to land.

---

## Sourcing Rules

### Data and statistics
- Every data point must be traceable to a verifiable public source
- Source verification pass is mandatory after every draft (see CLAUDE.md Validation Step)
- If a source cannot be verified, flag it with [UNVERIFIED] in the Source Verification Log
- Remove or replace any claim that fails verification – do not publish flagged claims
- When pairing statistics from different studies, name both sources explicitly in the text

### Field notes from discovery calls
- Anonymise all individuals by default (role and company type, not name)
- Paraphrase rather than direct-quote unless the exact words are the point
- Source every field note in the Field Note Source Log with: participant name, company, date, and the original words
- Editorial inferences (constructed scenes from real patterns) are permitted when specific moments are unavailable – but must be flagged as inferences in the source log
- Never combine statements from different transcript sections into a single attributed observation
- Never fabricate a field note. If no real moment exists for the structural opening, skip the arc for that section

### The inference rule
First preference is always what really happened or was said. Inference is acceptable for storytelling when specific material is unavailable, provided the inference accurately represents a documented pattern and is flagged in the source log. Fabrication is never acceptable.

---

## What This Newsletter Is Not

- A product newsletter for your audience. The product may appear as motivation (why the founder is in the room) but never as pitch.
- A trend report. Every section is grounded in specific people and specific observations. Category-level analysis without grounding fails the format.
- An advice column. The posture is 'here's what I'm seeing' not 'here's what you should do.'
- A contrarian hot-take vehicle. the founder has a point of view and states it. He does not perform provocation.

---

## Failure Modes to Watch

| Mode | Description |
|------|-------------|
| Stat-first opening | Section opens with a number instead of a person. The data should arrive second, as context for something the reader already felt. |
| Forced arc | The field note → pattern → field note structure is applied to a section where it doesn't fit. Skip the arc rather than force it. |
| Explained close | The section tells the reader what to think at the end instead of returning to the specific. Assume the intelligence of the audience. |
| Guru drift | The writing starts explaining from above rather than observing from alongside. Check: would the founder say this to a PM sitting next to him, or would he say it from a stage? |
| Fabricated field note | A constructed scene presented as a real moment without flagging it as an inference in the source log. |
| Orphaned data | A statistic cited without framing it in terms the reader's daily reality. The number alone is inert. |
| Over-production | Adding visual elements, complex formatting, or structural complexity before the content and audience warrant it. The writing does the work at this stage. |

---

## Visual Elements (Future – Not Yet Active)

Data visualisation is worth testing in a future issue when the data genuinely benefits from visual treatment. The rules for when that happens:

- One visual per issue maximum
- Only when the visual makes the point clearer than prose alone
- Clean, minimal, typographic style – not hand-drawn, not decorative
- If the visual exists to look like a newsletter rather than to clarify an argument, cut it

This section will be updated if and when a visual language for 'the newsletter' is developed.

---

## Output Requirements

- File location: `output/newsletter/`
- File naming: `YYYY-MM-DD-newsletter.md`
- Header format:

```
# <Your Newsletter Name>
**Issue – DD Month YYYY**

*For PMs and Designers navigating the AI transition at web-first B2B SaaS companies.*
```

- Source Verification Log and Field Note Source Log appended at the bottom, clearly marked as not for publication
- After saving, email the file to you@your-company.example via Gmail with subject: '[Newsletter Draft] YYYY-MM-DD'
