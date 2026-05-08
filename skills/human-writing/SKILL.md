---
name: human-writing
description: >
  Write text that reads as authentically human rather than AI-generated. Use this skill for ANY
  writing task where the output must not sound like it came from an AI: blog posts, emails, essays,
  articles, creative writing, marketing copy, social media posts, reports, documentation, cover letters,
  bios, product descriptions, or any content that will be read by humans who might notice or care
  about AI tells. Also trigger when the user says things like "make it sound human", "write naturally",
  "don't sound like AI", "avoid AI slop", "humanize this", or "write like a real person". This skill
  should be used even when the user just asks for writing and doesn't mention AI at all, if the context
  suggests the output will be published, shared, or evaluated by humans.
---

# Human Writing Skill

Write like a person, not a language model. This skill is built from peer-reviewed research
(UCC stylometry study, Dec 2025; Carnegie Mellon detection analysis, 2025; Kujur comparative
linguistics study, SSRN Nov 2025), Wikipedia's "Signs of AI Writing" editorial guide, the
Max Planck Institute vocabulary frequency analysis, Buffer's 52M-post corpus analysis, and
the 2026 arxiv paper "The Last Fingerprint: How Markdown Training Shapes LLM Prose."

The core finding across all of this research is that AI detection operates on three axes:
**perplexity** (word-level predictability), **burstiness** (sentence-level variation), and
**stylometric fingerprinting** (vocabulary and structural patterns). Human text scores higher
on the first two and is far more varied on the third. This skill addresses all three.

---

## HOW TO USE THIS SKILL

Before writing anything, read this file completely. Then read `references/banned-vocabulary.md`
for the full word/phrase avoidance list. Apply every rule below to all output. After drafting,
do a self-audit pass (Section 7) before delivering to the user.

---

## 1. VOCABULARY RULES

AI models converge on a small rotation of "impressive-sounding" words that now function as
statistical fingerprints. The Max Planck Institute found that words like "delve," "underscore,"
and "pivotal" spiked 50%+ in published text after ChatGPT launched. Wikipedia editors maintain
a living list of AI vocabulary grouped by model era.

### 1.1 Banned words (never use these)

The full list is in `references/banned-vocabulary.md`. The worst offenders, which must never
appear in output regardless of context:

delve, tapestry, testament, landscape (figurative), vibrant, pivotal, multifaceted, nuanced
(as filler), robust, seamless, cutting-edge, groundbreaking, game-changer, paradigm shift,
holistic, synergy, leverage (verb), foster, facilitate, utilize (use "use"), underscore,
spearhead, embark, unpack, unravel, craft (verb, when meaning "write" or "make"),
comprehensive, invaluable, endeavor, realm, intricate, meticulous, plethora, myriad (noun),
paramount, resonate, streamline, elevate, empower, unlock, unleash, harness

### 1.2 Banned phrases (never use these)

"In today's [adjective] [landscape/world/era]", "It's worth noting that", "It's important
to note", "Let's dive in", "Let's delve into", "At the end of the day", "Not just X, but Y"
(the false-contrast pattern), "In the realm of", "A testament to", "Serves as a reminder",
"It cannot be overstated", "This is where X comes in", "When it comes to", "The question
is not whether but how", "As we navigate", "In an era of", "The landscape of", "Moving
forward", "Going forward", "On the journey to", "In the ever-evolving world of",
"Here's the thing", "The reality is", "The truth is", "Make no mistake"

### 1.3 Banned openers (never start a sentence or paragraph with these)

Certainly, Moreover, Furthermore, Additionally, Indeed, Notably, Importantly, Interestingly,
Remarkably, Ultimately, Fundamentally, Essentially, Undoubtedly, Consequently, Subsequently,
Accordingly

### 1.4 What to use instead

Use plain, specific language. Prefer short Anglo-Saxon words over long Latinate ones.
"Use" not "utilize." "Help" not "facilitate." "Start" not "embark on." "Show" not
"showcase." "Important" not "paramount." If a word sounds like it belongs in a TED talk
or a LinkedIn post, pick a different one.

When you need transitions, use the ones actual humans use: "But", "And", "So", "Still",
"Then", "Also", "Plus", "Though", "Anyway", "That said", "Meanwhile", "Look",
"The thing is", "Here's what happened", "What I mean is".

---

## 2. SENTENCE STRUCTURE AND RHYTHM (BURSTINESS)

This is the single strongest detection signal. Research from ProofreaderPro.ai (analyzing
200 academic samples) found burstiness was more reliable than vocabulary analysis alone
for separating human from AI text.

AI text has a characteristic "metronomic" quality: sentences cluster in a narrow 15-20 word
range with similar grammatical structures. Human writing has wild variation.

### 2.1 Rules

- Vary sentence length deliberately. Mix 3-word sentences with 30-word sentences. After
  two medium-length sentences, throw in something very short. Or very long.
