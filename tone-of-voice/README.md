# tone-of-voice

> Tone of voice isn't about being funny or formal. It's about being consistent — so the landing page, the onboarding, and the error messages all sound like the same product wrote them.

Part of the [brand-and-copy](https://github.com/ohanatais/brand-and-copy) skill set, within the [build-from-zero](https://github.com/ohanatais/build-from-zero) ecosystem.

---

## What this skill does

Defines a product's **voice** (who it is in words — constant) and **tone** (how that voice flexes by context — variable), then turns both into something reusable: a lexicon, microcopy patterns, and an optional guardrail. The result is a product that sounds like itself everywhere, without the founder hand-editing every string.

It's grounded in content-design evidence rather than vibes: Nielsen Norman Group's four tone dimensions, the voice-vs-tone distinction, and Podmajersky's Voice Chart.

The skill is **universal by design**: the same method produces a dry, precise voice for a compliance tool and a warm, irreverent one for a hobby app — because each is derived from *that* product's personality, audience, and language. The lexicon and the banned list are always the user's own; there's no universal list of "bad words," only words that break *this* voice.

---

## The model: five layers, in order

```
1. Voice      →  Who is this product, in words? (the brand personality, made verbal)
2. Tone       →  How that voice flexes across contexts and emotional states
3. Lexicon    →  The words it uses — and the words that break it
4. Microcopy  →  Voice applied to errors, empty states, onboarding, buttons
5. Guardrail  →  The voice doc + an optional check that keeps it consistent at scale
```

Voice comes first because tone is a modulation of it. Microcopy gets its own layer because it's where voice is most often dropped — and most felt.

---

## Three modes, one interface

| Mode | When to use | Output |
|---|---|---|
| **guided** | Defining voice and tone for the first time | Step-by-step through the five layers, explaining the why |
| **chart** | Has the personality, wants the formal voice guide produced | Voice chart + lexicon + microcopy + guardrail |
| **audit** | Has copy, wants it checked for consistency | Verdict + drift findings by surface + on-voice rewrites |

---

## What every output includes

- **Voice definition** — three constraining adjectives + position on NN/g's four dimensions + one paragraph
- **Tone map** — how the voice flexes across recurring contexts (success, error, empty, confused)
- **Lexicon** — words to use, and a named list of words that break the voice
- **Microcopy patterns** — on-voice errors, empty states, onboarding, buttons
- **"Say it three ways" examples** — on voice / off voice / on the edge, in the product's real language
- **Voice doc + optional guardrail** — the reproducible deliverable
- **Next step** — usually `/product-copy`

---

## How to install

```bash
cp -r tone-of-voice /your-project/.claude/skills/
```

---

## How to trigger

In Claude Code, the skill activates when relevant, or invoke it directly:

```
/tone-of-voice
```

It also triggers on natural phrasing — "define our voice", "our copy sounds inconsistent", "the app sounds like a robot", "write error messages that aren't cold", "make it sound more like us" — even without the words "tone of voice".

---

## The relationship to the rest

Tone of voice is the **verbal** half of how a product feels; its visual twin is [`brand-identity`](../brand-identity). Both come alive in [`product-copy`](../product-copy), which inherits this voice to write the words that convert. Voice is the *system*; product copy is one *output* of it.

---

Made by [Ohana Taís](https://github.com/ohanatais) · part of [build-from-zero](https://github.com/ohanatais/build-from-zero)
