# Mode: Chart

For a user who already has a personality (from `/brand-identity` or `/positioning`) and
wants the **voice chart, lexicon, and guardrail produced efficiently** — the formal,
reusable voice guide, not a teaching walk.

Load `references/core-principles.md` and `references/components.md` alongside this file.

## Posture

Respect the upstream thinking. Pull the archetype and adjectives and treat them as the source
of truth, then make confident, reasoned proposals across all five layers in one pass. The
deliverable is the voice doc + (optionally) the consistency check, ready to drop into the
project and use immediately — by the user, teammates, or Claude.

## The flow (one pass, then refine)

1. **Translate personality into voice.** State the three "how it writes" adjectives and the
   default NN/g four-dimension setting, derived from the brand personality. If the personality
   doesn't yet imply a crisp voice, propose one and flag it — this is the one place worth a
   beat of friction.
2. **Build the voice chart** (Podmajersky columns): Concepts, Vocabulary, Verbosity, Grammar,
   Punctuation & capitalization. This is the heart of the deliverable — it's what makes the
   voice applicable line by line.
3. **Map tone** across the product's recurring contexts (emotional axis first).
4. **Write the lexicon** — use/avoid with swaps, the banned list made specific to this
   product.
5. **Produce microcopy patterns** and **3–4 "say it three ways"** examples in the product's
   real language.
6. **Assemble the voice doc**; offer to write it to a file matching their setup. If copy will
   be generated at scale or by AI, build the consistency check (named voice-breakers + golden
   examples) per `components.md`.

Present the voice as one coherent whole so the user reacts to a *voice*, not a pile of
isolated rules.

## Where to slow down

Even fast: keep the three adjectives sharp (exclude something), make the banned list the
user's own rather than a generic anti-AI list, and ground every example in their real
product nouns and language.

## Close

Deliver the full output set, write the files, and hand off to `/product-copy`. Flag anything
held as hypothesis to revisit once real copy ships and users react.
