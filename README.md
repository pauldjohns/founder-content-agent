# founder-content-agent

A Claude Code workspace that drafts founder-led content – LinkedIn posts, a newsletter, research
round-ups – in one specific person’s voice, and refuses to publish any of it. Ten skills, three
reference files, one orchestration file. No app, no API, no scheduler: you open the folder in Claude
Code and ask for a draft.

It ships as a scaffold. The framework is real and complete; the voice, the audience and the customer
vocabulary are yours to fill in, and the system is close to useless until you do.

## Why it is built this way

Most “AI writes your LinkedIn” setups fail the same way: the model writes competent category-average
prose that no reader can attribute to a person. Three things here fight that.

**A voice profile with convictions in it.** `founder-voice` is not a tone slider. It holds the
founder’s positions, their emotional register, what they explicitly do *not* sound like, and a
six-question test a draft has to pass. Positions are what let a draft close instead of hedge.

**An observation log that outranks the profile.** `style-observations` records every correction the
founder actually made, with the reason and a generalised rule. Where the log and the profile
disagree, the log wins – it came from a real edit rather than an intention. This is the part that
compounds; a system without it makes the same mistake in a new costume every month.

**A vocabulary gate.** `customer-vocabulary` allows a phrase into external copy only if a customer
said it in a recorded interview, and keeps a blocked list of phrases that were fabricated or that
came out of the interviewer’s own mouth. That second category is the sneaky one: you say it, they
say “yeah, exactly”, and it gets logged as customer language forever.

Then a verification pass, required after every draft: every statistic, quote and attributed claim
gets checked against its source, and anything that cannot be confirmed is removed rather than
flagged and shipped.

## The skills

| Skill | Does |
|---|---|
| `founder-voice` | identity, convictions, register, the Voice Test. **Template – fill it in first.** |
| `style-observations` | the running correction log, treated as hard constraints. **Template.** |
| `customer-vocabulary` | method for building a verified phrase set from your transcripts. **Template.** |
| `linkedin-drafts` | generate post drafts from a research pass or a raw idea |
| `linkedin-post-reviewer` | score a draft against voice, post-type discipline and vocabulary |
| `newsletter-draft` | draft an issue in the format defined in `reference/newsletter-format.md` |
| `weekly-research` | the recurring research pass that feeds everything else |
| `talking-point-extractor` | turn transcripts, articles or PDFs into categorised talking points |
| `discovery-messaging-advisor` | pressure-test messaging and write interview questions |
| `customer-persona-intelligence-builder` | build the buyer persona the reviewer scores against |

`reference/newsletter-format.md` is worth reading even if you never send a newsletter: it defines a
field note → pattern → field note arc, sourcing rules, and the failure modes that turn an issue into
a link dump.

## Set it up

1. **Fill in `.claude/skills/founder-voice/SKILL.md`.** Every section is a prompt. Use the founder’s
   own sentences – transcripts of them talking beat anything written for the purpose.
2. **Write `reference/audience-profile.md`** from `audience-profile.template.md`.
3. **Add `reference/post-examples/`** – five to ten of their actual published posts, as calibration,
   never as templates. `examples/post-example.md` shows the file shape.
4. **Build `reference/customer-vocabulary.md`** from your own interview transcripts, following the
   method in the `customer-vocabulary` skill. Skip this and the reviewer has nothing to check
   language against.
5. **Configure `CLAUDE.md`** – the two `CONFIGURE:` blocks are your audience filter and where
   finished drafts go.

Then open the folder in Claude Code: *“run this week’s research and draft three LinkedIn posts.”*

## What is deliberately missing

The repo this came from was one founder’s working setup. Removed before publishing, and gitignored so
they cannot come back: the filled-in voice profile, the real observation log, the audience profile,
the published-post calibration set, every draft in `output/`, and the customer vocabulary – which
contained verbatim interview quotes and the names of the customers who gave them.

The last one is worth stating plainly. A verified-vocabulary file is confidential research and, in
most jurisdictions, personal data. Keep it local, keep the names out of it, and never publish the
repo it lives in.

## Layout

```
CLAUDE.md                the orchestration - role, skills, hard rules, verification, output format
.claude/skills/          the ten skills, three of them templates you fill in
reference/               newsletter format, audience-profile template
examples/                one invented calibration post
output/                  drafts land here (gitignored)
```
