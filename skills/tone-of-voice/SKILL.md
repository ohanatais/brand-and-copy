---
name: tone-of-voice
description: >
  Define a product's voice and tone so it always sounds like itself — grounded in content-
  design evidence (Nielsen Norman Group's four tone dimensions, the voice-vs-tone
  distinction, and Podmajersky's Voice Chart). Produces a voice definition, a tone map for
  different contexts, a lexicon (words to use and words that break the voice), microcopy
  patterns for the moments that matter, and an optional guardrail to keep it consistent at
  scale — a system that makes every word, from the headline to an error message, sound like
  the same product wrote it.

  Make sure to use this skill whenever the user invokes /tone-of-voice or talks about how
  their product *sounds* in words — "define our voice", "how should the product talk",
  "write a voice and tone guide", "our copy sounds inconsistent / off / generic", "the app
  sounds like a robot", "make it sound more like us", "write error messages that aren't
  cold", "fix our microcopy", "our onboarding doesn't sound like our landing page", or "how
  do I keep my writing consistent" — even when they don't say "tone of voice". Also trigger
  right after brand identity is defined, as the verbal half of the same identity.

  Do NOT use for: the visual identity — colors, type, logo (use /brand-identity); writing a
  specific high-stakes conversion asset like the full landing page or onboarding flow from
  scratch (use /product-copy — though it should inherit the voice defined here); or strategic
  positioning and who the product is for (use /positioning or /personas). Voice is the
  *system*; product copy is one *output* of it.
---

# Tone of Voice

Tone of voice is not about being funny or formal. It is about being **consistent** — and
therefore recognizable. A product that sounds witty on the landing page, robotic in
onboarding, and apologetic in its error messages feels unfinished, even when the code is
flawless. The fix isn't "write better"; it's to define how the product talks *once*, so
every word after that sounds like the same person wrote it.

This skill helps a solo builder or small team define a **voice** (who the product is, in
words — constant) and a **tone** (how that voice flexes by context — variable), then turn
both into something reusable: a lexicon, microcopy patterns, and an optional guardrail. The
result is that the product sounds like itself everywhere, without you editing every string
by hand.

## Language rule

**Always respond in the user's language.** If the user writes in Portuguese (including
Brazilian Portuguese), respond entirely in Portuguese — every framework, label, and
example. This skill is written in English for GitHub conventions; the experience should
feel native. Voice is made of words, so language is not cosmetic here: a voice guide must
be written, and exemplified, in the language the product actually speaks. Never hand a
Portuguese product a voice illustrated only in English.

## The foundational distinction: voice vs. tone

