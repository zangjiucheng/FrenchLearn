---
name: french-writing-corrector
description: Correct and analyze French writing. Identify grammar issues, suggest natural phrasing, estimate CEFR level, and provide native alternatives. Build a personal common mistakes database.
license: MIT
compatibility: Works with any French text input
metadata:
  author: user
  version: "1.0"
---

# French Writing Corrector

Correct French text, analyze errors, suggest improvements, and build a personal mistake database for learning.

## Input Types

Accept:
- Single sentences
- Paragraphs
- Full texts (up to 500 words)
- Chat messages
- Written assignments
- Social media posts

## Workflow

### 1. Correct the Text

Provide a corrected version:
- Fix grammatical errors
- Correct spelling and accents
- Improve word order
- Fix punctuation

### 2. Identify Grammar Issues

Categorize each error:
- **Verb**: tense, conjugation, agreement
- **Noun**: gender, number, article
- **Adjective**: agreement, position
- **Pronoun**: usage, agreement, position
- **Preposition**: wrong preposition, missing
- **Word order**: French vs English order
- **Syntax**: sentence structure issues

### 3. Suggest Natural Phrasing

Show more natural alternatives:
- Too literal translations
- Unnatural word choices
- Formal vs informal
- Academic vs spoken

### 4. Estimate CEFR Level

Assess based on:
- Vocabulary complexity
- Sentence structure sophistication
- Error types
- Natural expression level

Provide: A1, A2, B1, B2, C1, or C2 with confidence level

### 5. Provide Native Alternatives

Offer alternative ways to express the same idea:
- More common expressions
- Different structures
- Native phrasing

### 6. Build Common Mistakes Database

Track patterns to create:
- Personalized error patterns
- Frequency analysis
- Areas for focus
- Review materials

## Output Format

```markdown
# Writing Correction

## Original
> [User's text]

## Corrected
> [Corrected version]

---

## Issues Found

| Error | Type | Fix |
|-------|------|-----|
| suis allé | Verb | "Je suis allé" (gender agreement) |
| au magasin | Preposition | "au" is correct but specify: "à la boulangerie" |

---

## Grammar Breakdown

### Verb Issues
- **être + allé**: CORRECT - motion verbs use être
- **Genre agreement**: Verify feminine form for female speaker

### Preposition Notes
- "au magasin" is grammatically correct
- More natural: specify which store

---

## Natural Phrasing

**Original**: "Aujourd'hui je suis allé au magasin..."
**More natural**:
- "Ce matin, je suis allé à la boulangerie."
- "Hier, je suis passé au Supermarché."

**Why**: Specify time + specific place sounds more natural

---

## CEFR Estimate

**Level**: B1
**Confidence**: 85%
**Reasoning**:
- Uses passé composé correctly
- Basic sentence structure
- Limited vocabulary range
- Some word choice issues

---

## Native Alternatives

**To say "I went to the store"**:
- "Je suis allé faire des courses." (went shopping)
- "Je suis passé au commerce." (popped by)
- "Je me suis rendu au magasin." (more formal)

---

## Common Mistakes Database

### This Error Type: Motion Verbs
**Pattern**: Motion verbs (aller, partir, venir) require être
- ✅ "Je suis allé au cinéma."
- ✅ "Elle est partie tôt."
- ❌ "J'ai allé..." (common English learner error)

**Similar verbs**: aller, partir, venir, arriver, retourner, entrer, sortir, tomber, monter, descendre

### Pattern: Time Expressions
- ✅ "Ce matin" / "Aujourd'hui" - don't mix
- ✅ "Hier" / "Ce matin" - clear time markers
```

### Detailed Example

