---
name: brand-identity
description: >
  Visual and verbal brand identity for solo builders and small teams — grounded in
  brand-strategy evidence (Aaker's five personality dimensions, Mark & Pearson's
  archetypes, Neumeier's onliness/differentiation, and color research showing that
  color meaning is contextual, not universal). Builds identity in dependency order:
  personality → color → typography → logo → documentation, and produces a brand
  brief plus reusable design tokens that Claude, a designer, or future-you can apply
  consistently without the founder in the room.

  Make sure to use this skill whenever the user invokes /brand-identity or talks about
  creating or refining a brand's look and feel — "I need a brand", "give my product an
  identity", "help me choose colors / a palette", "pick fonts / typography", "design a
  logo", "what's my brand personality / archetype", "write brand guidelines", "make a
  design system / tokens", "my product looks generic / like every other AI app", or
  "does my visual identity feel right" — even when they don't say the words "brand
  identity". Also trigger right after positioning or personas are defined and the
  natural next step is giving the product a face.

  Do NOT use for: writing the words on the page — headlines, landing copy, onboarding
  (use /product-copy); defining how the product *talks*, its voice and tone in sentences
  (use /tone-of-voice); strategic positioning or who the product is for (use /positioning
  or /personas); or implementing UI components and front-end code (that's a build task,
  not identity design).
---

# Brand Identity

Brand identity is not decoration you add at the end. It is the first decision your user
makes about whether to trust you — made in the half-second before they read a single
word. The colors, the type, the logo, and the personality underneath them all are part
of the product. They decide whether someone understands what you built, feels it was made
for them, and stays.

This skill helps a solo builder create a coherent visual and verbal identity **without a
designer** — not by guessing at taste, but by deriving every choice from what the brand
actually stands for. The output is a brand brief and a set of design tokens: a system
someone can apply consistently when you are not there to explain it.

## Language rule

**Always respond in the user's language.** If the user writes in Portuguese (including
Brazilian Portuguese), respond entirely in Portuguese — every framework, label, table,
and section header. This skill is written in English for GitHub conventions; the
experience should feel native to whoever is using it. Brand identity is culturally loaded
(color meaning, type feel, and naming all shift by culture), so working in the user's
language is not cosmetic — it changes the recommendations.

## The model: five components, always in order

Brand identity is built like positioning — in a fixed sequence where each component
depends on the one before it. Work out of order and the whole thing collapses into taste.

```
1. Personality   →  Who is this brand, as if it were a person? (archetype + traits + the "only")
2. Color         →  A palette that expresses that personality on purpose, not by preference
3. Typography    →  Type as the brand's speaking voice; what the words feel like before they're read
4. Logo          →  The simplest mark that carries the personality and survives at 16px
5. Documentation →  The brand doc + tokens that make all of the above reproducible without you
```

Why the order is non-negotiable:

- **Color is only "right" relative to a personality.** Purple is not premium or playful in
  the abstract — it depends on what the brand is trying to be. Color research (Labrecque &
  Milne) shows hue-to-personality links exist but are moderated by context, category, and
  culture. So you cannot choose color until you know the personality it must serve.
- **Type is a voice**, and a voice needs a character to belong to. A serif with optical
  wonk says something different on a banking app than on a poetry zine.
- **A logo assembles** the personality, color, and type into one mark. With nothing above
  it, a logo is just a shape you happen to like.
- **Documentation is what turns choices into a system.** An identity that lives only in
  your head is not an identity; it is a mood. The brand doc is the actual deliverable.

Load `references/core-principles.md` for every session, regardless of mode — it carries
the evidence base (the frameworks, the color caveat, and the anti-clichés) that keeps the
work honest.

## Entry point: detect what already exists

Before routing to a mode, read the conversation for what the user brings:

**Signal 1 — is there a strategy to express?** Identity is the face of a positioning. If
there is no positioning or persona work, name it once — don't block:

> "Identity works best when it has something to express. Do you have a sense of who this
> is for and what makes it different — even a hypothesis? If positioning isn't defined yet,
> we can build identity around a working thesis and tighten it later. (/positioning and
> /personas go deeper if you want to do that first.)"

If they have positioning/personas: use them as the source of the personality. Real
differentiation ("the only ___ that ___") is the richest input there is.

**Signal 2 — is there an existing identity?** Some colors, a logo, fonts already in use?
→ this is an **audit**, not a blank page. Don't redesign reflexively; diagnose first.

**Signal 3 — how much do they want to decide today?** A founder pre-launch may want the
whole system; someone mid-build may just need to lock a palette or sanity-check a logo.
Scope to the real need.

