---
name: french-flashcard-generator
description: Generate French flashcards from sentence mining. Create cloze deletion, audio, reverse cards, and grammar cards. Output in Obsidian Spaced Repetition format and Anki deck.
license: MIT
compatibility: Works with French vocabulary and sentence data
metadata:
  author: user
  version: "1.0"
---

# French Flashcard Generator

Generate effective flashcards for French learning using spaced repetition principles. Create various card types from vocabulary and sentence data.

## Input

Provide one or more:
- French vocabulary item with details
- Mined sentence with pattern
- Grammar point
- Expression with usage
- Previous session data for bulk generation

## Flashcard Types

### 1. Cloze Deletion Cards

Create cards by removing key elements from sentences:

**Vocabulary Cloze**:
```
Je ___ un café ce matin. (prendre)
Answer: prends
```

**Pattern Cloze**:
```
Je me suis rendu ___ que c'était difficile. (combe)
Answer: compte
```

**Translation Cloze**:
```
___ (I need) d'aide.
Answer: J'ai besoin
```

### 2. Vocabulary Cards

Basic word/phrase cards:

**Front**: French word/phrase
**Back**: Meaning, pronunciation, example

### 3. Reverse Cards

Two-way cards for bidirectional recall:

**Front → Back**: French → English
**Back → Front**: English → French

### 4. Audio Cards

Cards with pronunciation focus:

- Audio on front
- Listen and respond
- For pronunciation practice

### 5. Grammar Cards

Focus on grammar patterns:

**Type 1 - Rule Cards**:
- Front: Rule description
- Back: Explanation + examples

**Type 2 - Conjugation Cards**:
- Front: Verb in infinitive + tense
- Back: Conjugated form

**Type 3 - Structure Cards**:
- Front: Sentence pattern
- Back: Fill in the blank

## Output Formats

### Obsidian Spaced Repetition (SR) Format

```markdown
---
tags:
  - french
  - vocab
  - sr
deck: French Vocab
---

## Front

avoir besoin de

## Back

Meaning: to need

Example: J'ai besoin d'aide.

<!--SR:2024-01-15,2024-01-18,2024-01-22,2024-01-27,2024-02-02-->
```

### Cloze SR Format

```markdown
---
tags:
  - french
  - cloze
  - sr
deck: French Cloze
---

## Front

Je me suis ___ [c]que[/c] que c'était difficile.

## Back

se rendre compte

<!--SR:2024-01-15,2024-01-18,2024-01-22,2024-01-27,2024-02-02-->
```

### Anki Format

Export as:
- APKG (Anki package)
- CSV for manual import
- Markdown with Anki tags

#### CSV Format
```csv
front,back,tags,deck
avoir besoin de,"Meaning: to need<br>Example: J'ai'ai besoin d'aide.",french vocab,French Vocab
Je ___ un café,"prendre - to take<br>Je prends un café.",french cloze,French Cloze
```

### Anki Fields

| Field | Content |
|-------|---------|
| Front | Question/prompt |
| Back | Answer + context |
| Tags | french, vocab, cloze, audio, grammar |
| Deck | Deck name |
| Audio | [Sound:filename.mp3] |

## Card Generation Workflow

### From Sentence Mining Data

Input:
```markdown
# Sentence

Je me suis rendu compte que ce n'était pas si difficile.

## Pattern
se rendre compte que + indicative

## Translation
I realized that it wasn't that difficult.

## Tags
#verb/pronominal #B1 #discovery
```

Generate:

1. **Basic Vocab Card**:
   - Front: se rendre compte (de)
   - Back: to realize, to become aware

2. **Cloze Card 1**:
   - Front: Je me suis ___ compte que...
   - Back: rendu

3. **Cloze Card 2**:
   - Front: Je me suis rendu ___ que...
   - Back: compte

4. **Pattern Card**:
   - Front: se rendre compte ___ + indicative?
   - Back: que - used after "se rendre compte"

5. **Reverse Card**:
   - Front: to realize (French)
   - Back: se rendre compte (de)

### From Vocabulary Input

Input: "avoir besoin de - to need - expression - A2 - J'ai besoin d'aide."

Generate:
1. Vocab card
2. Translation cloze ("___ d'aide" → "avoir besoin")
3. Reverse card
4. Example sentence cloze

## Cloze Deletion Strategies

### Single Cloze
```
Le chat ___ sous le lit. (être)
Answer: est
```

