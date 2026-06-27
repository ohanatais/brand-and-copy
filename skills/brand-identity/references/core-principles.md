# Core Principles

Loaded for every brand-identity session, regardless of mode. These are the evidence base
and the non-negotiable stances that keep the work honest — so it produces a brand the user
*owns*, not a nicer version of someone else's.

## The one rule above all others: derive, never default

Every visual choice must trace back to something the brand stands for. The moment a
recommendation is justified by "this looks good" or "this is what modern products do," it
has failed. Color, type, and logo are downstream of personality; personality is downstream
of positioning. When you can answer "why this and not the opposite?" with a reason that
points at the brand's strategy, the choice is earned.

This is also what makes the skill universal. The same method must be able to output a soft,
hand-drawn identity for a children's-book app and a hard, monospaced identity for a
developer tool — because each is derived from a different personality, category, and
culture. If two different users would get recognizably similar brands out of this skill,
something is being defaulted instead of derived. Examples in these files show *how to
decide*; they are never the destination.

## Framework 1 — Brand personality: archetype + traits

Two complementary, research-grounded lenses. Use them together; neither alone is enough.

**Mark & Pearson's 12 archetypes** (*The Hero and the Outlaw*, 2001, adapting Jung). Each
archetype is a dominant human drive a brand can speak to. Pick **one primary** (a brand
that is everything is nothing) and optionally one secondary for nuance.

| Drive | Archetypes |
|---|---|
| Freedom / independence | Innocent, Explorer, Sage |
| Mastery / leaving a mark | Hero, Outlaw, Magician |
| Belonging / connection | Regular Guy/Gal (Everyperson), Lover, Jester |
| Structure / providing | Caregiver, Creator, Ruler |

The archetype is the *emotional spine*: an Explorer brand rewards discovery and the new; a
Caregiver brand reassures and protects; an Outlaw brand breaks the category's rules on
purpose. It quietly governs color energy, type feel, imagery, and tone.

**Aaker's five dimensions of brand personality** (Jennifer Aaker, *Journal of Marketing
Research*, 1997 — the canonical, validated brand-personality scale). Use these to pick
**three concrete adjectives** that *constrain* decisions:

- **Sincerity** — down-to-earth, honest, wholesome, cheerful
- **Excitement** — daring, spirited, imaginative, up-to-date
- **Competence** — reliable, intelligent, successful
- **Sophistication** — upper-class, charming, refined
- **Ruggedness** — outdoorsy, tough, strong

The test for the three adjectives: each must **exclude** something. "Trustworthy, modern,
clean" describes every product and constrains nothing. "Spirited, warm, a little
irreverent" rules out the cold and the corporate — now color and type have a job. Push the
user until their adjectives could not be swapped onto a competitor without it feeling wrong.

## Framework 2 — Differentiation: the onliness line

From Marty Neumeier (*The Brand Gap* / *Zag*): a brand is a person's gut feeling about a
product, and the engine of identity is **differentiation**. The litmus test is the
**onliness statement**:

> "Our [offering] is the **only** [category] that [benefit], for [who], in [context]."

If you cannot write it with the word *only* and keep it short, the brand has no edge for
the identity to dramatize — and the visual work will drift toward category defaults. The
onliness line is the brief behind the brief: a logo, a palette, and a type system all exist
to make that "only" feel inevitable at a glance. (If positioning was done via /positioning,
the onliness line may already exist — reuse it.)

## Framework 3 — Color: real, but not universal

Color carries personality, but **its meaning is contextual, not fixed.** This is the most
abused area of branding, so hold the evidence carefully:

- Labrecque & Milne (*Exciting red and competent blue*, 2012) show hue does map onto
  Aaker-style personality dimensions on average — e.g., blues skew "competent/trustworthy,"
  reds skew "exciting." So color *can* be chosen on purpose.
- **But** the same research and its successors show these effects are **moderated by
  context, product category, and culture.** Red means luck and celebration in much of
  China and danger or sale-urgency elsewhere. White reads as purity in one culture and
  mourning in another. There is no universal color dictionary — beware any source that
  hands you one.
- **Category norms and differentiation both matter.** Sometimes fitting the category color
  signals trust (fintech blues); sometimes breaking it is the whole point (a challenger
  brand going warm in a category of cold blues). Decide which move the onliness line calls
  for.

Practical stance: anchor color to *this* personality, *this* category, and *this* culture.
State the intended read, and flag explicitly where culture would change it. Never justify a
color with a one-size-fits-all "color psychology" claim.

## Framework 4 — Type and logo as carriers, not decoration

**Type is a voice.** A typeface communicates personality before a word is read — a humanist
serif feels editorial and warm; a geometric sans feels precise and modern; a monospace
feels technical and honest. Type choice is therefore a *personality* decision, not a taste
decision, and the same constraint applies: it must be derivable from the adjectives.

**A logo's job is to survive, not to dazzle.** The hard constraints are legibility at small
size (≈16px favicon), single-color reproduction, and fidelity to the personality. For solo
builders especially, a confident wordmark with one deliberate detail outperforms an
ambitious symbol that becomes a smudge. Ambition in a logo is a liability when there's no
brand-recognition budget to teach people what the abstract mark means.

## The anti-clichés (what a derived identity avoids)

Defaulting shows up as a recognizable set of tells. Flag these whenever they appear — not
because they are forbidden shapes, but because they are signs the identity was reached for
instead of reasoned to:

- The generic-AI-SaaS look: dark background, neon or purple-to-blue gradient, floating
  abstract 3D blobs — a costume worn by thousands of products that stand for nothing in
  particular.
- Decoration with no semantic job: geometric shapes, grid lines, and numbered section
  markers (01 / 02 / 03) used because the slot felt empty.
- A tiny all-caps tracked eyebrow above every section — one deliberate kicker is voice;
  eyebrows everywhere are filler.
- Cold, untinted gray as a base surface, when a faint tint toward the brand color would
  make every surface feel intentional.
- Adjectives that exclude nothing ("innovative, modern, trustworthy") standing in for a
  personality.
- Copy and naming that sound translated from English in a non-English market.

Each of these is a place where a real decision was skipped. The fix is always the same: go
back up the chain to the personality and the onliness line and decide on purpose.

## Accessibility is part of identity, not a later patch

A color nobody can read is not expressive, it's broken. Verify text contrast against its
background at **WCAG AA: 4.5:1 for body text, 3:1 for large text**, before any color ships.
Identity and accessibility are the same conversation: the brand only exists where people
can actually perceive it.

## The early-stage posture

Commit to the personality and the core color/type decisions — coherence is what makes a
small product feel trustworthy. But ship a tight one-page brand doc plus tokens rather than
an exhaustive bible, and treat it as living. The best brand refinements come from watching
how real users describe the product back to you.