Get this right and everything else follows (this is the Mailchimp content-design model, and
it's load-bearing):

- **Voice is constant.** It's the product's personality in words — the same whether things
  are going well or badly. Voice answers: *who is talking?*
- **Tone is variable.** It's how the voice adjusts to the moment — celebratory at a win,
  calm and plain at an error, brief in a button. Tone answers: *what does this moment need?*

A person has one voice but many tones: you're still you at a funeral and at a party, but you
don't talk the same way. A product is the same. Define the voice once; map the tones to the
contexts where they're needed.

## The model: five layers, in order

```
1. Voice      →  Who is this product, in words? (derived from brand personality, made verbal)
2. Tone       →  How does that voice flex across contexts and emotional states?
3. Lexicon    →  The words this product uses — and the words that break it
4. Microcopy  →  Voice applied to the small, high-stakes moments (errors, empty states, onboarding)
5. Guardrail  →  The voice doc + an optional check that keeps it consistent at scale
```

Why this order: tone is a *modulation of* voice, so voice comes first. The lexicon makes the
voice concrete enough to act on. Microcopy is where voice is most often dropped (and most
felt), so it gets its own layer. The guardrail is what makes the whole thing survive past
the founder's own keyboard.

Load `references/core-principles.md` for every session — it carries the evidence base (the
NN/g dimensions, the voice chart, and why consistency beats cleverness). Load
`references/components.md` when you reach the depth of any layer.

## Entry point: detect what already exists

**Signal 1 — is there a brand identity / personality?** Voice is the verbal expression of
the brand's personality. If `/brand-identity` (or positioning) defined an archetype and
adjectives, *reuse them* — the voice must agree with the visual identity, or the product
feels split. If none exists, name it once but don't block:

> "Voice is the spoken half of a brand's personality. Do you have a sense of the brand's
> character already — even three adjectives? If you've done /brand-identity or /positioning
> we'll build straight from that; if not, we can define a working personality here first."

**Signal 2 — is there existing copy?** Real strings (landing page, emails, errors) are the
best raw material — for defining voice *and* for auditing drift. Pull them in.

**Signal 3 — what do they need today?** Defining voice from scratch, producing the formal
voice chart + guardrail, or checking existing content for consistency?

Route:

| Mode | When | Reference |
|---|---|---|
| **guided** | Defining voice and tone for the first time | `references/mode-guided.md` |
| **chart** | Has the personality, wants the voice chart + lexicon + guardrail produced | `references/mode-chart.md` |
| **audit** | Has copy, wants it checked for voice consistency and drift | `references/mode-audit.md` |

If ambiguous, ask one question:

> "Are we defining the voice from scratch, writing up the formal voice guide, or checking
> existing copy for whether it sounds like one product?"

## How each layer is decided (the short version)

**1. Voice.** Make the brand personality verbal. Pick **three constraining adjectives** for
*how it writes* (not just what it is) — each must rule something out. Then place the voice on
**NN/g's four tone dimensions** as a default setting: Funny↔Serious, Formal↔Casual,
Respectful↔Irreverent, Enthusiastic↔Matter-of-fact (each a 3-point scale). This turns "be
friendly" into something measurable and repeatable.

**2. Tone.** For each adjective/dimension, define how it *shifts* by context. The sharpest
axis is emotional state: how the voice sounds at a win vs. at an error vs. when the user is
confused. Map the handful of contexts that actually recur in the product.

**3. Lexicon.** Make it concrete: words and phrases this product **uses** (its
vocabulary — names for things, signature turns of phrase) and words that **break** the
voice (jargon, clichés, anything that sounds translated or off-brand). The banned list is as
defining as the approved one.

**4. Microcopy.** Apply the voice where it's usually lost: error messages (never just
"Invalid"), empty states (a chance to set tone, not a dead end), onboarding's first
sentences, buttons and labels. These tiny moments carry disproportionate emotional weight.

**5. Guardrail.** Write the **voice chart / voice doc** (the deliverable). For teams or
AI-generated copy, optionally add a lightweight **consistency check** — a named list of
voice-breakers plus a small set of "golden" on-voice examples — so the voice holds even when
many hands (or models) write. See `references/components.md` for the technique.

## The "say it three ways" exercise

The most reliable way to make a voice *teachable* rather than vague. For a real message in
the product, write it three ways:

- **On voice** — exactly right.
- **Off voice** — a plausible version that breaks it (too stiff, too jokey, too generic).
- **On the edge** — almost right, but subtly wrong.

The contrast is what makes the voice legible to anyone else (including future-you and
Claude). A voice guide with three or four of these does more than a page of adjectives.

## Output always includes

1. **Voice definition** — three constraining adjectives + the position on NN/g's four
   dimensions + one paragraph on who's talking.
2. **Tone map** — how the voice flexes across the product's recurring contexts (especially
   the emotional ones: success, error, empty, confused).
3. **Lexicon** — words/phrases to use, and a named list of words that break the voice.
4. **Microcopy patterns** — on-voice examples for errors, empty states, onboarding, buttons.
5. **"Say it three ways" examples** — at least three, in the product's real language.
6. **Voice doc + optional guardrail** — offer to write the voice guide to a file; for
   scaled/AI writing, offer the consistency check.
7. **Next step** — usually `/product-copy`, which inherits this voice to write the
   high-stakes conversion copy.

## The early-stage posture

A solo builder doesn't need a 40-page voice bible. They need three sharp adjectives, the
four-dimension setting, a short banned-words list, and four "say it three ways" examples —
enough to keep the product sounding like one product. Ship that, keep it living, and deepen
it as more surfaces appear. Consistency, not completeness, is the win.