```markdown
# Writing Correction

## Original
> "Je mange le petit-déjeuner à 7h du matin et puis je vais au travail."

## Corrected
> "Je prends le petit-déjeuner à 7h du matin, puis je vais au travail."

---

## Issues Found

| Error | Type | Fix | Explanation |
|-------|------|-----|-------------|
| mange | Verb | "prends" | "Manger le petit-déjeuner" uses "prendre", not "manger" |
| le petit-déjeuner | Noun | correct | OK |
| à 7h du matin | Time | correct | OK, but "à 7 heures" more common |
| et puis | Connector | "puis" or "et" | Redundant - choose one |
| au travail | Preposition | correct | OK |

---

## Grammar Breakdown

### Verb Choice: "prendre" vs "manger"
- **Manger** = to eat (general)
- **Prendre** = to take (for meals: prendre le petit-déjeuner, prendre le déjeuner, prendre le dîner)

**Rule**: You "take" a meal in French, not "eat" it

### Connector: "et puis" vs "puis"
- "et puis" = and then (when connecting two clauses)
- "puis" = then (used at beginning or after punctuation)
- In list: "puis" is sufficient

---

## Natural Phrasing

**Too literal**: "Je mange le petit-déjeuner..."
**Natural**: "Je prends le petit-déjeuner..."

**More variations**:
- "Je déjeune à 7h." (more casual)
- "Le matin, je prends un café et des tartines." (describe what you eat)
- "7h, c'est l'heure de mon petit-déjeuner." (time-focused)

---

## CEFR Estimate

**Level**: A2
**Confidence**: 90%
**Reasoning**:
- Simple present + past composition
- Basic vocabulary
- Some word choice issues (manger vs prendre)
- Clear but limited expression

---

## Native Alternatives

**Same meaning, more natural**:
1. "Je prends mon petit-déjeuner à 7h, ensuite je vais au travail."
2. "Le matin, je déjeune à 7h avant d'aller au bureau."
3. "7h: petit-déjeuner. 7h30: direction le travail."

---

## Common Mistakes Database

### ❌ Error Pattern: Meal Verbs

**Common mistake**: Using "manger" for all meals
**Correction**: Use "prendre" for meals

| Meal | Correct | Incorrect |
|------|---------|-----------|
| Breakfast | prendre le petit-déjeuner | manger le petit-déjeuner |
| Lunch | prendre le déjeuner | manger le déjeuner |
| Dinner | prendre le dîner | manger le dîner |

**Mnemonic**: You "take" time for meals in French

### ❌ Error Pattern: Time Expressions

**Common mistake**: "à 7h du matin" (redundant)
**Better**: "à 7h" or "à 7 heures du matin" (if clarifying morning vs evening)

**Note**: "du matin" is used to distinguish from afternoon/evening
- "à 7h du matin" (7 AM)
- "à 7h du soir" (7 PM)
```

## Database Structure

Track common mistakes in this format:

```markdown
# Common Mistakes

## [Error Category]

### Pattern: [Error Type]
**Original**: [Common wrong form]
**Correct**: [Right form]
**Why**: [Explanation]

### Examples
- ❌ [wrong]
- ✅ [correct]

### Related Errors
- [[Link to related mistake]]
- [[Another related]]
```

### Error Categories

1. **Verb Errors**
   - Tense confusion (passé composé vs imparfait)
   - Agreement with être
   - Subjunctive triggers
   - Infinitive vs past infinitive

2. **Noun/Article Errors**
   - Gender confusion
   - Wrong article (le/la vs un/une)
   - Partitive articles (du/de la)

3. **Preposition Errors**
   - "à" vs "de" after verbs
   - Geographic prepositions
   - Time expressions

4. **Word Order**
   - Pronoun placement
   - Question formation
   - Negative construction

5. **Word Choice**
   - False friends
   - Too literal translations
   - Register issues

## Guidelines

- Be encouraging - focus on what they did well
- Explain WHY, not just what to fix
- Prioritize errors by impact
- Provide alternatives, not just corrections
- Build the database with each correction
- Note patterns across corrections
- Distinguish between errors and style preferences
- Consider context (formal vs informal)