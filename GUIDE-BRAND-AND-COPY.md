# Guide: Brand and Copy Before You Code

> This guide is meant to be read inside Claude Code, or in any Markdown reader.
> Each module takes 20 to 60 minutes. You can stop and pick up where you left off.

---

## Why this guide exists

Most people treat brand and copy as the last step. Something to "make it look nice" once the product works.

That's backwards.

The words you use, the colors you choose and the tone you speak in aren't decoration. They're part of the product. They're the first thing someone judges, in the half second before reading a single sentence, and they decide whether that person understands what you built, feels it's for them, and stays.

This guide covers the layer between "I know what I'm building" and "I'm ready to write code." It's what makes your product *feel like something*, not just *do something*.

It comes after [product-discovery](https://github.com/ohanatais/product-discovery) (you already know who it's for and what sets you apart) and before [build-with-claude](https://github.com/ohanatais/build-with-claude) (time to build).

---

## What you'll learn

Three modules. The order matters: each builds on the one before.

| Module | Core question | Skill |
|---|---|---|
| [1. Brand identity](#module-1-brand-identity) | Who is this product, and what does it look like? | `/brand-identity` |
| [2. Tone of voice](#module-2-tone-of-voice) | How does this product talk, and how does it always sound like itself? | `/tone-of-voice` |
| [3. Product copy](#module-3-product-copy) | Which words make the right person feel this was made for them? | `/product-copy` |

Identity sets the visual container. Tone of voice sets the verbal personality. Copy is where both come alive in the moments that matter. Build in that order: copy written without a defined tone sounds like everyone else, and a tone defined without an identity has nothing to anchor to.

You don't need the skills to follow the guide. But they do the work with you, inside Claude Code, in whatever language you speak, deriving everything from *your* reality instead of a ready-made style.

---

## How to use this guide

**If you're starting from scratch:** follow the modules in order. Each has a reading (~10 min) and a practice (~20–40 min with the skill).

**If you're already midway:** jump to the module you're on. But if the copy feels generic downstream, the cause is almost always a step you skipped upstream, usually a poorly defined identity or tone.

**If you only want the skills:** each module has install and usage instructions. You don't need to read the whole guide.

One thing before you start: these skills are **universal by design**. The frameworks are fixed, but the output isn't. The same skill produces a warm, handwritten brand for one product and a hard, technical brand for another, because each one derives from *your* personality, category and culture. Nothing here pushes you toward a "right" style.

---

## Module 1: Brand identity

### What it is and why it matters

Brand identity isn't decoration you add at the end. It's the first decision your user makes about trusting you, made before reading a word.

You don't need an agency or a designer. You need clarity about what the product stands for, and a consistent visual system that communicates it when you're not in the room to explain.

The rule that governs everything: **derive, never default.** Every visual choice has to come from something the brand stands for. The moment the justification becomes "it looks nice" or "it's what modern products do," the choice has failed.

### The five components, always in order

Identity is built in a fixed sequence, where each piece depends on the previous one:

```
1. Personality    →  Who is the brand, if it were a person? (archetype + traits + the "only")
2. Color          →  A palette that expresses that personality on purpose, not by taste
3. Typography     →  Type as the brand's voice, before a single word is read
4. Logo           →  The simplest mark that survives at 16px and in one color
5. Documentation  →  The brand doc + tokens that make it all reproducible without you
```

Why the order is non-negotiable: a color is only "right" relative to a personality. Purple isn't premium or playful in the abstract; it depends on what the brand is trying to be. A logo with nothing above it is just a shape you happened to like.

### Personality: archetype + adjectives that constrain

Two research-based lenses, used together:

- **Archetype** (Mark & Pearson's 12, building on Jung): the dominant human drive the brand taps into. Pick **one** primary.
- **Three adjectives** anchored in Jennifer Aaker's five dimensions of brand personality (Sincerity, Excitement, Competence, Sophistication, Ruggedness). The test: each adjective has to **exclude** something. "Modern, clean, trustworthy" describes any product and constrains nothing. "Witty, warm, a little irreverent" rules out cold and corporate; now color and type have a job.

And the **onliness statement** (Neumeier): "the only [category] that [benefit]." If you can't write it with the word "only," the brand has no edge to dramatize.

### Color: real, but not universal

Color carries personality, but its meaning is contextual, not fixed. Research (Labrecque & Milne) shows that hues map to personality traits *on average*, but the effect is moderated by context, category and culture. Red means luck in China and danger elsewhere. There's no universal color dictionary; be suspicious of any source that hands you one.

### What to do now

```bash
# Copy it into your project
cp -r path/to/brand-and-copy/skills/brand-identity .claude/skills/

# In Claude Code:
/brand-identity
```

The skill has three modes: **guided** (from scratch, explaining each component), **brief** (you already have positioning and want the brief + tokens directly), and **audit** (you already have an identity and want an honest critique of coherence, clichés and accessibility).

**What you'll have at the end:** a personality statement (archetype + three adjectives + the onliness line), a color system named by role, a type system with your signature, a logo direction, and a brand doc + tokens: the deliverable that makes the brand reproducible without you.

---

## Module 2: Tone of voice

### What it is and why it matters

Tone of voice isn't about being funny or formal. It's about being **consistent**, and therefore recognizable.

A product that sounds witty on the landing page, robotic in onboarding and apologetic in error messages feels unfinished, even with flawless code. What people feel is the consistency: whether the page, the onboarding, the buttons and the errors sound like the same person. Inconsistency reads as sloppiness. A consistent voice, even a simple one, reads as a product that understands itself.

### Voice vs. tone: the distinction that holds everything up

- **Voice is constant.** It's the product's personality in words. It doesn't change between a celebration and an error. Voice answers: *who is speaking?*
- **Tone is variable.** It's how the voice adjusts to the moment: celebratory on a win, calm and direct on an error. Tone answers: *what does this moment need?*

A person has one voice and many tones: you're still you at a funeral and at a party, but you don't speak the same way. A product is the same. Define the voice once; map tones to contexts.

### The four dimensions (NN/g)

Nielsen Norman Group's research gives tone something "be friendly" doesn't have: a way to measure it. Any text sits somewhere on four scales:

1. **Funny ↔ Serious**
2. **Formal ↔ Casual**
3. **Respectful ↔ Irreverent**
4. **Enthusiastic ↔ Matter-of-fact**

This makes the voice repeatable ("casual, serious, respectful, matter-of-fact" is a setting someone else can hit) and has a measured effect on perceived friendliness, trustworthiness and desirability.

### "Say it three ways"

The most reliable way to make a voice *teachable*. For a real product message, write three versions: **on voice** (exactly right), **off voice** (a plausible version that breaks it: too harsh, too playful, too generic), and **on the edge** (almost right, but subtly wrong). The contrast is what makes the voice legible to anyone else, including Claude.

### What to do now

```bash
cp -r path/to/brand-and-copy/skills/tone-of-voice .claude/skills/

# In Claude Code:
/tone-of-voice
```

The skill has three modes: **guided** (define voice and tone from scratch), **chart** (you already have the personality and want the formal voice guide produced), and **audit** (you have copy and want to check whether it sounds like one product).

One thing the skill carries: the **lexicon and the banned list are always yours**. There's no universal list of "bad words," only words that break *this* voice. One product bans exclamation points; another lives on them.

**What you'll have at the end:** a voice definition (three adjectives + position on the four dimensions), a tone map by context, a lexicon (words it uses and words that break the voice), microcopy patterns (error, empty state, onboarding), "say it three ways" examples, and a voice doc, with an optional guardrail to keep things consistent when many hands (or AI) are writing.

---

## Module 3: Product copy

### What it is and why it matters

Copy isn't about sounding smart. It's about making the right person, at the right moment, feel this product was made for them.

Generic copy is invisible; the eye slides right off it. Specific copy converts, because it sounds like someone who knows something true about *that* person. The difference is almost never talent; it's method: knowing who's reading, how much they already know, what they actually want, and saying it in words they recognize.

### The five stages of awareness (Schwartz)

The most useful lens in copywriting, from *Breakthrough Advertising* (Eugene Schwartz, 1966). Before writing a word, place the reader:

1. **Unaware**: doesn't even know they have the problem. The job: name the problem.
2. **Problem-aware**: feels the problem, doesn't know there's a solution. The job: show you understand the problem precisely.
3. **Solution-aware**: knows solutions exist, is comparing. The job: your differentiation (the "only" from your positioning).
4. **Product-aware**: knows your product, isn't convinced yet. The job: proof, specificity, objections answered.
5. **Most aware**: ready, needs a nudge. The job: a clear offer and an easy next step.

The rule that prevents most mistakes: match the copy to where the reader *actually is*, which is almost always a stage or two earlier than the founder assumes. The founder is "most aware" about their own product; the visitor rarely is.

### The "so what?" ladder

A feature is what the product has. A benefit is what it does. *Meaning* is what it changes in the reader's life, and meaning is what converts. Walk every important claim down by asking "so what?" until you hit something the person actually feels:

- Feature: "exports to PDF"
- So what? → "share your work without sending the file"
- So what? → "look professional to your client in two clicks, nothing to install"

Ask "so what?" at least twice for every benefit.

### Mine, don't invent

The best copy is assembled, not authored. The words that convert usually already exist: in reviews, support tickets, sales calls, forum threads. Message mining means harvesting the phrases real people use to describe the problem and the relief, and putting those phrases in the copy. When you have any real customer language, use it before inventing.

### What to do now

```bash
cp -r path/to/brand-and-copy/skills/product-copy .claude/skills/

# In Claude Code:
/product-copy
```

The skill has three modes: **guided** (writes an asset from scratch, explaining the moves), **asset** (you know the message and the voice and want the copy produced), and **audit** (you have copy that isn't converting and want a diagnosis).

It **inherits** what you've already done: the positioning (the message) and the voice (from `/tone-of-voice`). Copy is the last layer, and it's strongest when it rests on the ones before.

**What you'll have at the end:** the reader + awareness stage call, the value proposition in one sentence, the copy written in the product's voice with each part labeled, the reasoning behind the key lines, objections answered, a clarity check (the 5-second test), and 2–3 headline/CTA variations to test.

---

## Next steps

With identity, voice and copy defined, the product has a face, talks like itself, and says the right thing to the right person.

What comes after this repository:

- **[build-with-claude](https://github.com/ohanatais/build-with-claude)**: Claude Code for non-technical builders, with every technical decision explained and step-by-step tool setup
- **[go-to-market](https://github.com/ohanatais/go-to-market)**: launch strategy, channels, first users

And, if you haven't been through it yet:

- **[product-discovery](https://github.com/ohanatais/product-discovery)**: market research, validation, personas, positioning, PRD (the layer that comes before this one)

---

*Made by [Ohana Taís](https://github.com/ohanatais), Senior PM, building in public.*
*Part of the [build-from-zero](https://github.com/ohanatais/build-from-zero) ecosystem.*
