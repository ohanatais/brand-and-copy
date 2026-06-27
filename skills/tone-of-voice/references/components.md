# Component Deep-Dives

The per-layer method. Load when a session reaches the depth of an actual layer. Examples
use three *contrasting* voices so the method is visible without implying one is correct:

- **Voice A — "warm & spirited"** (a consumer product that wants to feel human).
- **Voice B — "precise & calm"** (a B2B tool where trust and clarity lead).
- **Voice C — "blunt & energetic"** (a challenger product that breaks category politeness).

The user's voice is almost certainly none of these exactly — derive theirs.

## Contents
- [1. Voice](#1-voice)
- [2. Tone](#2-tone)
- [3. Lexicon](#3-lexicon)
- [4. Microcopy](#4-microcopy)
- [5. Guardrail & documentation](#5-guardrail--documentation)

---

## 1. Voice

**Goal:** a definition of *who is talking* that someone else can hit consistently.

**Method:**
1. Start from the brand personality (archetype + adjectives from `/brand-identity` or
   `/positioning`). If absent, derive a working personality first — voice with no character
   behind it is just style.
2. Choose **three adjectives for how it writes** — not what the brand *is* in the abstract,
   but how that shows up in sentences. Each must exclude something. "Clear" is weak;
   "clear, unhurried, never cute" rules things out.
3. Set the **default on NN/g's four dimensions** (each 3-point): Funny↔Serious,
   Formal↔Casual, Respectful↔Irreverent, Enthusiastic↔Matter-of-fact. This is the
   repeatable setting.
4. Write **one paragraph** describing the voice as a person: who they are, how they make the
   reader feel, what they'd never do.

| | Voice A (warm) | Voice B (precise) | Voice C (blunt) |
|---|---|---|---|
| Adjectives | warm, spirited, unpretentious | exact, calm, plain | blunt, energetic, no-jargon |
| Funny↔Serious | leans funny | serious | leans funny |
| Formal↔Casual | casual | neutral | casual |
| Respectful↔Irreverent | respectful | respectful | irreverent |
| Enthusiastic↔Matter-of-fact | enthusiastic | matter-of-fact | enthusiastic |

Same four dimensions, three different settings — three unmistakably different products.

---

## 2. Tone

**Goal:** how the constant voice flexes to fit each recurring moment.

**Method:**
1. List the **contexts that actually recur** in this product — don't theorize all of them.
   The usual high-value set: success/celebration, error/failure, empty state, confusion/help,
   first-run onboarding, destructive confirmation, billing/money.
2. For each, note **which way the dimensions shift** from the default. The emotional axis
   matters most: a voice that's enthusiastic by default must *dial enthusiasm down* at an
   error — celebrating near someone's failure reads as tone-deaf.
3. Capture each as a one-line rule: "At an error: stay calm and plain, take responsibility,
   say what to do next. Never joke, never blame the user."

**Example — same warm Voice A, three moments:**
- *Win:* "Nice — that's your third week in a row." (enthusiasm up)
- *Error:* "That didn't save. Your text is still here — try again in a moment."
  (enthusiasm down, calm, reassuring, actionable)
- *Empty state:* "Nothing here yet. Add your first one and it'll show up here." (inviting,
  not a dead end)

The voice is the same person throughout; only the tone moved.

---

## 3. Lexicon

**Goal:** make the voice concrete at the word level.

**Method:**
1. **Words/phrases to use** — the product's actual vocabulary: what it calls its core
   objects and actions, signature turns of phrase, the person it speaks in (you/we), and its
   punctuation habits (per Podmajersky's voice chart). Consistency in *naming* is half of
   sounding coherent.
2. **Words/phrases that break the voice** — a **named banned list** specific to this
   product. This is as defining as the approved list. Pull a starting set from the anti-tells
   in `core-principles.md`, then make it the user's own: add their pet peeves, remove what
   doesn't apply. One product bans exclamation points; another runs on them.
3. **Show the swap** — for each banned item, the on-voice replacement, so the rule is
   actionable, not just a prohibition.

| | Voice A | Voice B | Voice C |
|---|---|---|---|
| Uses | "you", contractions, plain verbs | "you", full words, exact nouns | "you", short imperatives, slang sparingly |
| Avoids | corporate jargon, hype adverbs | exclamation points, vague claims | hedging, "just", filler politeness |
| Person | second person, friendly | second person, neutral | second person, direct |

---

## 4. Microcopy

**Goal:** keep the voice in the small, high-stakes moments where it's usually dropped.

These tiny strings carry outsized emotional weight — they're where users are most frustrated,
most lost, or most delighted. A product that nails its hero headline but ships "Error: null"
has a broken voice.

**Patterns:**
- **Error messages** — say what happened, reassure (their data is safe if it is), and give
  the next action. Never just "Invalid" or "Something went wrong." Never blame the user.
- **Empty states** — treat as an invitation and a tone-setter, not a blank. Say what will
  appear here and how to start.
- **Onboarding first lines** — the first five sentences decide whether someone stays. Speak
  to the value, in the voice, immediately; don't make them read a manual.
- **Buttons & labels** — verbs that match the voice and the action ("Save and continue" vs.
  "Submit"). Consistent capitalization and length.
- **Confirmations (especially destructive)** — be clear and calm about consequences; this is
  not the place for cleverness.

Always demonstrate these in the user's real language with real product nouns, not lorem.

---

## 5. Guardrail & documentation

**Goal:** make the voice survive past the founder's own keyboard — across surfaces, teammates,
and AI-generated copy.

**The voice doc (always).** Write the deliverable: the voice definition (adjectives + four-
dimension setting + paragraph), the tone map, the lexicon (use/avoid with swaps), the
microcopy patterns, and 3–4 "say it three ways" examples. Offer to write it to a file in the
user's project (e.g. `VOICE.md` or `voice.md`). This is what lets anyone — or Claude — write
on voice without the founder present.

**The consistency check (optional, for scale or AI writing).** When copy will be produced at
volume or generated by a model, a prose guide isn't enough — voice drifts silently. A
lightweight, *deterministic* guardrail catches it:

1. **A named list of voice-breakers** — the banned words/phrases/patterns from the lexicon,
   each as a checkable rule ("no em-dash", "no hype adverb from this set", "metric claims
   always include a timeframe"). String/regex matching, no judgment call needed.
2. **A golden set** — a handful of *approved* on-voice examples (one per content type) that
   should always pass the rules and represent the target. They double as the reference for
   "what good sounds like" and as a regression guard: if a future prompt change makes a
   golden example fail, the voice has drifted.
3. **Run it where copy is generated or reviewed** — a quick check in CI, a pre-publish lint,
   or simply a checklist Claude applies before shipping strings.

This technique is *structure, not content*: the rules and golden examples are entirely the
user's own voice. The same scaffold enforces a buttoned-up B2B voice and an irreverent
consumer one — only the banned list and the golden examples differ. That's what makes it a
reusable system rather than one product's rulebook.

A minimal guardrail shape (fill with the user's own rules and examples):

```
voice-breakers:   [ list of banned words / phrases / patterns, each checkable ]
golden-examples:  [ one approved, on-voice sample per content type ]
check:            run breakers over new copy; confirm golden examples still pass
```
