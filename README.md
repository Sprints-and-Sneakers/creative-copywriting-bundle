# Creative Copywriting Bundle

**By [Sprints & Sneakers](https://sprintsandsneakers.com)**

Six skills for Claude that turn brand and customer research into scored, production-ready ad copy.

Works in the Claude app, Claude Code, and the Claude API. No coding required.

> **New to this? Read [HOW-TO.md](HOW-TO.md).** It walks you through everything step by step.

These are agents rather than prompt templates, which mostly means they argue with themselves before they hand you anything. The copywriter writes a batch, scores it against 10 quality criteria, rewrites whatever falls below 8/10, and goes round again until the batch passes or it runs out of attempts. The reviewer then scores the same work cold, without knowing what the copywriter already fixed.

---

## Try it in two minutes

Every skill works on its own. You do not need the pipeline, a brief, or any research to get
something useful out of this.

Install `stop-slop-copy`, paste in ad copy you already have, and ask:

> Check this copy for typos and AI-sounding writing.

You get back severity-rated findings, each with the exact line quoted and a real rewrite. It also
knows the difference between a punchy triplet in an ad, where that is a deliberate technique, and
the same pattern in a cold email, where it reads as fake.

Then install `creative-reviewer`, paste the same copy, and ask it to score the ads. Two skills,
two minutes, no setup.

Once that earns its keep, the full pipeline below is where the real gains are.

---

## Install

### Claude app (browser or desktop)

You need a Pro, Max, Team, or Enterprise plan with file creation switched on.

Download this repo, then upload each zip from the `dist/` folder via **Settings → Features → Skills**. Upload them exactly as they are. Do not unzip them first.

There are 6 zips because Claude only accepts one skill folder per upload. You do not need all six. Start with `stop-slop-copy` and `creative-reviewer`, add the rest when you want them.

### Claude Code

```
/plugin marketplace add Sprints-and-Sneakers/creative-copywriting-bundle
/plugin install creative-copywriting
```

Or copy the folders manually:

```bash
cp -R skills/* .claude/skills/
```

Restart Claude Code afterwards.

### Claude API

Upload each skill through the `/v1/skills` endpoints with the `skills-2025-10-02` beta header, then reference the returned `skill_id` in the `container` parameter alongside the code execution tool.

> Skills do not sync between surfaces. Uploading to the Claude app will not make them available in Claude Code or the API, or the other way round. Install them wherever you plan to work.

---

## The skills

| Skill | What it does |
|---|---|
| `brand-brief` | Structured intake. Offer, audience, differentiation, goals. Marks gaps as `TBD` rather than inventing answers. |
| `creative-strategy` | Per-channel strategy (Meta, TikTok, YouTube) across 10 sections each, plus testing roadmap, production plan and KPI targets. |
| `creative-copywriter` | UGC scripts, founder ads, static copy, carousels, motion graphics. Writes modularly, so one angle yields ten or more usable variants. Self-reviews and rewrites until every ad scores 8+. |
| `creative-reviewer` | Independent quality gate. Scores every ad and returns specific rewrite instructions for anything it flags. |
| `wild-copywriter` | The 20% that breaks the rules. Run it alongside the copywriter for the experimental swings. |
| `stop-slop-copy` | Two-pass copy checker. First grammar and spelling, then whether it sounds like a person wrote it. Returns severity-rated findings with a real rewrite for each. It also knows that punchy triplets are deliberate in ad copy and fake in a cold email. |

The skills switch on by themselves when they are relevant, so you ask in plain language and Claude picks. They also work independently. If you already have a strategy, start at the copywriter. If you already have copy sitting in a doc somewhere, run the reviewer straight over it.

## Output

Plain markdown, organised under `output/{brand-slug}/`:

```
output/{brand-slug}/
├── 00-inputs/          your own data: past performance, swipe files
├── 01-research/        creative brief, VOC dictionary, segments, angle bank, gap matrix
├── 02-strategy/        creative strategy, testing roadmap, production plan, KPI dashboard
└── 03-copywriting/
    ├── scripts/        video scripts, one file per angle and format
    ├── static-copy/    static, carousel, motion graphics copy
    ├── copy-index.md   the map of the batch
    └── copy-review.md  scored review with rewrite instructions
```

---

## What this bundle does not do

It does not gather the research. The skills will run without it and tell you honestly what that costs, but they cannot go and find customer language for you.

Research is the other half of the job and it has its own bundle: **[Creative Research Bundle](https://github.com/Sprints-and-Sneakers/creative-research-bundle)**, which covers everything from customer intelligence through to a ranked angle bank. Run that first, then come back here.

This is worth taking seriously, because it decides almost everything about the output. What separates good ad copy from forgettable ad copy is whether the writer is working from real customer language or from its own assumptions. Give these skills a thin brief and you get competent, generic ads that could belong to any company in the category. Give them a few hundred real customer quotes sorted by pain, desire, objection and trigger, and the copy starts sounding like it came from someone who has actually met the customer.

You can supply that research in whatever form you already have it. An export, a document, pasted notes, a transcript from a sales call. The skills will ask. The only thing that really matters is that it is what customers actually said, rather than your summary of what they think.

Doing that research at real depth means full review corpora, competitor ad libraries and cross-source synthesis, which is what we run as a service. If you would rather have it done properly for your brand, talk to us at [sprintsandsneakers.com](https://sprintsandsneakers.com).

---

## Notes

Benchmarks in `skills/creative-strategy/references/benchmarks.md` carry a date stamp. Check it before you rely on the numbers.

After editing any skill, run `./build-zips.sh` to rebuild `dist/`.

---

## Credits

Built by **[Sprints & Sneakers](https://sprintsandsneakers.com)**, a performance creative and growth unit. These are the skills we use on client work, packaged so you can run them yourself.

Everything here is © Sprints & Sneakers: the pipeline, the quality criteria, the review loops, the anti-slop taxonomy, and the scoring and severity models.
