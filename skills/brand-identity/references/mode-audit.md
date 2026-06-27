# Mode: Audit

For a user who already has an identity — some colors, a logo, fonts in use — and wants it
**pressure-tested** before they commit further or launch. Diagnose before you redesign. The
goal is an honest verdict plus a prioritized fix list, not a reflexive from-scratch redo.

Load `references/core-principles.md` and `references/components.md` alongside this file.

## Posture

Resist the urge to replace what exists with your own taste. The user may have something
that's 80% right with two real problems; throwing it out would be a disservice. Find what's
working and protect it; isolate what's broken and explain *why* in terms of the brand's own
strategy. Critique the identity against the personality it claims — not against a house
style.

## What to check, in order

**1. Coherence with strategy.** Does the identity express the personality and the onliness
line? Ask the user (or infer) the archetype and three adjectives, then test each visual
choice against them. The most common real problem isn't ugliness — it's an identity that
contradicts what the brand is trying to be (a "warm, human" brand rendered in cold corporate
blues).

**2. The anti-clichés.** Run the list from `core-principles.md`. Flag the generic-AI-SaaS
look, decoration with no semantic job, eyebrows on every section, cold-gray bases, and
adjectives that exclude nothing. For each, name *why* it signals defaulting and what
deriving from the personality would do instead.

**3. Color discipline.** Is there a clear dominant and a rationed accent, or is everything
shouting at once? Are colors named by role or floating as random hexes? **Run contrast on
every text/surface pair** — failures here are blocking, not cosmetic.

**4. Type discipline.** More than three families? No signature move (forgettable) or an
over-applied one (exhausting)? Does it hold up at the smallest real size? Does the type's
voice match the personality?

**5. Logo survival.** Test at 16px and in one color. Does it read? Is it distinct from
category competitors? Does it still feel like the personality when stripped down?

**6. Reproducibility.** Is there a brand doc and a token set, or does the identity live only
in the founder's memory and a few Figma frames? An undocumented identity will drift the
moment a second person (or Claude) touches the product.

## Output

1. **Verdict** — one honest line: solid and ship-ready, solid-with-fixes, or needs rework
   at the personality level. Lead with it.
2. **What's working** — name it explicitly so it's protected through the changes.
3. **Findings by severity** —
   - **Blocking**: contrast failures, an identity that contradicts the strategy, illegible
     logo. Fix before launch.
   - **Should-fix**: clichés, undisciplined color/type, no documentation.
   - **Polish**: smaller refinements.
   For each: the problem, *why* it matters in this brand's terms, and the concrete fix.
4. **Prioritized fix list** — ordered, so a solo builder knows what to do first.
5. **Next step** — if the audit surfaces a personality-level contradiction, route to a
   short **guided** pass on the affected components; otherwise hand off to `/tone-of-voice`
   to align the verbal identity with the now-validated visual one.
