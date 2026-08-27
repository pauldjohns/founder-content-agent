---
name: style-observations
description: Running log of editorial corrections the founder has made, treated as hard constraints. Read BEFORE drafting or reviewing. Where an observation conflicts with the voice profile, the observation wins - it is the more specific, demonstrated preference.
---

# Style Observations

The voice profile says how the founder writes. This file records what they actually corrected, in
order, with the reason. It is the part of the system that improves.

## How this file works

- **Every entry is a hard constraint**, not a suggestion.
- **Observations beat the voice profile.** A profile is written once from intent; an observation
  comes from a real edit on a real draft. When they conflict, the specific demonstrated preference
  wins, and that is a signal the profile needs revisiting.
- **Log the reason, not just the rule.** "Cut the closing summary" is a rule you will misapply. "Cut
  the closing summary - it restated the paragraph above it and told the reader nothing new" is a rule
  you can generalise from.
- **Append, never rewrite.** Dated entries in order. When an observation is superseded, add the new
  one and mark the old one superseded rather than deleting it - the pair is more informative than
  either alone.
- **One observation per correction.** If an edit fixed three things, that is three entries.

## Entry format

```
### YYYY-MM-DD — [channel: LinkedIn / newsletter / email / landing page]

**Draft said:** the exact text that was wrong, quoted.
**Founder changed it to:** the exact replacement, quoted.
**Why:** the founder's own reason, in their words if you have them.
**Generalised rule:** the constraint to apply next time, stated so it is checkable.
**Failure mode tag:** one of the tags below.
```

## Worked example

### 2026-01-14 — LinkedIn

**Draft said:** "In today's fast-moving landscape, teams are increasingly finding that their
existing workflows no longer serve them."
**Founder changed it to:** "Three teams told me the same thing last month: they stopped using the
thing they built in the first week."
**Why:** the original describes a trend nobody can check. The replacement is something that
happened, and the reader can picture it.
**Generalised rule:** open with a specific incident and a number, never with a state-of-the-industry
claim. If the first sentence could open any post in the category, it is not the first sentence.
**Failure mode tag:** `#generic-opener`

## Failure mode tags

Start with these and add your own as patterns repeat. The tags are how you spot that the same
mistake is being made in a new costume.

| Tag | Means |
|---|---|
| `#generic-opener` | first line could belong to any post on the topic |
| `#unearned-claim` | asserts something with no source and no incident behind it |
| `#recap` | closing paragraph restates what the reader just read |
| `#hedge` | ends on a question or a maybe where a position belonged |
| `#borrowed-voice` | register drifted toward LinkedIn-default or press-release |
| `#jargon` | reached for a category word where a plain one was available |
| `#invented-detail` | added a specific that was not in the source material |
| `#length` | said in nine sentences what three would carry |

## Adding to this file

The founder will say things like "that's a pattern", "log that", or "add to style notes". Those are
the trigger. Write the entry while the edit is still in front of you - reconstructing the reason
later produces a rule that sounds right and does not match what actually bothered them.
