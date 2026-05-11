---
name: french-sentence-miner
description: Extract high-value French sentences from various sources (transcripts, novels, articles, subtitles). Identify grammar patterns, colloquial expressions, and generate bilingual explanations with auto-tagging for spaced repetition.
license: MIT
compatibility: Works with any French text source
metadata:
  author: user
  version: "1.0"
---

# French Sentence Miner

Extract and analyze valuable French sentences from any source for language learning.

## Input Types

Process these input types:
- Video/audio transcripts (YouTube, podcast)
- Novels and literary texts
- News articles and blog posts
- Subtitle files (SRT, VTT, ASS)
- Any French text content

## Workflow

### 1. Identify Worth-Learning Sentences

Select sentences that are:
- **Pattern-rich**: Contains useful grammatical structures (subjunctive, relative pronouns, conditional, passive, etc.)
- **Natural**: Authentic usage from native content
- **Transferable**: Pattern can be reused in many contexts
- **Intermediate+**: Not overly simple, but not niche jargon

Prioritize:
- Sentences with verb patterns (pronominal verbs, impersonal expressions)
- Sentences with idiomatic expressions
- Sentences showing discourse markers
- Sentences with connectors and transitions

Avoid:
- Sentences with heavy proper nouns or specific references
- Sentences too simple (just subject + verb + object)
- Sentences too context-dependent

### 2. Extract Grammar Patterns

For each selected sentence, identify:
- **Main pattern**: The reusable grammatical or lexical pattern
- **Components**: Breaking down how the pattern works
- **Usage context**: When this pattern is used

Examples:
- `se rendre compte que` - pronominal verb + que clause
- `Il n'est pas rare de + inf` - impersonal expression + infinitive
- `quoi que + subj` - concessive conjunction

### 3. Mark Colloquial Expressions

Identify and tag:
- **Spoken French**: Contractions, elisions common in speech (j'suis, j'comprends)
- **Informal**: Casual expressions (genre, quoi, enfin)
- **Idiomatic**: Non-literal expressions (avoir la flemme, c'est bon)
- **Regional**: Common in France vs. Quebec (putain vs. tabernacle)

### 4. Generate Bilingual Explanation

Provide clear translations:
- **Literal**: Word-for-word when helpful
- **Natural**: How a native speaker would express it in English
- **Context**: When to use this sentence

### 5. Auto-Tag

Add relevant tags for organization:
- Grammar: #verb/pronominal #subjunctive #relative-pronoun #conditional #impersonal
- Level: #A1 #A2 #B1 #B2 #C1 #C2
- Type: #spoken #written #idiom #expression #pattern
- Topic: #emotion #time #comparison #cause #result #contrast

## Output Format

For each sentence, output:

```markdown
# Sentence

[Original French sentence]

## Pattern
[Grammar pattern name or expression]

## Translation
[Natural bilingual translation]
- Literal: [if helpful]
- Context: [when to use]

## Tags
#grammar-type #level #style

## Notes
[Any additional context, common mistakes, related patterns]
```

### Example Output

```markdown
# Sentence

Je me suis rendu compte que ce n'était pas si difficile.

## Pattern
se rendre compte que + indicative

## Translation
I realized that it wasn't that difficult.
- Literal: "I made myself aware that..."
- Context: Used when you come to understand something

## Notes
- Colloquial: Often shortened to "Je me suis rendu compte..." in speech
- Related: [[s'apercevoir que]] (to notice), [[prendre conscience que]] (to become aware)

## Tags
#verb/pronominal #B1 #discovery #understanding
```

### Another Example

```markdown
# Sentence

Quoi qu'il arrive, je serai là.

## Pattern
quoi qu + subjunctive (imperative mood)

## Translation
Whatever happens, I'll be there.
- Literal: "What whatever it comes..."
- Context: Making promises, showing commitment

## Tags
#subjunctive #conjunction #B2 #promise #certainty
```

## Batch Processing

When multiple sentences are found, present as a ranked list by learning value:

| # | Sentence | Pattern | Level | Tags |
|---|----------|---------|-------|------|
| 1 | Je me suis rendu compte que... | se rendre compte que | B1 | #pronominal #discovery |
| 2 | C'est la première fois que... | c'est la première fois que | B1 | #tense #experience |
| 3 | Si jamais tu as besoin... | si jamais + future | B2 | #condition #offer |

Follow with full details for each sentence in Obsidian format.

## Guidelines

- Extract 3-10 sentences per source (depending on length)
- Focus on variety of patterns
- Prefer sentences with multiple learning points
- Note source for context but don't over-cite
- Make translation natural, not literal
- Include pronunciation notes for tricky items