---
name: french-vocab-extractor
description: Extract and analyze French vocabulary from various sources (text, YouTube transcripts, podcast subtitles, web pages). Identify high-frequency words, CEFR levels, parts of speech, examples, word roots, and generate Obsidian notes.
license: MIT
compatibility: Works with any text input
metadata:
  author: user
  version: "1.0"
---

# French Vocabulary Extractor

Extract and analyze French vocabulary from provided content, create structured vocabulary notes for Obsidian.

## Input Types

Process these input types:
- Plain French text passages
- YouTube video transcripts
- Podcast subtitles (SRT, VTT)
- Web page content
- **Transcriptions**: French interview/podcast transcripts with Chinese translation (stored in `transcriptions/` folder)

## Workflow

### 0. Store Transcriptions

For video/audio sources, also create transcription files in `transcriptions/` folder with:
- Original French transcript
- Chinese translation
- Key vocabulary highlighted
- Audio/video source link

### 1. Analyze the Input

Read the provided French content and identify:
- Unique vocabulary items (excluding very common words like "le", "la", "de", "et", "un", "une", "est", "sont", "que", "qui", "dans", "pour", "avec", "sur", "ce", "cet", "cette", "ces", "je", "tu", "il", "elle", "nous", "vous", "ils", "elles")
- Key phrases and expressions
- Verb conjugations and idioms

### 2. Extract High-Frequency Words

Prioritize vocabulary based on frequency and usefulness:
- A1-A2: Basic nouns, verbs, adjectives
- B1-B2: Intermediate expressions, complex structures
- C1-C2: Advanced vocabulary, nuances

Select 5-15 most valuable words/phrases from the content.

### 3. Research Each Word/Phrase

For each selected item, find:
- **Meaning**: Clear English translation
- **Type**: noun, verb, adjective, adverb, expression, preposition, conjunction
- **CEFR Level**: A1, A2, B1, B2, C1, or C2 (estimate based on frequency and complexity)
- **Examples**: 1-2 authentic example sentences from the source or constructed naturally
- **Word Root**: Etymology or root if applicable (especially for Latin-based words)

### 4. Generate Obsidian Note

Create a well-structured vocabulary note in Markdown format:

```markdown
# [Word or Expression]

**Meaning**: [English translation]
**Type**: [part of speech / expression type]
**CEFR Level**: [A1/A2/B1/B2/C1/C2]
**Source**: [where you found it]

## Examples
- [Example sentence 1]
- [Example sentence 2]

## Related
- [[related words]]

## Notes
[Any additional context, nuances, or memory tips]
```

### 5. Group Related Vocabulary

For expressions like "avoir besoin de", create notes that show:
- The full expression as the heading
- Component breakdown if useful
- Related expressions

## Output Format

Present vocabulary in a clear table format followed by individual Obsidian-ready notes for each item.

### Example Output

| Word/Expression | Meaning | Type | CEFR | Examples |
|-----------------|---------|------|------|----------|
| avoir besoin de | to need | expression | A2 | J'ai besoin d'aide. |
| manquer | to miss/lack | verb | B1 | Il manque de temps. |

---

## Obsidian Notes

### avoir besoin de

**Meaning**: to need
**Type**: expression (verb + preposition)
**CEFR Level**: A2
**Source**: [source reference]

**Examples**:
- J'ai besoin d'aide.
- Nous avons besoin de temps.

**Related**:
- [[falloir]] - to be necessary
- [[avoir envie de]] - to want

**Notes**: Literal meaning is "to have need of". Used to express necessity or strong need.