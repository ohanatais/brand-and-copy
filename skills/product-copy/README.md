# product-copy

> Copy isn't about sounding smart. It's about making the right person, in the right moment, feel like this product was made for them. Generic copy is invisible. Specific copy converts.

Part of the [brand-and-copy](https://github.com/ohanatais/brand-and-copy) skill set, within the [build-from-zero](https://github.com/ohanatais/build-from-zero) ecosystem.

---

## What this skill does

Writes the product copy that does real work — landing pages, onboarding, emails, and the words in between — by matching the right message to the right reader at the right moment, in the product's own voice. It produces the copy **and the reasoning behind every line**, so the founder can keep writing it themselves.

It's grounded in copywriting evidence rather than swipe files: Eugene Schwartz's five stages of awareness, jobs-to-be-done, voice-of-customer / message mining, and the features-to-benefits-to-meaning ladder.

The skill is **universal by design**: the same method writes a calm, technical page for a security tool and a loud, playful one for a party game — because each is derived from *that* reader, *that* job, and *that* voice. Examples in the references show how to decide; they're never phrases to reuse.

---

## What it inherits

Copy is the last layer, strongest when it stands on:
- **Positioning / personas** ([`/positioning`](https://github.com/ohanatais/product-discovery)) — the message: who it's for, what's different
- **Voice** ([`tone-of-voice`](../tone-of-voice)) — how it should sound

It can derive working versions if those are missing, but it'll name the gap — copy over an undefined message converts worse.

---

## The model: five layers, in order

```
1. Reader & moment   →  Who's reading, and how aware are they? (Schwartz's 5 stages)
2. Message           →  The value proposition: one sentence that means something
3. Structure         →  The anatomy of the asset (landing / onboarding / email)
4. Craft             →  Lines that work: specific, benefit-with-meaning, in the reader's words
5. Proof & CTA       →  Earning belief and a CTA that feels inevitable
```

You can't choose a headline before you know how aware the reader is — the same product needs a different first line for someone who doesn't know they have the problem versus someone comparing you to a competitor.

---

## Three modes, one interface

| Mode | When to use | Output |
|---|---|---|
| **guided** | Writing a key asset for the first time, wants to learn the moves | Section-by-section build with the reasoning |
| **asset** | Knows message and voice, wants the copy produced | A full asset, drafted in voice, ready to test |
| **audit** | Has copy that isn't landing, wants it diagnosed | Verdict + findings by impact + prioritized rewrites |

---

## What every output includes

- **Reader & awareness call** — who's reading and which stage
- **The value proposition** — the one-sentence message + the job it serves
- **The copy** — drafted in the product's voice, with each part labeled
- **The reasoning** — why the key lines are built that way
- **Proof & objections handled** — claims backed, hesitations answered
- **A clarity check** — the 5-second test + the "so what" pass
- **Variations & next step** — headlines/CTAs to test, then ship or `/go-to-market`

---

## How to install

```bash
cp -r product-copy /your-project/.claude/skills/
```

---

## How to trigger

In Claude Code, the skill activates when relevant, or invoke it directly:

```
/product-copy
```

It also triggers on natural phrasing — "write my landing page", "I need a headline", "what's my value proposition", "my copy isn't converting", "write onboarding copy", "write a launch email" — even without the word "copy".

---

## The relationship to the rest

Product copy is where the **visual identity** ([`brand-identity`](../brand-identity)) and the **voice** ([`tone-of-voice`](../tone-of-voice)) come alive in the moments that matter — the landing page, the first email, the first error. Build them in that order: copy written without a defined identity and voice sounds like everyone else.

---

Made by [Ohana Taís](https://github.com/ohanatais) · part of [build-from-zero](https://github.com/ohanatais/build-from-zero)
