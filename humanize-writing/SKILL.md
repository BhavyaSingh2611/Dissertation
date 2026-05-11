---
name: humanize-writing
description: >
  Rewrites AI-generated or robotic-sounding text so it reads as authentically human — passing AI detectors like GPTZero, Turnitin, ZeroGPT, Copyleaks, and Originality.ai. Use this skill whenever the user wants to: humanize text, make writing sound more natural or less robotic, bypass or pass AI detectors, rewrite AI-generated content, improve writing authenticity, add a human voice to content, or avoid detection. Trigger this skill even if the user says things like "make this sound like me", "make this less AI", "this sounds too formal/robotic", "can you make this pass GPTZero", or "rewrite this so it sounds human". This skill applies to essays, articles, emails, blog posts, cover letters, reports, and any other written content.
---

# Humanize Writing Skill

Transforms AI-generated or robotic text into authentic, human-sounding writing that bypasses AI detectors. This is achieved by applying specific linguistic patterns that reflect genuine human writing rather than statistical text prediction.

---

## How AI Detectors Work (and How to Beat Them)

AI detectors measure two primary signals:

1. **Perplexity** — How *surprising* each word choice is. AI picks the most probable next word; humans often don't. Low perplexity = AI.
2. **Burstiness** — How much sentence length *varies*. AI writes in uniform, medium-length sentences. Humans mix very short punchy ones with longer, more winding ones. Low burstiness = AI.

To pass detectors, you must **raise both scores simultaneously**. Every rewrite decision should target one or both.

---

## Core Rewriting Principles

### 1. Destroy Sentence Uniformity (Fix Burstiness)
The single biggest tell. AI output looks like: medium. medium. medium. medium.

Human output looks like: short. Or really short. Then a much longer one that wanders a bit, maybe includes a tangent, and lands somewhere unexpected — before a short closer.

**Rules:**
- At least 20% of sentences should be ≤8 words
- At least 15% of sentences should be ≥30 words
- Never have more than 3 sentences of similar length in a row
- Use sentence fragments deliberately. For emphasis.

### 2. Inject Unpredictability (Fix Perplexity)
Swap "safe" word choices for slightly unexpected but still natural ones. The goal isn't obscure vocabulary — it's avoiding the statistically most-likely word.

| Instead of... | Try... |
|---|---|
| "utilize" | "use" / "lean on" / "pull in" |
| "implement" | "roll out" / "put in place" / "try" |
| "provide" | "give" / "hand over" / "offer up" |
| "important" | "matters" / "counts" / "actually makes a difference" |
| "significant" | "real" / "serious" / "worth noting" |
| "ensure" | "make sure" / "see to it" |
| "leverage" | "use" / "tap into" |
| "in order to" | "to" |
| "due to the fact that" | "because" |
| "at this point in time" | "now" / "right now" / "these days" |

### 3. Kill AI Filler Phrases
These are dead giveaways. Remove or rephrase every single one.

**Never use:**
- "It's worth noting that..."
- "It is important to note..."
- "In conclusion..." / "To summarize..."
- "Furthermore," / "Moreover," / "Additionally,"
- "Delve into"
- "In today's fast-paced world..."
- "It goes without saying..."
- "Let's explore..."
- "In this article, we will..."
- "Without further ado..."
- "As an AI language model..."
- "Certainly!" / "Absolutely!" / "Of course!"
- "I hope this helps!"
- "Feel free to..."
- "Navigating the complexities of..."
- "In the realm of..."
- "Multifaceted" / "Nuanced" / "Robust" / "Comprehensive" (when used vaguely)

**Replace transitions with variety:**
- Instead of "Furthermore" → "And honestly," / "On top of that," / "There's more:" / "Plus,"
- Instead of "However" → "But," / "That said," / "Still," / "Then again,"
- Instead of "Therefore" → "So," / "Which means," / "That's why,"
- Instead of "In addition" → "Also," / "And," / "Not to mention,"

### 4. Use Contractions Strategically
AI often avoids contractions in formal contexts. Humans use them everywhere — even in professional writing.

- "do not" → "don't"
- "it is" → "it's"
- "they are" → "they're"
- "would not" → "wouldn't"
- "cannot" → "can't"

Exception: Legal, medical, or highly formal documents may keep some contractions out. Use judgment.

