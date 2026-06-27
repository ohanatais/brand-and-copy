---
name: product-copy
description: >
  Write product copy that converts — landing pages, onboarding, emails, and the words in
  between — grounded in copywriting evidence (Eugene Schwartz's five stages of awareness,
  jobs-to-be-done, voice-of-customer / message mining, and the features-to-benefits-to-
  meaning ladder). Matches the right message to the right reader at the right moment, in the
  product's own voice, and produces copy plus the reasoning behind every line so the founder
  can keep writing it themselves.

  Make sure to use this skill whenever the user invokes /product-copy or wants to write or
  improve the actual words that sell or activate the product — "write my landing page", "I
  need a headline", "what's my value proposition", "my copy isn't converting", "rewrite this
  hero section", "write onboarding copy", "write a CTA", "write a launch email", "the words
  on my homepage sound flat", or "say what we do in one sentence" — even when they don't say
  "copy". Also trigger right after voice and positioning are defined, as the place where both
  come alive.

  Do NOT use for: defining the voice/tone *system* itself (use /tone-of-voice — this skill
  inherits that voice); the visual identity, colors, type (use /brand-identity); or strategic
  positioning and personas (use /positioning and /personas — copy is downstream of them).
  This skill writes the words; the others decide who they're for and how they should sound.
---

# Product Copy

Copy isn't about sounding smart. It's about making the right person, in the right moment,
feel like this product was made for them. Generic copy is invisible — the reader's eyes
slide off it. Specific copy converts, because it sounds like it knows something true about
*them*. The difference is almost never talent; it's method: knowing who's reading, how much
they already know, what they actually want, and saying it in words they recognize.

This skill helps a solo builder write the copy that does real work — the landing page, the
onboarding, the emails — and, just as importantly, understand *why* each line is built the
way it is, so they can write the next one without help.

## Language rule

**Always respond in the user's language.** If the user writes in Portuguese (including
Brazilian Portuguese), write the copy and all guidance in Portuguese. This skill is in
English for GitHub conventions; the copy itself must be native — not translated. Copy
translated from English is the fastest way to sound generic in another market; the right
word is the one the reader would actually use.

## What this skill inherits

Copy is the last layer, not the first. It is strongest when it stands on:

- **Positioning / personas** (`/positioning`, `/personas`) — *who* it's for and *what makes
  it different*. The message comes from here.
- **Voice** (`/tone-of-voice`) — *how* it should sound. Copy must be written in the defined
  voice, or it fights the rest of the brand.

If these exist, pull them in and build on them. If they don't, you can still write good copy
by deriving a working version on the spot — but name the gap, because copy papering over an
undefined message will convert worse and you'll both be guessing.

## The model: five layers, in order

```
1. Reader & moment   →  Who is reading, and how aware are they? (Schwartz's 5 stages)
2. Message           →  The value proposition — one sentence that means something
3. Structure         →  The anatomy of the asset (landing / onboarding / email)
4. Craft             →  Lines that work: specific, benefit-with-meaning, in the reader's words
5. Proof & CTA       →  Earning belief (objections + evidence) and a CTA that feels inevitable
```

Why this order: you cannot choose a headline before you know how aware the reader is — the
same product needs a completely different first line for someone who doesn't know they have
the problem versus someone comparing you to a competitor. Message precedes structure;
structure precedes line-craft; proof and CTA close. Skip to "write me a headline" and you're
guessing at the one thing that determines everything.

Load `references/core-principles.md` every session (the evidence base and the "specific
beats clever" thesis). Load `references/components.md` when you reach the depth of any layer
or asset.

## Entry point: detect what already exists

**Signal 1 — message & voice.** Check for positioning/personas and a defined voice. Reuse
them. If missing, derive a working message and voice, and flag it.

**Signal 2 — the asset & the reader.** What are we writing (landing page, onboarding flow,
email, a single section)? And **where is the reader on the awareness ladder** when they hit
it? Cold traffic from an ad is Unaware/Problem-aware; someone on your pricing page is
Product-aware. This single question reshapes everything downstream.

**Signal 3 — from scratch or improving?** New copy, or fixing copy that isn't landing?

Route:

| Mode | When | Reference |
|---|---|---|
| **guided** | Writing a key asset for the first time, wants to understand the moves | `references/mode-guided.md` |
| **asset** | Knows the message and voice, wants the copy produced efficiently | `references/mode-asset.md` |
| **audit** | Has copy, wants it diagnosed and improved for clarity and conversion | `references/mode-audit.md` |

If ambiguous, ask one question:

> "What are we writing, and where's the reader's head when they land on it — do they already
> know they have this problem, or are we starting colder than that?"

## How each layer is decided (the short version)

**1. Reader & moment.** Place the reader on **Schwartz's five stages of awareness**: Unaware,
Problem-aware, Solution-aware, Product-aware, Most-aware. The stage sets the *job of the
opening*: an Unaware reader needs the problem named; a Solution-aware reader needs your
differentiation; a Most-aware reader just needs the nudge. Most failed copy is written one or
two stages ahead of where the reader actually is.

**2. Message.** Write the **value proposition**: what this does, for whom, and why it
matters — one sentence that *means something*, not "the best way to manage your work." Anchor
it in the **job to be done** (what the reader is hiring the product to accomplish) and the
differentiation (the "only"). Lead with value, not features.

**3. Structure.** Use the asset's anatomy as a checklist, not a cage. A landing page has a
job per section (hero → how it works → proof → objections → CTA); onboarding has an
activation arc; an email has one goal and one CTA. See `references/components.md`.

**4. Craft.** Make each line earn its place: **specificity** over generality, **benefits
with meaning** (features → what it does → what that means for *their* life — the "so what"
test, run twice), and **voice-of-customer language** — phrases the reader already uses, mined
from real reviews, support tickets, and interviews rather than invented. All of it in the
defined brand voice.

**5. Proof & CTA.** Handle objections *before* the reader has to voice them (without sounding
defensive), back claims with concrete proof, and write a CTA that reads as the obvious next
step — specific and low-friction, never pushy. A CTA feels inevitable when the copy above it
has already done the work.

## Output always includes

1. **Reader & awareness call** — who's reading and which stage, stated explicitly (it
   justifies every choice below).
2. **The value proposition** — the one-sentence message, plus the job-to-be-done it serves.
3. **The copy itself** — drafted for the asset, in the product's voice and language, with
   structure labeled (what each section/line is doing).
4. **The reasoning** — short notes on *why* the key lines are built that way, so the user can
   write the next one.
5. **Proof & objections handled** — what's claimed, how it's backed, which objection each
   piece answers.
6. **A clarity check** — the 5-second test (can a stranger say what this is and who it's for?)
   and the "so what" pass on every benefit.
7. **Variations & next step** — 2–3 alternative headlines/CTAs to test, and the handoff
   (ship it, A/B test, or `/go-to-market` for distribution).

## The early-stage posture

Pre-product-market-fit, copy is a hypothesis you're testing, not a monument. Write it
specific and clear, ship it, and **change it when real readers tell you what lands** — their
words are better than yours. Favor one sharp claim you can defend over five vague ones, and
mine actual customer language the moment you have any. Clarity first, cleverness never
required.
