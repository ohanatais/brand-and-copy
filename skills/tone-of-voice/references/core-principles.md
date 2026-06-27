# Core Principles

Loaded for every tone-of-voice session. The evidence base and the stances that keep the
work honest — so the product ends up sounding like *itself*, not like a nicer template.

## The thesis: consistency is the product, not cleverness

The instinct is to ask "should we be funny? professional? quirky?" That's the wrong first
question. The thing users actually feel is **consistency** — whether the landing page, the
onboarding, the buttons, and the error messages sound like one coherent person. An
inconsistent voice reads as carelessness, even when each individual sentence is fine. A
consistent voice — even a plain one — reads as a product that has its act together.

So the goal is never "a more impressive voice." It's a voice that is *recognizable and
repeatable* across every surface and every author (including AI). Optimize for "this sounds
like us" over "this is a great line."

## Voice vs. tone (the load-bearing distinction)

From content design practice (canonically, Mailchimp's content style guide):

- **Voice is constant** — the product's personality in words. It does not change between a
  celebration and an error. Voice = *who is talking.*
- **Tone is variable** — how that voice adapts to the moment. Tone = *what this moment
  needs.*

The human analogy: you have one voice and many tones. You're recognizably you whether you're
consoling a friend or cracking a joke, but you modulate. Conflating the two is the most
common mistake — people either freeze the tone (robotic sameness) or let the voice drift
(no identity). Define voice once; map tone to contexts.

## Framework 1 — NN/g's four dimensions of tone

Nielsen Norman Group's research gives voice and tone something most "be friendly" advice
lacks: a way to *measure* it. Any piece of writing can be placed on four dimensions, each a
3-point scale (one side, neutral, the other side):

1. **Funny ↔ Serious**
2. **Formal ↔ Casual**
3. **Respectful ↔ Irreverent**
4. **Enthusiastic ↔ Matter-of-fact**

Two reasons this matters:

- **It makes voice repeatable.** "Casual, serious, respectful, matter-of-fact" is a setting
  someone else can hit consistently. "Friendly" is not.
- **It has measured effects.** NN/g found tone measurably shifts users' impressions of an
  organization's *friendliness, trustworthiness, and desirability* — so this is a lever on
  perception, not decoration. Critically, the right setting is **context-dependent**: a
  playful error message can read as careless during a failure. Tone must fit the moment.

Use the four dimensions twice: once to set the **default voice**, and again to describe how
each dimension **shifts by context** (the tone map).

## Framework 2 — The Voice Chart (making it actionable)

From Torrey Podmajersky's *Strategic Writing for UX*: a voice derives from **product
principles** (what the experience is trying to be for its users) and is captured in a
**voice chart** with concrete columns:

- **Concepts** — the ideas/themes the product keeps returning to
- **Vocabulary** — the words it uses (and the ones it avoids)
- **Verbosity** — how much it says; the balance of information and brevity
- **Grammar** — sentence shape, person (you/we), simplicity
- **Punctuation & capitalization** — the small consistent habits that build familiarity

The value of the chart is that it turns "personality" into columns someone can *apply* line
by line. It's the bridge from adjectives to actual strings.

## Universal by design — derive from this product

The frameworks are fixed; the output must not be. The same method has to produce a dry,
precise voice for a compliance tool and a warm, irreverent one for a hobby app — because each
is derived from *that* product's personality, audience, and language. If two different
products would get a similar voice out of this skill, something is being defaulted. Every
example in these files is an illustration of *how to decide*, never a target to copy. When a
recommendation starts sounding like "write it the way this cool brand writes," stop and
re-derive from the user's own adjectives and four-dimension setting.

This is also why the **lexicon and the banned list are per-product.** One product bans
exclamation points; another lives on them. One forbids a word the next one owns. There is no
universal list of "bad words" — only words that break *this* voice.

## The anti-AI / anti-generic tells (one application, not the definition)

A frequent, legitimate use of this skill is making copy stop sounding like generic AI
output. Common tells to watch for — useful as a *starting* checklist the user then makes
their own:

- The em-dash-and-antithesis cadence: "It's not X — it's Y." Striking once, hollow on repeat.
- Empty intensifiers and hype adverbs ("truly", "seamlessly", "effortlessly").
- Translated-from-English phrasing in a non-English product ("potencialize", "maximize seu
  impacto") — it reads as foreign to a native speaker.
- Buzzwords and platform jargon used as filler ("leverage", "unlock", "supercharge").
- Praise inflation and exclamation spam where calm would read as more confident.
- Decorative emoji standing in for actual warmth.

Treat this as a template the user *edits*, not a law. The point isn't these specific items —
it's the habit of naming, for this product, the things that break its voice, so they can be
caught. (For one way to enforce such a list at scale, see the guardrail technique in
`references/components.md`.)

## Accessibility and plainness

Clarity is part of voice, not opposed to it. Favor plain language, short sentences, and the
second person where it fits; a voice nobody can parse isn't characterful, it's broken. Even
the most playful voice should be readable, scannable, and unambiguous in the moments that
carry stakes (errors, confirmations, money, data).
