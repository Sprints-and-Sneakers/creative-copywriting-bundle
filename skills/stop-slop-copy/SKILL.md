---
name: stop-slop-copy
description: Checks marketing copy for spelling and grammar mistakes, then checks whether it sounds like a real person wrote it or like an AI wrote it, and suggests a fix for each problem found. Use when reviewing ad copy for statics/video/UGC ads, LinkedIn messages, emails, organic captions, or any written marketing text before it goes out.
metadata:
  author: Sprints & Sneakers (https://sprintsandsneakers.com)
---

# Stop-Slop Copy Checker

Two jobs, one skill: is the copy written correctly, and does it sound human. Read both reference files in full before reviewing anything — do not review from memory.

## What this skill uses

- `references/grammar-style-guide.md` — calibrated Dutch and English grammar/spelling rules, plus general-knowledge coverage (capped confidence) for any other language
- `references/anti-slop-checklist.md` — phrases and sentence structures that give away AI-written text
- `references/anti-slop-examples.md` — before/after examples of the fixes below
- `references/scoring-rubric.md` — how to turn what you found into one overall verdict for this piece

The checklist merges two established open-source anti-slop lists into one, de-duplicated and re-calibrated for marketing copy. See `anti-slop-checklist.md` for provenance.

## Before you start

You need to know **what channel this copy is for**: ad copy (statics, video ads, or UGC ad scripts — the primary text/caption/headline that runs with the ad), LinkedIn message, cold email, database/nurture email, organic post, or organic caption. If you weren't told, ask.

If you were given **a sample of copy that already sounds right for this brand**, read it first and match its voice in your suggested rewrites instead of a generic human voice — short sentences if they write short, "stuff" if they say "stuff" instead of upgrading to "elements."

This matters for one specific reason: some things that look like AI-slop in a normal message are deliberate, proven techniques in ad copy — short punchy triplets, dramatic contrast, staccato rhythm. Direct-response ads use these on purpose, and they work. A LinkedIn message or cold email doing the same thing reads as fake and salesy. Full detail in the "channel exception" section of `anti-slop-checklist.md`.

## Step 1 — Grammar & spelling

Read the copy in whichever language it's written. For Dutch or English, check it against `references/grammar-style-guide.md`'s calibrated rules. For any other language, still check it — don't skip it — using that language's general grammar/spelling knowledge per the guide's "Any other language" section, and cap `Confidence` at Medium accordingly. Flag real mistakes only — not style choices.

## Step 2 — Does it sound human

Read the copy again. Check it against `references/anti-slop-checklist.md`, applying the channel exception if this is ad copy.

**Do not flag a single isolated instance of a minor pattern.** One "actually," one adverb, one em dash — that's just normal writing. Only flag:
- Any single instance of a **strong** tell (a full AI-vocabulary sentence, a whole filler-opener sentence, a chatbot phrase like "I hope this helps")
- Or a **cluster** of two or more minor tells appearing close together

Read "What NOT to flag" in `anti-slop-checklist.md` before you write a single finding. A reviewer that flags everything gets ignored — don't be that reviewer.

Then score the piece using `references/scoring-rubric.md`. This gives the overall verdict for this check (clean / needs polish / needs another pass) — in addition to, not instead of, the individual findings below.

## How to write a finding

Every finding, from either step, uses this exact shape. No exceptions.

```
[Severity: blocker / should-fix / nit]
Quote: "the exact words from the copy"
Rule: which specific rule this breaks — name it, don't just say "sounds off"
Source: grammar-style-guide.md or anti-slop-checklist.md (name the file + section)
Confidence: High / Medium / Low
Why it matters: what a reader does or feels because of this
Fix: a real rewrite of that line — not "make it sound more human"
```

Step 1 (grammar/spelling) findings are mechanical — `Confidence: High` for Dutch or English (calibrated rules), capped at `Confidence: Medium` for any other language (no calibrated rule set behind it — see `grammar-style-guide.md`'s "Any other language" section). Step 2 (does-it-sound-human) findings are judgment — confidence required: High = unambiguous match to the checklist, Medium = matches but could plausibly be deliberate style, Low = borderline, include only as part of a cluster.

## Severity guide

- **Blocker:** a spelling/grammar mistake that changes meaning or sits in a headline, CTA, or brand name — OR a cluster of AI-slop tells that would embarrass the brand in front of a partner — OR the piece scores below the cutoff in `scoring-rubric.md`
- **Should-fix:** grammar awkwardness that doesn't confuse meaning — OR one or two isolated AI-slop tells
- **Nit:** a stylistic preference, or a single very minor tell

## Before you finalize the report

For every finding: re-read the quote and confirm it is copied exactly from the submitted text, and that the rule you named actually applies to it. Cut anything you can't verify this way. An ungrounded finding is worse than no finding — it costs trust in every other finding in the report.

---

*Part of the Creative Copywriting Bundle by [Sprints & Sneakers](https://sprintsandsneakers.com).*
