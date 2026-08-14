# Structural Slop

Sentence and paragraph patterns that mark copy as machine-written, even when every individual word
is fine. Bilingual: Dutch and English.

These are harder to spot than the word-level tells in `07-anti-slop-phrases.md` and they do more
damage, because a reader cannot point at what is wrong — the copy simply fails to land.

**Before flagging section 1, read the ad-copy exception at the bottom.** It changes the rules.

---

## 1. Manufactured drama

Structures that fake tension the content has not earned.

**Binary contrasts.** The reversal is visible from the opening clause.

- EN: "Not because X. Because Y." / "The answer isn't X, it's Y." / "It feels like X. It's actually Y."
- NL: "Niet omdat X. Maar omdat Y." / "Het antwoord is niet X. Het is Y." / "Het voelt als X. Het is eigenlijk Y."

State the conclusion. Drop the setup.

**Negative listing.** "No X. No Y. A Z." / NL: "Geen X. Geen Y. Een Z." A striptease in front of an
ordinary point. State Z.

**Period-stacking.** Verbless fragments in sequence: "Four minutes. On the toilet. Scrolling."
Two measurable tests:

- More than 10 full stops per 100 words in spoken or UGC-style copy is a problem. More than 13 is an automatic rewrite.
- Three or more consecutive sentences under 8 words is fragmentation. Rejoin with and / but / because / while / so — NL: en, maar, omdat, terwijl, dus.

**Rule-of-three lists.** Two items, or one. Three is the model's default cadence.

**The one-liner habit.** Every paragraph landing on a short punchy closer.

**Rhetorical wind-ups.** "What if [reframe]?", "Here's what I mean:", "Think about it:" / NL: "Wat
als...?", "Dit bedoel ik:", "Denk er eens over na:". They promise insight and make the reader wait.

**Em-dash conversion damage.** After removing an em dash, inspect the full stop it left behind. It
usually wanted to be a comma, or and / but / because — not a sentence break.

---

## 2. Distance from the subject

Nobody is present. No person acts. The writer observes from above the scene, and the copy stops
sounding like it came from anyone.

**Passive constructions.** Every sentence wants a human subject performing a verb. "Mistakes were
made" / NL: "Er zijn fouten gemaakt" → name who made them.

**Objects performing human actions.** "The complaint becomes a solution", "the decision emerges",
"the data tells us" / NL: "De klacht wordt een oplossing", "het besluit ontstaat". Abstractions
cannot act. Name the person.

**Narration from orbit.** "Nobody designed this", "This happens because" / NL: "Niemand heeft dit
ontworpen". Put the reader in the room. "Je" outperforms "mensen"; "you" outperforms "people".

**Copula avoidance.** "serves as", "stands as", "represents" where "is" would do / NL: "fungeert
als", "vertegenwoordigt". Use "is".

**Participle tails.** "...highlighting the brand's commitment", "...reflecting a broader shift" /
NL: "...wat de toewijding onderstreept". A clause bolted on to manufacture significance. Cut it.

**Question-word openers.** Sentences beginning What / When / Where / Which / Who / Why / How — NL:
Wat / Wanneer / Waar / Welke / Wie / Waarom / Hoe. Restructure to lead with the subject or verb.

**Formulaic constructions.** "Not only... but also" / NL: "Niet alleen... maar ook". Symmetrical
pairs that signal assembly rather than thought.

---

## 3. Surface tells

Cheap to check. They cluster with everything above.

Em dashes. Curly quotes in plain-text copy. Emoji in headings. Title Case In Headings. Bold applied
to whole sentences instead of single terms. Hyphenated pairs sitting after the noun ("the report is
high-quality" wants "high quality").

---

## 4. Em dashes are language-dependent

**Dutch:** a single em dash (U+2014) is a tell on its own, at high confidence, with no supporting
evidence needed. Dutch typography uses a spaced en dash (–) for the *gedachtestreepje*. An unspaced
em dash is rare enough in native Dutch commercial writing that it usually means the text came
straight out of a model unedited.

**English:** one em dash proves nothing. Editors and journalists use them constantly. Only flag as
part of a cluster.

---

## 5. The ad-copy exception — read before flagging section 1

Staccato rhythm, hard contrast and triplets are deliberate, tested techniques in **ad copy**: the
primary text, caption or headline running with a static, video or UGC ad. Direct-response training
teaches them on purpose, and they work.

The identical pattern inside a LinkedIn message, cold email, organic post or organic caption reads
as manufactured.

**Channel is ad copy:** flag section 1 only when a pattern is extreme — well past the numeric
thresholds above — or clearly accidental, such as fallout from an em-dash conversion rather than a
deliberate hook.

**Every other channel:** section 1 applies in full.

---

## 6. Flag clusters, not instances

One dash, one "however", one adverb is normal writing. The Dutch em dash in section 4 is the only
standalone exception.

The real signal is accumulation: em dashes plus a triplet plus "vibrant tapestry" plus a
summarising wrap-up, all inside one piece.

**Protect these** — signs a human wrote it, and editing them out makes the copy worse:

- A specific detail nobody would invent: an odd number, a stray aside, a real name
- Unresolved tension instead of a tidy conclusion
- Genuine self-correction mid-thought
- Sentence lengths that vary inside one paragraph
- A first-person opinion the writer could defend if challenged
