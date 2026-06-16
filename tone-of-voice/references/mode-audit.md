# Mode: Audit

For a user who has copy already — a landing page, emails, in-product strings — and wants to
know whether it **sounds like one product**. Diagnose drift; don't rewrite everything by
reflex. The output is an honest read plus the specific places the voice breaks and how to
fix them.

Load `references/core-principles.md` and `references/components.md` alongside this file.

## Posture

The most common real problem isn't bad writing — it's *inconsistency*: copy that's witty on
the landing page, robotic in onboarding, and cold at errors. Find the surfaces that already
sound right and treat them as the reference; isolate the ones that drift and explain *why* in
terms of the product's own voice. If no voice is defined yet, infer the intended one from the
strongest existing copy and check the rest against it.

## What to check, in order

**1. Establish the target.** Pull the defined voice (adjectives + four-dimension setting) or
infer it from the best existing copy. Everything is measured against this, not against taste.

**2. Consistency across surfaces.** Sample real strings from each surface — landing, emails,
onboarding, empty states, errors, buttons. Place each on the four dimensions. Drift shows up
as the same product landing in different places on the scales. Name where and how.

**3. The emotional moments.** Check errors, empty states, and destructive confirmations
specifically — voice is dropped here most. Flag cold "Invalid"/"Something went wrong" strings,
joke-in-the-wrong-place tone mismatches, and user-blaming language.

**4. The lexicon.** Is naming consistent (the same object called one thing, not three)? Run
the anti-tells from `core-principles.md` as a starting checklist — translated-from-English
phrasing, hype adverbs, buzzword filler, exclamation inflation — and flag instances, framed
as "does this match your voice?" not "this is objectively wrong."

**5. Reproducibility.** Is there a voice doc, or does the voice live only in the founder's
ear? Undocumented voice will keep drifting, especially once a second writer or an AI touches
the copy.

## Output

1. **Verdict** — one honest line: sounds like one product, mostly-consistent-with-drift, or
   no coherent voice yet. Lead with it.
2. **What's working** — the surfaces that already nail it, named so they're protected and
   used as the reference.
3. **Drift findings, by surface** — for each problem: the string, where it sits on the
   dimensions vs. the target, *why* it breaks the voice, and an on-voice rewrite.
4. **Priority fixes** — ordered; the emotional-moment microcopy usually ranks high because it
   carries the most weight per word.
5. **Next step** — if there's no defined voice, route to a short **guided** or **chart** pass
   to lock it; then offer the consistency check so the fixed voice stays fixed. Hand off to
   `/product-copy` for any surface that needs rewriting from scratch, not just tuning.
