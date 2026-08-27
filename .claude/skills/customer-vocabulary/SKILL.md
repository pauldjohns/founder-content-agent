---
name: customer-vocabulary
description: Build and enforce a verified vocabulary from your own customer interviews, so marketing copy uses language customers actually used. Blocks fabricated phrases. This is the METHOD - the phrase lists are yours to fill in from your own transcripts.
---

# Customer Vocabulary

## Purpose

Marketing copy drifts toward the words the company uses internally, which are almost never the words
customers use. This skill closes that gap by making one rule enforceable: **a phrase may appear in
external copy only if a customer said it in a recorded conversation.**

Everything below is the method and the schema. The vocabulary itself is built from your transcripts
and lives in `reference/customer-vocabulary.md`, which is gitignored, because verbatim customer
quotes are confidential research and often personal data.

## Core principle

Verified means traceable. Every entry carries the interview it came from, so any claim in a landing
page can be walked back to a person who said it. A phrase that "sounds like what customers mean" is
a fabrication with good intentions, and it is the specific failure this skill exists to prevent.

## Building the vocabulary

1. **Transcribe every discovery call.** Speaker-labelled. The labels are load-bearing - see the
   contamination check below.
2. **Pull only customer turns.** Filter out the interviewer entirely before you start reading for
   language.
3. **Bucket the quotes** into four categories. These four are what messaging actually needs:

   | Bucket | What goes in it |
   |---|---|
   | **Pain language** | how they describe the problem, unprompted |
   | **Outcome language** | what they say they want to be true afterwards |
   | **Current process** | what they do today, including the workarounds and the tools they name |
   | **Trigger moments** | what made this urgent now rather than last quarter |

4. **Record each entry verbatim** - the sentence as spoken, disfluencies included. Cleaning a quote
   into marketing English destroys the thing you extracted it for.
5. **Count.** A word-frequency table over substantive quotes tells you which term is native and which
   one you have been imposing. Frequency beats taste here.
6. **Version it.** Note the interview count and quote count at the top, and what changed since last
   revision. When the vocabulary grows, messaging gets re-checked against the new version.

### Entry format

```
✓ "exact sentence as the customer said it"     [interview 23, 2026-02-14, PM at a 200-person SaaS]
```

Role and company shape are enough context. Names and employers do not belong in a file that gets read
during drafting.

## The contamination check

The most common way a "verified" vocabulary goes wrong: the interviewer says a phrase, the customer
says "yeah, exactly", and the phrase gets logged as customer language. It is now house vocabulary
wearing a customer's voice, and it will feel validated every time you use it.

So: **search every candidate phrase across the interviewer's own turns first.** If it appears there
before it appears in a customer turn, it is contaminated. Move it to the blocked list with a note of
where it came from. Do this even when the customer repeated it back enthusiastically - especially
then.

## Blocked phrases

Two kinds, kept in the same list with the reason attached:

- **Fabricated** - phrases that appeared in earlier copy and appear in no transcript at all. Usually
  category-standard language that a model or a marketer supplied because it sounded right.
- **Contaminated** - phrases that only ever came out of the interviewer's mouth.

A blocked list with reasons is more useful than a style guide, because it names the exact temptations
this product's copy keeps falling for. Expect it to be long, and expect the entries to be plausible -
that is why they got in.

## Voice preservation

**Always preserve:** hedges, hesitation and qualifiers ("kind of", "I guess", "for us, maybe"); the
customer's own metaphors; the specific numbers they used; their tool names; the messy sentence
structure of speech.

**Never:** smooth a quote into a slogan, merge two speakers into one composite, tighten a
disfluent sentence, or promote a paraphrase to a quotation. If a quote is too long for a headline,
the headline is not ready - do not trim the customer to fit it.

## Using it

| Context | How the vocabulary applies |
|---|---|
| Website copy | headline and subhead must be traceable to a real quote or a direct compression of one |
| Social posts | pain language in the opening, outcome language in the close, blocked list checked before publishing |
| Outreach | the trigger-moment bucket is the highest-value one - it tells you why now |
| Product naming | check the current-process bucket for what they already call the thing |

## Reviewing a draft

For each customer-facing claim, ask: which quote is this from? If the answer is "it's the general
sense of several", rewrite it until it points at one. If a phrase is on the blocked list, it comes
out even when it reads better - readability is not the standard here, traceability is.
