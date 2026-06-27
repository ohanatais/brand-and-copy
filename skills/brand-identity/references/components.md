# Component Deep-Dives

The per-component method. Load this when a session reaches the depth of an actual
component. Every section ends with the same three *contrasting* illustrations so the method
is visible without implying one aesthetic is correct:

- **Brand A — "a warm cultural brand"** (Lover/Everyperson archetype; sincere, warm,
  spirited). A consumer product that wants to feel human and local.
- **Brand B — "a precise fintech"** (Ruler/Sage; competent, exact, trustworthy). A B2B
  tool where trust and clarity matter most.
- **Brand C — "a rugged outdoors brand"** (Explorer/Hero; tough, free, energetic). A
  product for the outdoors and the physical world.

These are invented to span the space. The user's brand is almost certainly none of them —
that's the point. Derive theirs.

## Contents
- [1. Personality](#1-personality)
- [2. Color](#2-color)
- [3. Typography](#3-typography)
- [4. Logo](#4-logo)
- [5. Documentation & tokens](#5-documentation--tokens)

---

## 1. Personality

**Goal:** a one-paragraph identity the rest of the system can be derived from.

**Method:**
1. Pull the strategy if it exists (positioning, personas, onliness line). If not, ask 2–3
   questions that surface the drive: "If this product were a person at a dinner party, who
   are they? What do they make people feel? What would they never do?"
2. Choose **one primary archetype** (see the 12 in `core-principles.md`). Optionally one
   secondary for nuance, never a third.
3. Choose **three adjectives** anchored in Aaker's five dimensions. Stress-test each: does
   it exclude something? Replace any that could describe any brand.
4. Write the **onliness line**: "the only ___ that ___, for ___."
5. Capture a **"north star" sentence** — the felt idea the whole identity serves (e.g., a
   single emotion or moment the brand is about). This becomes the tie-breaker for every
   later decision.

**Output:** archetype (primary [+ secondary]), three adjectives, onliness line, north-star
sentence. One paragraph.

| | Brand A (warm cultural) | Brand B (precise fintech) | Brand C (rugged outdoors) |
|---|---|---|---|
| Archetype | Lover + Everyperson | Ruler + Sage | Explorer + Hero |
| Adjectives | warm, spirited, unpretentious | exact, calm, authoritative | tough, free, plainspoken |
| North star | "the feeling of being truly seen" | "money you can finally understand" | "built for the trail, not the showroom" |

Notice the adjectives already pre-decide the next four components in different directions.

---

## 2. Color

**Goal:** a small, named palette that expresses the personality and passes contrast.

**Method:**
1. Translate each adjective into a chromatic direction (warmth/coolness, saturation,
   contrast level) — and write the *intended read* for each color. Anchor to personality,
   category, and culture; consult `core-principles.md` for the color-is-contextual caveat.
2. Decide the differentiation move: **fit** the category color (signals trust) or **break**
   it (signals challenger). Let the onliness line decide.
3. Build the minimal role set:
   - **One dominant brand color** — the color people will associate with the product.
   - **One accent** — used as *punctuation only*. Rarity is its power; if the accent covers
     more than ~10% of a screen it stops meaning "look here."
   - **Neutral base(s)** — backgrounds and text. Prefer bases faintly *tinted* toward the
     brand over dead gray, so every surface feels intentional.
   - **Semantic colors** — success, warning, error/destructive. These can borrow from the
     palette but must stay unambiguous.
4. **Name every color by role and meaning, not by hex or generic scale.** "brand-primary /
   trust-blue," not "blue-500." A named role tells the next person *when* to use it. (This
   is also how design tokens stay legible — see section 5.)
5. **Verify contrast** for every text-on-surface pair at WCAG AA (4.5:1 body, 3:1 large)
   before it ships. A beautiful color that fails contrast is not shippable.

**Output:** each color with name, value, role, intended read, and a contrast note.

| | Brand A | Brand B | Brand C |
|---|---|---|---|
| Move | break the category (warm, not corporate) | fit + refine (own a precise blue) | break (earthy, not neon-sporty) |
| Dominant | a deep saturated warm hue | a single exact, slightly cool blue | a deep forest or slate |
| Accent | a bright spark used sparingly | one restrained signal color | a high-vis safety orange, rationed |
| Base | warm off-white, never cold gray | near-white + one cool gray scale | stone / oat neutrals |

The method is identical; the outputs share nothing. That is the signal it's working.

---

## 3. Typography

**Goal:** type that sounds like the brand before a word is read.

**Method:**
1. Decide the **voice of the type** from the adjectives: editorial-warm (humanist serif),
   precise-modern (geometric/neo-grotesque sans), technical-honest (monospace influence),
   characterful (a display face with a quirk).
2. Choose **two families** in most cases — a **display/character** face for headlines and a
   **legible workhorse** for body — three at the absolute most. More than three reads as
   indecision.
3. **Pair for contrast with a reason** (serif display + sans body is a reliable contrast).
   The pairing should dramatize the personality, not just "look nice together."
4. Define one **signature move** the brand owns and repeats — a recognizable typographic
   gesture. Examples of the *kind* of move (not to copy): mixing weight or style within one
   headline; an oversized first line; a consistent tight tracking; a specific italic for
   emphasis. One move, used consistently, is what makes type *recognizable*.
5. Set a **hierarchy** (display / headline / title / body / label) with sizes, weights, and
   line-heights, and **check the smallest real size** — labels and captions on a phone, not
   just the hero. Body line-length ≈ 60–75 characters; line-height ≥ 1.5 for prose.

**Output:** families + pairing rationale, the signature move, and a hierarchy table.

| | Brand A | Brand B | Brand C |
|---|---|---|---|
| Display | a warm humanist serif with optical character | a precise grotesque, tight and even | a strong condensed or industrial sans |
| Body | a clean neutral sans | the same grotesque, lighter weight | a sturdy, legible sans |
| Signature | weight/italic mix inside one headline | numerals always tabular and aligned | all-caps headline with wide tracking |

---

## 4. Logo

**Goal:** the simplest mark that carries the personality and survives everywhere.

**Method:**
1. Start from the wordmark. For most solo builders, a **wordmark with one deliberate
   detail** is the right answer — it's recognizable on day one with no recognition budget.
   A purely abstract symbol asks the audience to *learn* a meaning you can't yet afford to
   teach.
2. The one detail should encode the personality or the onliness idea — a single letter
   modified, a ligature, a mark integrated into a character. One idea, executed cleanly.
3. **Hard tests, in order:**
   - Readable at **16px** (favicon) and in a single color (no gradient crutch).
   - Works on light *and* dark, and on a busy background.
   - Distinct from category competitors at a glance.
   - Still feels like the personality when stripped to one color.
4. Deliver a **direction** even if not final art: the concept, the rationale, and the
   construction notes. (If asked for actual art and tooling is available, generate an SVG;
   otherwise specify it precisely enough for a designer or an AI image tool to execute.)

**Output:** logo concept, why it fits the personality, and small-size/one-color notes.

| | Brand A | Brand B | Brand C |
|---|---|---|---|
| Direction | wordmark, one warm detail in a single glyph | exact wordmark, even spacing, a precise geometric monogram | sturdy wordmark, a simple iconic mark that works as a stamp |
| The detail | a diacritic or letter that becomes a small spark | a perfectly aligned dot or cut | a single bold geometric form |

---

## 5. Documentation & tokens

**Goal:** the artifact that makes the brand reproducible without the founder present. This
is the real deliverable — an identity that lives only in someone's head is a mood, not a
brand.

**Method:**
1. Write a **brand doc** (e.g. `DESIGN.md` or `brand.md`) with: the personality paragraph,
   the palette (each color named, with role + value + intended read), the type system
   (families, hierarchy, the signature move), logo usage, and an explicit **do / don't**
   list. The do/don't list is where the anti-clichés get named for *this* brand.
2. Produce **design tokens** — machine-usable values a developer or Claude applies directly:
   color (by role name), typography (families, sizes, weights, line-heights), spacing scale,
   radius, and elevation. Tokens are what let the brand show up consistently in real code.
3. Write a few **"rules with names"** — short, memorable constraints that travel. The point
   of naming a rule ("the accent is punctuation: never more than ~10% of a screen") is that
   people remember and apply named rules; they ignore buried prose.
4. Keep it **one page of doc + one block of tokens** at early stage. Depth is earned by
   usage, not front-loaded.

**Output:** offer to write the brand doc and tokens to files in the user's project. Tokens
should be usable as-is (CSS custom properties, a Tailwind/shadcn theme, or a JSON token set
— match the user's stack if known).

A minimal token shape (adapt names and values to the brand):

```
colors:    brand-primary, accent, base, surface, text, text-muted, border, success, error
type:      display (family/size/weight/lh), body (...), label (...)
spacing:   xs sm md lg xl  (a consistent scale)
radius:    sm md lg  (one grammar, e.g. interactive vs container)
```

Naming colors by *role* (not `blue-500`) is what keeps tokens legible: the next person
reads "accent" and knows it's for punctuation, reads "error" and knows it's destructive —
no guessing. The values differ wildly across Brand A, B, and C; the *role structure* is the
same, which is exactly why it's a reusable system rather than a one-off palette.