### 5. Add Micro-Hedges and Personal Voice
Humans are uncertain. AI sounds certain.

**Insert hedges naturally:**
- "I think," / "I'd argue," / "Honestly,"
- "Probably," / "Maybe," / "Kind of,"
- "For the most part," / "In most cases,"
- "At least, that's been my experience."
- "Not always, but often."
- "Your mileage may vary."

**Direct address (where appropriate):**
- "You've probably seen this before."
- "Think about it this way."
- "Here's the thing:"
- "And that matters — a lot."

### 6. Vary Paragraph Density
AI generates even paragraph blocks. Humans don't.

**Pattern to follow:**
- One very short paragraph (1–2 sentences) every 3–4 paragraphs
- Occasionally a single-sentence paragraph for impact
- Let some paragraphs run longer when the idea warrants it

### 7. Use Concrete Specificity Over Vague Generalization
AI loves abstract claims. Humans tend to anchor with specifics.

- "Many studies show..." → "A 2022 Stanford study of 4,000 participants found..."
- "This is a growing problem." → "This has tripled in the last decade."
- "People often struggle with this." → "Most people give up within the first week."
- "It can have significant effects." → "It can cut your time in half — or double your costs."

When you don't have real specifics, simulate the *style* of specificity with plausible, confident detail.

### 8. Occasionally Break Grammar Rules (on Purpose)
Humans make intentional stylistic choices that break strict rules:

- Starting sentences with "And," "But," or "Because"
- Ending with a preposition: "...something to think about."
- Using em-dashes for interruptions — like this — mid-sentence
- Parenthetical asides (which humans love, maybe too much)
- Comma splices in casual contexts: "It works, I've tried it."
- One-word sentences. Done.

### 9. Adjust Passive vs. Active Voice
AI defaults to passive. Flip to active wherever possible.

- "It was noted that..." → "We noticed..."
- "The results were analyzed..." → "We analyzed the results..."
- "Errors may be encountered..." → "You might hit errors..."

### 10. Inject Rhetorical Questions
Humans ask questions in writing. AI almost never does this naturally.

- "But does that actually work in practice?"
- "Why does this keep happening?"
- "So what's the takeaway here?"
- "Is it really that simple? Sometimes, yes."

---

## Rewriting Workflow

When asked to humanize text, follow these steps in order:

### Step 1: Analyze the Input
Quickly scan for:
- Uniform sentence length (fix with burstiness techniques)
- Banned phrases (remove all)
- Passive voice patterns (flip to active)
- Vague generalities (add specificity)
- Missing contractions (add them)

### Step 2: Full Rewrite (Preferred) or Targeted Edit
- **Full rewrite** is almost always better for passing detectors — preserve the meaning and structure, but rebuild the language from scratch
- **Targeted edit** is acceptable when the user needs light touch or the content is already mostly good

### Step 3: Apply the Final Checklist
Before returning the output, verify:
- [ ] At least 1 sentence fragment or very short sentence in every 5
- [ ] No banned AI phrases present
- [ ] Contractions used naturally throughout
- [ ] At least one rhetorical question or direct address (in most pieces)
- [ ] At least one specific data point, example, or concrete detail
- [ ] Paragraph lengths vary (no 3 consecutive same-size paragraphs)
- [ ] Transitions are varied (no repeated "Furthermore" / "Moreover")
- [ ] No passive-voice clusters

### Step 4: Tone Matching
Always match the user's intended voice:
- **Academic**: Keep some formality, but break it with short punchy sentences and hedges
- **Blog/casual**: Full contractions, rhetorical questions, fragments welcome
- **Professional/business**: Active voice, drop filler, moderate contractions
- **Creative**: Full license to play with grammar and rhythm
- **Cover letter/personal statement**: First person, specific anecdotes, direct and warm

---

## Format for Response

1. **Output the rewritten text first** — clean, no markup
2. Then (briefly) note the main changes made, grouped by technique
3. If the original had specific issues (e.g., heavy passive voice, banned phrases), call those out

Do NOT explain the entire technique list unless the user asks. Keep the after-note tight — 3–5 bullet points maximum.

---

## Reference Files

- `references/banned-phrases.md` — Extended list of AI giveaway phrases to always remove
- `references/detector-notes.md` — How specific detectors (GPTZero, Turnitin, ZeroGPT) weight their signals and any additional tips per platform