- Never write three or more consecutive sentences of similar length (+/- 5 words).
- Never write three or more consecutive sentences with the same grammatical structure
  (e.g., Subject-Verb-Object, Subject-Verb-Object, Subject-Verb-Object).
- Use fragments. Intentionally. Like this one.
- Use run-on-ish sentences joined with "and" sometimes, the way people actually talk when
  they get going on something and don't want to stop.
- Start some sentences with conjunctions (And, But, So, Or). English teachers used to
  say not to. They were wrong, and every good writer does it.
- Interrupt yourself with parenthetical asides (like this) or mid-sentence pivots.

### 2.2 Self-test

After drafting, count the words in each sentence for two consecutive paragraphs.
If the standard deviation is below 5, rewrite. Aim for a standard deviation of 8+.
The sequence should look jagged, not flat: something like 6, 22, 4, 31, 12, 8, 19.

---

## 3. STRUCTURAL PATTERNS TO AVOID

### 3.1 The Rule of Three

AI loves triplets: "adjective, adjective, and adjective" or "phrase, phrase, and phrase."
Wikipedia editors flag this constantly. Use pairs, or lists of four, or just one thing.
When three items genuinely belong together, fine. But question every triplet: is that
third item adding meaning or just filling out the rhythm?

### 3.2 The Hedging Seesaw

"While X is true, Y is also important." "On one hand... on the other hand..." AI uses
this pattern to sound balanced without committing to anything. Pick a side. State your
point. If the counterpoint matters, give it its own sentence with its own weight.

### 3.3 The Corporate Pep Talk

Inflating importance with value language: "This represents a significant advancement"
or "a powerful approach that enables teams to..." Strip the adjectives. Say what the
thing actually does in concrete terms.

### 3.4 False Agency / Inanimate Subjects

"The data reveals", "The analysis demonstrates", "The market rewards", "This approach
enables." AI gives human verbs to non-human things to avoid naming actual people. Name
the human. "We found" not "The analysis reveals." "Customers prefer" not "The market
rewards." Who did the thing? Say who.

### 3.5 Passive Voice Clusters

One passive sentence is fine. Three in a row reads like a government report written by
no one in particular. Default to active voice. Use passive only when who-did-it genuinely
doesn't matter or is unknown.

### 3.6 The Sycophantic Opener

Never start with "Great question!" or "That's a really interesting point!" or "Absolutely!"
Jump straight to the substance.

### 3.7 The Summary-Conclusion Pattern

AI loves to end with a paragraph that restates everything it just said, starting with
"In conclusion" or "In summary" or "Ultimately." Don't do this. End with your last real
point. Let the reader feel the piece is done without being told it's done.

---

## 4. PUNCTUATION AND FORMATTING

### 4.1 Em dashes

Target: zero. Hard maximum: one per 1,000 words. This is the single most discussed
AI punctuation tell. A 2026 arxiv paper demonstrated that em dashes are "markdown leaking
into prose" — the smallest surviving unit of structural formatting that LLMs absorb from
their training data. Replace with commas, periods, parentheses, or restructure the sentence.

### 4.2 Semicolons

Use sparingly. One per 500 words maximum. Most humans rarely use semicolons outside
academic writing.

### 4.3 Exclamation marks

Maximum one per piece unless the tone genuinely calls for more. AI uses them for false
enthusiasm.

### 4.4 Ellipsis

Almost never. It reads as dramatic AI trailing off...

### 4.5 Formatting

- Do not use bold for emphasis in running prose unless the user specifically requests it.
- Do not use headers in short pieces (under 500 words) unless the user asks for structure.
- Do not use bullet points where prose would work. Bullets are for genuinely list-like
  content (steps, specs, feature comparisons). Everything else should be sentences.
- Never put emoji in headers or bullet points.
- Never produce "**Bold header:** description text" list patterns. This is the most
  recognizable AI formatting pattern of all. If you need a list, use plain bullets.
  If you need headers, use actual headers.

### 4.6 Markdown leakage

If writing plain text (emails, social posts, bios), never let markdown syntax through.
No asterisks for emphasis, no hashtags for headers, no backticks. Write in the format
the output will actually be read in.

---

## 5. CONTENT AND REASONING PATTERNS

### 5.1 Specificity over abstraction

AI defaults to abstract claims. Humans use specific examples, numbers, names, places,
and dates. Instead of "many companies have adopted this approach," say "Stripe started
doing this in 2019." Instead of "this can improve productivity," say "it cut our
deployment time from 3 hours to 20 minutes."

### 5.2 Imperfection and informality

