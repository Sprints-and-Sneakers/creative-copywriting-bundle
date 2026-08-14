# Grammar & Spelling — Baseline Rules

**Scope: generic professional-writing rules.** These are brand-agnostic. If your brand has its own tone rules (formal vs. informal address, banned words, brand-name formatting), supply them and apply those on top. Do not invent brand-specific rules to fill a gap.

This file is self-contained on purpose, so the skill still works when uploaded on its own.

## What counts as a real mistake (flag these)

- Misspelled words
- Wrong verb conjugation or tense
- Subject-verb agreement errors ("the team are" instead of "the team is")
- Wrong word entirely (there/their/they're, its/it's, dan/als in Dutch comparisons)
- Missing or extra words that change meaning
- Wrong capitalization of brand/product names
- Punctuation that changes meaning (missing comma that creates ambiguity, not a missing Oxford comma)
- Number/currency formatting errors for the language (Dutch: "€19,99" not "€19.99"; English: the reverse)

## What does NOT count as a mistake (do not flag these)

- Sentence fragments used on purpose for rhythm ("Simple. Fast. Done.") — that's a style choice, not an error
- Starting a sentence with "En," "Maar," "And," or "But" — fine in marketing copy
- Informal contractions ("don't," "je," "'t") — expected in conversational copy
- One missing Oxford comma, or a style preference either way
- Deliberate lowercase for brand voice reasons (a brand that never capitalizes its own name)

## Common Dutch mistakes to check for

- de/het article errors
- English loanwords used with Dutch grammar incorrectly attached
- Hoofdletters (capitals) in the middle of a sentence where not needed

### Compound nouns wrongly split (*de Engelse ziekte*)

The single most common error in Dutch marketing copy, and the one a Dutch reader notices fastest — splitting a compound noun into separate words the way English would. Named *de Engelse ziekte* ("the English disease") for exactly this reason.

- "web site" → **webshop**, not "web shop"
- "klant contact" → **klantcontact**, not "klant contact"
- "doelgroep analyse" → **doelgroepenanalyse**, not "doelgroep analyse"

Flag every instance — this is a mechanical error, `Confidence: High`, not a style call.

### Tussen-n errors

Whether a compound needs a connecting -n- between its parts (klant + service = klantenservice, not klantservice) follows a real but complex rule (plural-in--en gets the -n-, with exceptions). Rather than encoding the full rule, check against this common-word lookup list first, and treat anything not on the list as a judgment call:

- klantenservice (not klantservice)
- medewerkerstevredenheid
- gegevensbescherming
- doelgroepenanalyse
- klantenbestand
- productencatalogus

A hit against this list is `Confidence: High`. A compound not on the list that looks wrong is `Confidence: Medium` — flag it, but don't present it as certain.

### dt-fouten (verb conjugation)

| Form | Rule | Example |
|---|---|---|
| ik-vorm | stam (no -t) | ik word, not ik wordt |
| jij/hij-vorm, present tense | stam + t | jij wordt, hij wordt |
| voltooid deelwoord | 't kofschip rule — -t after a voiceless consonant (t, k, f, s, ch, p), -d otherwise | gewerkt (werk+t), geland (land+d) |

Before: "Hij word elke dag actiever." After: "Hij wordt elke dag actiever." (jij/hij-vorm needs the -t)
Before: "Het is getest en goedgekeurt." After: "Het is getest en goedgekeurd." (kofschip: goedkeuren → goedgekeurd, "keur" ends in a voiced sound)

### hun/hen

Direct object → hen. Indirect object (after a preposition, or "aan"/"voor" implied) → hun. "Ik zag hen" (direct object) vs. "Ik gaf hun het rapport" (indirect object, "aan hen" implied). One of the most common native-speaker errors too — flag it at `Confidence: High` when clearly wrong, `Medium` when genuinely ambiguous (this distinction is eroding in spoken Dutch).

## Common English mistakes to check for

- Its vs. it's
- Affect vs. effect
- Then vs. than
- Subject-verb agreement across a long clause ("the list of features are" — wrong, "is")
- Dangling modifiers that create an unintended meaning

## Any other language

Dutch and English are the only languages with hand-calibrated rules above — real, deliberately hand-tuned ones (the tussen-n/dt-fouten/hun-hen rules didn't come from generic knowledge, they came from actual Dutch marketing-copy patterns). Don't pretend that same level of calibration exists for other languages.

If copy shows up in a language other than Dutch or English (e.g. German, French, Spanish), still check it — don't skip it just because there's no dedicated section for it. Apply the "What counts as a real mistake" / "What does NOT count as a mistake" principles above (they're language-agnostic: misspellings, wrong conjugation, subject-verb agreement, wrong word entirely, meaning-changing punctuation, number/currency formatting for that language) using general knowledge of that language's grammar. Flag real, unambiguous errors — the kind a native speaker would immediately catch, not a marginal style call you're guessing at.

**Cap `Confidence` at Medium for any non-Dutch/English finding, even an error that feels certain.** There's no calibrated rule set behind it the way there is for Dutch/English, so it doesn't earn the same `High` a tussen-n error or an its/it's mix-up gets. If you're genuinely unsure whether something is a real mistake or a valid regional/dialect variant, don't flag it at all rather than flagging it at `Confidence: Low` — a wrong guess in an unfamiliar language costs more trust than staying silent.

## How to report a finding

Same shape as every other finding in this skill:

```
[Severity: blocker / should-fix / nit]
Quote: "the exact words from the copy"
Rule: the specific rule broken
Source: grammar-style-guide.md
Confidence: High for Dutch/English (mechanical, calibrated) / Medium cap for any other language (see "Any other language" above)
Why it matters: what a reader would notice or misread
Fix: the corrected version
```

Grammar/spelling severity:
- **Blocker** — the mistake changes meaning, or sits in a headline, CTA, or brand name
- **Should-fix** — a real mistake, but meaning stays clear
- **Nit** — arguable, a style call either way
