---
name: linkedin-post-reviewer
description: Review and score LinkedIn posts against a founder-led writing framework and customer vocabulary engine for PM/designer audience resonance. Use when the user submits a draft LinkedIn post for review, asks to check a post against their writing framework, wants vocabulary resonance scoring, or asks to review content before publishing on LinkedIn. Also use when the user references 'post review,' 'check this post,' 'review my draft,' or 'does this sound right for PMs.'
---

# LinkedIn Post Reviewer

Review LinkedIn posts for voice compliance, post-type discipline, and PM/designer vocabulary resonance.

## Setup

Before reviewing any post, read the following reference files:
- `reference/customer-vocabulary.md` — PM-native phrases, pain points, desired outcomes
- `.claude/skills/customer-vocabulary/SKILL.md` — Verified customer language, blocked phrases, voice preservation rules
- `reference/audience-profile.md` — Content Triggers, Pain Points, What They Ignore, and Language & Tone sections
- `.claude/skills/style-observations/SKILL.md` — Apply every active observation as a hard constraint during review. Where an observation conflicts with a general voice guideline, the observation wins.

## Review Workflow

For every submitted draft, execute these steps in order.

### Step 1: Classify Post Type

Determine which post type the draft is attempting:
- **Recognition** — One truth, no explanation, no product mention
- **Diagnosis** — Names a breakdown, no authority claim, no solution
- **Builder Context** — Present-tense focus, the product appears as motivation only

State the classification. Then check for mixed jobs: if the post is trying to do more than one of these jobs simultaneously, flag exactly where the second job begins.

### Step 2: Voice Compliance Check

Score pass/fail on each rule:

| Check | Pass/Fail |
|---|---|
| No PM role borrowing | |
| Present-tense, observational | |
| Artifact-level (concrete, not abstract) | |
| No narrator language ('I keep seeing,' 'Patterns I've noticed') | |
| No abstraction-first framing | |
| No stacked metaphors | |
| No CTA verbs or marketing tone | |
| No retrospective authority claims | |
| Builder-focused, not explainer-focused | |
| product-mention constraint respected for post type | |

For each failure, quote the offending phrase and state why it fails.

### Step 3: Vocabulary Resonance Score

Score the draft 0–10 based on how well it uses PM-native language from the customer vocabulary and marketing guide.

Provide:
- The numeric score
- Which PM-native phrases or themes the draft successfully mirrors (if any)
- Which abstract or generic phrases could be swapped for PM-native alternatives (use the substitution table)

### Step 3.5: Audience Profile Impact Check

Using the audience profile loaded in Setup, evaluate the post on three dimensions:

**Content Trigger match:** Does the post touch one of the triggers listed in the audience profile's *Content triggers* section? Name the trigger it hits, or flag that it misses all of them. Read the triggers from the profile - do not carry them in this file, or the reviewer will score every draft against whoever wrote it first.

**Pain point alignment:** Does the post name or address a pain listed in the profile's *Pain points and motivations* section, or something outside them? Quote the pain it lands on.

**'What they ignore' check:** Does the post read like any of the things this audience scrolls past — generic tips lists, vendor-toned content, abstract AI trend pieces without grounding? If yes, flag exactly where the post crosses into ignore territory.

Score the post: **High / Medium / Low audience impact** with one sentence of justification.

### Step 4: Scorecard Summary

Present a compact scorecard:

```
Post Type: [Classification]
Mixed Jobs: [None / Flagged — describe]
Voice Compliance: [X/10 checks passed]
Vocabulary Resonance: [X/10]
Audience Profile Impact: [High / Medium / Low — one line reason]
Overall: [Ready to post / Needs revision]
```

If any voice check fails OR resonance is below 5 OR mixed jobs are detected OR audience impact is Low → mark 'Needs revision.'

### Step 5: Revised Draft (If Needed)

If the post needs revision, provide a rewritten version that:
- Fixes all flagged voice violations
- Resolves any mixed-job issues (split into separate posts if necessary)
- Substitutes abstract language with PM-native alternatives where natural
- Sharpens the content trigger alignment if audience impact was Medium or Low
- Preserves the original insight and intent

After the revised draft, briefly state what changed and why — one line per change, no more.

## Edge Cases

- If the draft is a thread or multi-post sequence, review each post individually, then evaluate whether the sequence follows the story arc (Truth → Mechanism → Focus).
- If the user specifies the intended post type, use that classification instead of inferring. Still flag if the content doesn't match the declared type.
- If a post is strong and passes all checks, say so directly. No padding, no unnecessary suggestions.
