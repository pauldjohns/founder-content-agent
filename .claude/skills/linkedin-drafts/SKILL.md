---
name: linkedin-drafts
description: "Draft LinkedIn posts in the founder's voice from the weekly research signal file. Use when producing weekly LinkedIn post drafts."
---

# LinkedIn Post Drafts

## Process
1. Read the most recent signal file from output/research/.
2. Read reference/customer-vocabulary.md.
3. Read 2–3 examples from reference/post-examples/ to calibrate voice.
4. Load the founder-voice skill. Load style-observations skill.
5. Select 3–5 of the strongest angles from the signal file.
6. For each angle, draft a complete LinkedIn post:
   - Written in the founder's voice per the founder-voice skill
   - Apply vocabulary from the marketing guide
   - Apply style-observations as hard constraints
   - Run the Voice Test (6 questions) – revise until it passes
7. Run the linkedin-post-reviewer skill against each completed draft.
   Include the full scorecard below each post.
8. Run the validation step from CLAUDE.md: verify every source, quote,
   statistic, and attributed claim.
9. Label each draft with its angle/topic and category.

## Output
Save all drafts to output/linkedin/YYYY-MM-DD-posts.md.
Email the file to you@your-company.example via Gmail connector with
subject: '[LinkedIn Drafts] YYYY-MM-DD'.

Each post should be complete and ready for the founder to copy-paste-publish
after his review.

## Acceptance Criteria
- 3–5 complete LinkedIn posts
- Each passes the Voice Test
- Each reviewed by linkedin-post-reviewer with scorecard included
- All sources verified per validation step
- No AI-slop words or forbidden patterns
- File saved to output/linkedin/
- Email sent to you@your-company.example
