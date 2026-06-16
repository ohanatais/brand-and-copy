# brand-identity

> Your brand isn't decoration you add at the end. It's the first decision your user makes about whether to trust you — made in the half-second before they read a single word.

Part of the [brand-and-copy](https://github.com/ohanatais/brand-and-copy) skill set, within the [build-from-zero](https://github.com/ohanatais/build-from-zero) ecosystem.

---

## What this skill does

Creates a coherent visual and verbal brand identity for a solo builder or small team — **without a designer** — by deriving every choice from what the brand actually stands for, not from taste or trend. It produces a brand brief and a set of design tokens: a system someone (a designer, a developer, Claude, or future-you) can apply consistently when you're not there to explain it.

It's grounded in brand-strategy evidence rather than vibes: Aaker's five personality dimensions, Mark & Pearson's 12 archetypes, Neumeier's onliness/differentiation, and color research showing that color meaning is contextual, not universal.

The skill is **universal by design**: the same method produces a warm, hand-drawn identity for one product and a stark, technical one for the next — because each is derived from *that* product's personality, category, and culture. Examples in the references are illustrations of how to decide, never a house style to copy.

---

## The model: five components, always in order

```
1. Personality   →  Who is this brand, as a person? (archetype + traits + the "only")
2. Color         →  A palette that expresses that personality on purpose
3. Typography    →  Type as the brand's voice, before a word is read
4. Logo          →  The simplest mark that survives at 16px and one color
5. Documentation →  The brand doc + tokens that make it reproducible without you
```

The order is non-negotiable: each component is derived from the one above it. Color is only "right" relative to a personality; a logo with nothing above it is just a shape you happen to like.

---

## Three modes, one interface

| Mode | When to use | Output |
|---|---|---|
| **guided** | Building identity from scratch, or doing it deliberately for the first time | Step-by-step through all five components, explaining the why |
| **brief** | Has positioning/personas, wants the brand brief + tokens produced efficiently | A full coherent identity proposal + brand doc + tokens |
| **audit** | Has an identity, wants it pressure-tested before committing | Verdict + findings by severity + prioritized fix list |

---

## What every output includes

- **Personality statement** — primary archetype + three constraining adjectives + the onliness line
- **Color system** — each color named by role, with rationale and a contrast note
- **Type system** — families, pairing rationale, hierarchy, and the signature move
- **Logo direction** — the concept and why it fits (final art optional)
- **Brand documentation + tokens** — the reproducible deliverable
- **What this identity rules out** — the anti-patterns and clichés this brand won't use
- **Open questions & next step** — usually `/tone-of-voice`, then `/product-copy`

---

## How to install

```bash
cp -r brand-identity /your-project/.claude/skills/
```

---

## How to trigger

In Claude Code, the skill activates when relevant, or invoke it directly:

```
/brand-identity
```

It also triggers on natural phrasing — "I need a brand", "help me choose a palette", "pick fonts for my product", "design a logo", "my product looks like every other AI app", "write brand guidelines" — even without the words "brand identity".

---

## The relationship to the rest

Brand identity is the **visual** half of how a product feels. Its verbal twin is [`tone-of-voice`](../tone-of-voice) (how the product *talks*), and both come alive in [`product-copy`](../product-copy) (the words that convert). Build them in that order — copy written without a defined identity and voice sounds like everyone else.

---

Made by [Ohana Taís](https://github.com/ohanatais) · part of [build-from-zero](https://github.com/ohanatais/build-from-zero)
