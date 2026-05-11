# AI Detector Notes — Platform-Specific Tips

## GPTZero
**What it measures:** Perplexity + burstiness, sentence-level and document-level. Also has a "model probability" classifier trained on GPT/Claude outputs.

**Most important fixes:**
1. Burstiness is heavily weighted — focus hard on sentence length variation
2. Avoid starting consecutive sentences with the same grammatical structure (e.g., three sentences in a row starting with "The...")
3. GPTZero is trained heavily on GPT-4 outputs, so Claude-specific patterns (very structured, thorough, numbered lists for everything) are also flagged
4. One-sentence paragraphs help a lot — they spike burstiness dramatically
5. Informal rhetorical questions help because they're low-probability in formal text

**Green flags (things GPTZero rewards):**
- Fragments. Real ones.
- Mixed register (formal sentence followed by a casual one)
- Self-corrections or caveats mid-paragraph
- Personal anecdotes or first-person observations
- Unusual but natural word choices

---

## Turnitin AI Detection
**What it measures:** Primarily a writing style classifier, not pure perplexity. Trained to detect patterns in structure, hedging, transition use, and predictability at the phrase level.

**Most important fixes:**
1. Eliminate all transitional filler ("Furthermore," "Moreover," "Additionally,")
2. Avoid perfectly parallel list structures (three bullet points of exactly similar length are a red flag)
3. Turnitin is very sensitive to the "thesis → body → conclusion" structure in essays — break the mold
4. Add genuine imperfection: a slightly run-on sentence, an em-dash aside, a parenthetical thought
5. Do NOT rely on just swapping synonyms — Turnitin's classifier goes beyond word-level to syntax patterns

**Green flags:**
- Idiomatic English that's slightly informal
- Non-standard essay structure
- Quoted material or attributed claims (shows research, not generation)
- Variation in clause structure (not just sentence length)

---

## ZeroGPT
**What it measures:** A hybrid of perplexity and a trained classifier. Tends to be more aggressive than GPTZero and has a higher false-positive rate.

**Most important fixes:**
1. ZeroGPT is very sensitive to repetitive syntactic structures — vary how clauses are built, not just length
2. Short paragraphs are extremely effective here — ZeroGPT scores block-by-block
3. Avoid perfect grammar throughout — one comma splice or casual aside can shift scores significantly
4. Run-on sentences (when intentional) score well

**Green flags:**
- Anything that breaks the "clean, organized, easy-to-read" pattern
- Direct address to the reader
- Opinion stated without hedging (e.g., "This is wrong." not "This may be considered suboptimal.")

---

## Originality.ai
**What it measures:** One of the more accurate detectors — uses a fine-tuned classifier specifically trained to distinguish human vs. AI writing patterns at the semantic level.

**Most important fixes:**
1. Word swapping alone won't fool this one — full sentence restructuring is required
2. Particularly sensitive to AI's tendency to be comprehensive and exhaustive — humans leave things out
3. Add opinions, preferences, and takes that aren't universally true ("Personally, I prefer X even though many people disagree")
4. Include some imprecision — humans don't always give the complete picture

**Green flags:**
- Tangential observations ("This reminds me of...")
- Admitting uncertainty ("I'm not totally sure about this, but...")
- Incomplete coverage (not listing every single consideration)
- Informal logic flow (humans jump around; AI is linear)

---

## Copyleaks
**What it measures:** AI classifier + plagiarism detection in one. The AI detection component focuses on semantic predictability.

**Most important fixes:**
1. High sentence-level entropy — each sentence should feel like it could have gone a different direction
2. Avoid topic sentences that perfectly summarize the paragraph that follows
3. Use some passive voice (strategically) — 100% active voice is also a tell
4. Vary between showing and telling within the same paragraph

---

## General Strategies That Help Across All Detectors

1. **The "omission" trick**: Real human writers don't cover everything. Drop one obvious point and the coherence score drops below what AI would produce.

2. **Double structure variation**: Change both sentence length AND sentence type (declarative, interrogative, exclamatory, conditional) within each paragraph.

3. **The mid-paragraph pivot**: Start a paragraph going one direction, then course-correct or add a counterpoint partway through. AI finishes what it starts cleanly; humans often don't.

4. **Format inconsistency**: Mix formatted and unformatted text. Not every list needs bullets. A paragraph that could have been a list but wasn't is a human signal.

5. **After humanizing, read aloud**: If it sounds like it was written by a person in a conversation, it will likely pass. If it sounds like it was read from a document, it probably won't.