### Multiple Cloze
```
Je ___ que tu ___ venir. (vouloir/pouvoir)
Answers: veux, peux
```

### Custom Cloze
```
avoir ___ de (to need)
Answer: besoin
```

### Context Cloze
```
- Tu veux quelque chose ?
- Oui, j'ai ___ d'aide. (avoir besoin)
Answer: besoin
```

### Grammar Cloze
```
Si j'étais ___ (riche), je voyagerais.
Answer: riche (imparfait)
```

## Audio Integration

### Audio Tags for Anki
```
[sound:avoir_besoin_de.mp3]
```

### Audio Tags for Obsidian SR
```markdown
![audio](avoir_besoin_de.mp3)
```

### Sources
- Text-to-speech (future)
- Pre-recorded audio files
- AI-generated pronunciation

### Audio Card Types
1. **Listen and translate**
2. **Listen and speak back**
3. **Dictation** (type what you hear)

## Grammar Cards

### Verb Conjugation

**Infinitive + Tense**:
```
Front: parler - passé composé
Back: j'ai parlé, tu as parlé, il/elle a parlé...
```

**Irregular Verbs**:
```
Front: être - subjonctif présent
Back: que je soit, que tu sois, qu'il soit...
```

### Structure Cards

**Pattern**: Subjunctive triggers
```
Front: Verbes de émotion + subjonctif
Back: avoir peur que, regretter que, être content que...
```

### Rule Cards

**Rule**: When to use subjunctive
```
Front: Quand utilise-t-on le subjonctif ?
Back: After expressions of will, emotion, doubt, necessity
```

## Example Output

### Complete Card Set

```markdown
# Card Set: se rendre compte

## Card 1: Vocab

**Front**: se rendre compte (de)
**Back**: to realize, to become aware
**Tags**: #french #verb #pronominal #B1

---

## Card 2: Cloze - Verb

**Front**: Je me suis ___ compte que...
**Back**: rendu
**Tags**: #french #cloze #verb

---

## Card 3: Cloze - Pattern

**Front**: Je me suis rendu ___ que...
**Back**: compte
**Context**: se rendre compte que + indicatif
**Tags**: #french #cloze #pattern

---

## Card 4: Translation

**Front**: I realized that...
**Back**: Je me suis rendu compte que...
**Tags**: #french #translation #B1

---

## Card 5: Example

**Front**: J'ai ___ que ce n'était pas si difficile.
**Back**: me rendu compte
**Tags**: #french #example #sentence

---

## Card 6: Reverse

**Front**: to become aware
**Back**: se rendre compte (de)
**Tags**: #french #reverse #vocab
```

### Anki CSV Export

```csv
front,back,tags,deck
se rendre compte (de),"to realize, to become aware",french vocab,French Vocab
Je me suis rendu ___ compte que...,"rendu - realized",french cloze,French Cloze
Je me suis rendu compte ___,"que - used after 'se rendre compte'",french pattern,French Patterns
I realized that...,Je me suis rendu compte que...,french translation,French Translation
J'ai ___ que ce n'était pas si difficile.,"me rendu compte - realized",french example,French Examples
```

## Deck Organization

### By Level
- French-A1-Start
- French-A2-Basics
- French-B1-Intermediate
- French-B2-Upper
- French-C1-Advanced
- French-C2-Master

### By Type
- Vocab
- Cloze
- Grammar
- Pronunciation
- Expression

### By Topic
- Daily Life
- Travel
- Work
- Emotions
- Time
- Numbers

## Spaced Repetition Settings

### Initial Intervals (Anki)
- Again: 1 minute
- Hard: 1 day
- Good: 4 days
- Easy: 7 days

### Graduation
- New → Learning: 1 successful review
- Learning → Review: 3 successful reviews

### Review Limits
- New cards/day: 20
- Reviews/day: 100

## Bulk Generation

When processing multiple items:

1. Group by type
2. Apply consistent tagging
3. Balance card types
4. Add variety
5. Track generation stats

### Generation Report

```
Generated: 45 cards
├── Vocabulary: 15
├── Cloze: 20
├── Grammar: 8
├── Reverse: 10
└── Audio: 2

Tagged: #french #B1
Deck: French-B1-Intermediate

Ready for: Obsidian SR, Anki
```

## Quality Guidelines

- Keep cards simple (one concept per card)
- Use natural contexts
- Include audio when possible
- Test reverse cards
- Balance difficulty
- Review generated cards
- Update based on performance