Humans aren't polished. They:
- Use contractions (don't, can't, it's, wouldn't, I've, they're)
- Start sentences with "I" or "We"
- Express uncertainty naturally ("I think", "probably", "not sure but", "from what I can tell")
- Have opinions and state them directly
- Use colloquial phrasing ("kind of", "sort of", "pretty much", "a lot", "way more")
- Occasionally use informal punctuation (a dash here, a parenthetical aside there)
- Reference personal experience or observation

### 5.3 No invented evidence

Never fabricate statistics, studies, quotes, or anecdotes to make a point seem more
credible. This is an accuracy failure, not a style issue. If you don't have a real
number, don't make one up. Say "I don't have exact figures" or just omit the claim.

### 5.4 Emotional honesty

When something is boring, you can say it's boring. When something is hard, say so.
AI text maintains relentless upbeat neutrality. Human text has texture: doubt, frustration,
excitement, boredom, humor, annoyance. Match the emotional register to the actual content.

---

## 6. TONE CALIBRATION

### 6.1 Match the register to the context

- Casual (social media, Slack, texts): Short. Loose grammar. Contractions. Sentence
  fragments. Personality.
- Professional (emails, reports): Clear and direct. Still use contractions. Avoid jargon
  unless the audience expects it. No buzzwords.
- Formal (academic, legal, policy): Longer sentences allowed. Technical vocabulary
  expected. Still vary rhythm. Still avoid the banned vocabulary.
- Creative (stories, essays, blogs): Maximum freedom. Break rules intentionally. Let
  voice emerge.

### 6.2 Don't over-explain

AI hedges and qualifies everything because it's trained to be safe. Humans state things
and move on. "The best way to learn guitar is to play every day" not "While there are
many approaches to learning guitar, and individual results may vary, many experts suggest
that consistent daily practice is often considered one of the most effective strategies."

---

## 7. SELF-AUDIT CHECKLIST

Before delivering any written output, run through these checks:

1. **Vocabulary scan**: Search your output for any word from the banned list. Replace all.
2. **Opener check**: Does any paragraph start with a banned opener? Fix it.
3. **Burstiness check**: Pick any two consecutive paragraphs. Eyeball the sentence lengths.
   Do they vary enough? If three sentences in a row are similar length, rewrite one.
4. **Triplet check**: Find every list of exactly three things. Is the third one earning
   its place, or just filling out a pattern? Cut it or add a fourth.
5. **Em dash count**: Are there any? Remove or replace.
6. **Formatting check**: Did you use bold-colon list patterns? Unnecessary headers?
   Bullet points where prose would work? Fix it.
7. **False agency check**: Did you give human verbs to inanimate subjects? Name the human.
8. **Abstraction check**: Is there a claim without a concrete example or specific detail?
   Add one or cut the claim.
9. **Read it aloud**: Does it sound like something a person would actually say? If any
   sentence sounds like it came from a press release or a LinkedIn post, rewrite it.
10. **Final gut check**: Would a Wikipedia editor flag this? Would a colleague reading this
    in an email think "this sounds AI-generated"? If yes, find the tell and fix it.

---

## 8. EXAMPLES

### Bad (AI-typical):

"In today's rapidly evolving digital landscape, content creation has undergone a
transformative shift. AI-powered tools have emerged as game-changers, enabling creators to
streamline their workflows and unlock new levels of productivity. However, it's worth noting
that the human touch remains paramount. By leveraging these innovative technologies while
fostering authentic creativity, content creators can navigate the complexities of modern
media and deliver truly impactful results."

Problems: Uses 7 banned words/phrases, metronomic sentence length (12, 11, 11, 19 words),
opens with a banned phrase, hedging seesaw, corporate pep talk tone, zero specificity.

### Good (human):

"Most writing advice about AI boils down to 'use it but add your voice,' which is about
as helpful as telling someone to 'just be yourself' at a party. What actually works is
more boring. Write shorter. Cut the adjectives. Say who did what. I've been editing AI
drafts for a year and the biggest tell isn't any single word. It's the rhythm. Every
sentence the same length, the same structure. Real writing lurches around. A sentence runs
long and then you stop. Like that."

Why it works: Sentence lengths vary wildly (19, 17, 4, 5, 5, 19, 9, 8, 5, 3), uses
personal experience, has an opinion, informal register, no banned vocabulary, no em dashes,
specific observation, ends abruptly.

---

## IMPORTANT CAVEATS

- These rules are about default behavior. If the user asks for formal academic writing,
  some formality is appropriate. If they ask for marketing copy, some energy is expected.
  Calibrate to the genre, but even within formal genres, burstiness and vocabulary
  freshness matter.
- These rules don't apply to technical writing where precision requires specific terms.
  "Robust" in engineering means something real. "Leverage" in finance is a real concept.
  Context matters.
- Not every short piece needs every rule. For a 50-word product description, focus on
  vocabulary and specificity. For a 2,000-word article, every rule applies.
- The goal is not to sound stupid or sloppy. The goal is to sound like a specific human
  who has thoughts and says them clearly.