Route:

| Mode | When | Reference |
|---|---|---|
| **guided** | First time, or building identity from scratch | `references/mode-guided.md` |
| **brief** | Has positioning/personas, wants the brand brief + tokens produced efficiently | `references/mode-brief.md` |
| **audit** | Has an identity, wants it critiqued for coherence, clichés, and accessibility | `references/mode-audit.md` |

If it's ambiguous, ask one question:

> "Are we creating identity from scratch, producing the brief from positioning you already
> have, or pressure-testing an identity that exists?"

Whenever you reach the depth of a specific component (color, type, logo, documentation),
load `references/components.md` — it holds the per-component method plus short,
*contrasting* examples (a warm cultural brand, a precise fintech, a rugged outdoors
brand) so the method is visible without any single aesthetic being implied as "correct."

## This skill is universal — adapt to the user's reality

The frameworks here are fixed; the outputs are not. The same five-component method must
produce a warm, handwritten-feeling brand for one user and a stark, technical one for the
next — because each is derived from *that* user's personality, category, and culture, not
from a house style. Treat every example in the references as an illustration of *how to
decide*, never as a destination. If you ever find the recommendation drifting toward "make
it look like this nice brand I know," stop and re-derive from the user's own onliness line
and archetype. A founder should finish a session with an identity that feels unmistakably
theirs, in their language and their market — not a copy of someone else's good taste.

## How each component is decided (the short version)

The reference files go deep; this is the spine so you can hold the whole thing in mind.

**1. Personality.** Name the brand as a person. Use two grounded frameworks together, not
vibes: pick a primary **archetype** (Mark & Pearson's 12 — the dominant human drive the
brand speaks to) and **three personality adjectives** (anchored in Aaker's five dimensions
— Sincerity, Excitement, Competence, Sophistication, Ruggedness — so the words actually
constrain choices). Then write the **onliness line** (Neumeier): "the only ___ that ___."
Three adjectives that could describe any brand ("modern, clean, trustworthy") have failed —
push until they exclude something.

**2. Color.** Derive a palette from the personality, then pressure-test it. One dominant
brand color, one accent used as *punctuation* (rarity is its power), warm/neutral bases,
and semantic colors (success, error). Name colors by role and meaning, not by hex. Always
verify text contrast (WCAG 4.5:1 for body) before shipping a color. Resist universal
"color psychology" claims — anchor to the personality and category, and flag where culture
changes the read.

**3. Typography.** Choose type as voice. Usually two families (a display/character face +
a legible workhorse), three at most. Pair for contrast with a reason. Define one
**signature move** the brand owns. Check legibility at the smallest real size, not just in
the hero.

**4. Logo.** The test is not "is it beautiful" but "does it survive." Simple enough to read
at 16px and in one color, memorable, and true to the personality. For a solo builder, a
strong wordmark with one deliberate detail beats an ambitious symbol that reads as a smudge.

**5. Documentation.** Produce the artifact: a brand doc (personality, palette with roles,
type system, logo usage, do's/don'ts) and machine-usable **design tokens** (color, type,
spacing, radius). This is what lets Claude or a designer apply the brand without you.

## Output always includes

Whatever the mode, every brand-identity session ends with:

1. **Personality statement** — primary archetype + three constraining adjectives + the
   onliness line. One short paragraph, for internal alignment.
2. **Color system** — each color named by role, with its rationale and a contrast note.
3. **Type system** — families, pairing rationale, hierarchy, and the signature move.
4. **Logo direction** — the concept and why it fits (final art optional; direction required).
5. **Brand documentation + tokens** — the reproducible deliverable (offer to write it to a
   file, e.g. `DESIGN.md` or `brand.md` + a tokens block).
6. **What this identity rules out** — the anti-patterns and clichés this brand will not use.
   Naming what you reject is as defining as what you choose.
7. **Open questions & next step** — what's still a hypothesis, and the explicit handoff:
   usually `/tone-of-voice` (the verbal half of the same identity), then `/product-copy`.

## The early-stage exception

For a solo builder pre-product-market-fit, hold identity **firmly enough to be coherent,
loosely enough to evolve.** The personality and the core color/type decisions should be
real and committed — coherence is what makes a small product feel trustworthy. But don't
over-invest in an exhaustive 60-page brand bible before anyone uses the product. Ship a
tight one-page brand doc plus tokens, and deepen it as the product earns the right. Include
this note in early-stage output:

> "This is enough identity to launch with and look intentional. Treat the brand doc as
> living — revisit it once real users tell you what the product actually feels like to them."
