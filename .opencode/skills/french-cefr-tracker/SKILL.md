---
name: french-cefr-tracker
description: Automatically analyze French proficiency across vocabulary complexity, grammar usage, listening, and speaking. Estimate CEFR level (A1-C2) and recommend gaps for targeted improvement.
license: MIT
compatibility: Requires French language samples
metadata:
  author: user
  version: "1.0"
---

# French CEFR Tracker

Automatically assess your French proficiency level. Analyze vocabulary, grammar, listening, and speaking to estimate your CEFR level and identify gaps.

## Input

Provide samples across:
- Written text (journal, essay, chat)
- Transcripts of listened content
- Audio/video for listening assessment
- Speaking recordings or transcripts
- Vocabulary lists

Or provide access to your learning data.

## Analysis Dimensions

### 1. Vocabulary Complexity

**Metrics**:
- Average word length
- Sophistication of word choice
- Domain-specific vocabulary presence
- Abstract vs concrete language
- Idiom usage

**Indicators by Level**:

| A1 | A2 | B1 | B2 | C1 | C2 |
|----|----|----|----|----|----|
| Basic nouns, common verbs | Expanded vocabulary, some adjectives | Varied vocabulary, some idioms | Rich vocabulary, idioms, nuances | Advanced vocabulary, rare words | Near-native word choice |
| 500-1000 words | 1000-2000 words | 2000-4000 words | 4000-6000 words | 6000-10000+ words | Native-like range |

### 2. Grammar Usage

**Metrics**:
- Sentence complexity
- Tense usage (basic vs advanced)
- Mood usage (indicative, subjunctive, conditional)
- Pronoun usage (basic vs complex)
- Clause structures

**Indicators by Level**:

| A1 | A2 | B1 | B2 | C1 | C2 |
|----|----|----|----|----|----|
| Simple present, past | passé composé, imparfait | Future, conditional | Subjunctive, complex tenses | All tenses, nuances | Native-like structures |
| Short sentences | Compound sentences | Complex sentences | Subordinate clauses | Sophisticated discourse | Creative constructions |

### 3. Listening Level

**Metrics**:
- Comprehension of slow vs normal speech
- Familiar vs unfamiliar topics
- Clear vs accented speech
- Abstract concepts
- Fast native speech

**Indicators by Level**:

| A1 | A2 | B1 | B2 | C1 | C2 |
|----|----|----|----|----|----|
| Slow, clear, familiar | Normal speed, familiar topics | Native speed, some unknowns | Fast native, most topics | Fast, abstract, accented | Native, all conditions |

### 4. Speaking Fluency

**Metrics**:
- Hesitation frequency
- Vocabulary retrieval speed
- Grammar auto-correction
- Pronunciation clarity
- Connected speech

**Indicators by Level**:

| A1 | A2 | B1 | B2 | C1 | C2 |
|----|----|----|----|----|----|
| Slow, many pauses | Basic fluency, some hesitations | Natural speed, occasional pauses | Fluent, few hesitations | Smooth, native-like | Native speed and flow |

## CEFR Descriptors Used

### A1 - Beginner
- Can understand and use familiar everyday expressions
- Can introduce themselves and others
- Can ask and answer questions about personal details
- Can interact in a simple way if the other person talks slowly

### A2 - Elementary
- Can communicate in simple and routine tasks
- Can describe aspects of their background and immediate environment
- Can exchange information on familiar topics

### B1 - Intermediate
- Can understand the main points of clear standard input on familiar matters
- Can deal with most situations likely to arise while travelling
- Can produce simple connected text on topics of personal interest
- Can describe experiences, events, dreams, and ambitions

### B2 - Upper Intermediate
- Can understand the main ideas of complex text on both concrete and abstract topics
- Can interact with a degree of fluency and spontaneity
- Can produce clear, detailed text on a wide range of subjects

### C1 - Advanced
- Can understand a wide range of demanding texts
- Can express ideas fluently and spontaneously without obvious searching
- Can use language flexibly and effectively for social and professional purposes

### C2 - Mastery
- Can understand with ease virtually everything heard or read
- Can summarize information from different sources
- Can express themselves spontaneously with very natural flow

## Output Format

```markdown
# CEFR Level Assessment

**Date**: [Assessment Date]

---

## 📊 Overall Level: B1

**Confidence**: 80%

---

## Breakdown by Dimension

| Dimension | Level | Confidence |
|-----------|-------|------------|
| Vocabulary | B1 | 85% |
| Grammar | A2-B1 | 70% |
| Listening | B1 | 80% |
| Speaking | A2-B1 | 65% |

---

## Vocabulary Analysis

### Your Vocabulary Profile
- **Range**: ~2000 words (estimate)
- **Quality**: Mix of basic + intermediate
- **Strength**: Concrete nouns, everyday verbs
- **Gap**: Abstract vocabulary, idioms

### Evidence
✓ Strong: "manger", "aller", "parler" - basic verbs
✓ Strong: Food, travel, daily activities vocabulary
⚠ Weak: Few idiomatic expressions
⚠ Weak: Abstract concepts (emotions, opinions)

**Sample from your text**: Simple concrete words dominate

---

## Grammar Analysis

### Your Grammar Profile
- **Strengths**: Basic sentence structure, passé composé
- **Weaknesses**: Subjunctive rarely used, complex subordinate clauses

### Evidence
✓ Present, past, future basic forms
✓ Simple compound sentences
⚠ Subjunctive: Only 1 instance (should be more for B1)
⚠ Conditionals: Not used (should appear at B1)

**Verdict**: A2 grammar with some B1 elements

---

## Listening Analysis

### Your Listening Profile
- **Comprehension**: ~70% of slow-native content
- **Speed**: Need slightly slower than native
- **Accent**: France French okay, Quebec harder

### Evidence
✓ France news: Good comprehension
✓ Slow podcasts: Good
⚠ Native speed: Miss 30%
⚠ Unknown topics: Significant gaps

**Verdict**: B1 listening - can handle familiar topics at near-native speed

---

## Speaking Analysis

### Your Speaking Profile
- **Fluency**: Basic, frequent pauses
- **Accuracy**: Simple sentences mostly correct
- **Complexity**: Rarely uses complex structures

### Evidence
✓ Basic vocabulary available
⚠ Hesitations every 3-4 sentences
⚠ Rarely initiates complex sentences
⚠ Limited range of expressions

**Verdict**: A2-B1 speaking - functional but limited

---

## 🎯 Gap Analysis & Recommendations

### Priority Gaps

| Gap | Current | Target | Priority |
|-----|---------|--------|----------|
| Subjunctive | Rare | Frequent (B1) | 🔴 High |
| Conditionals | None | Basic usage (B1) | 🔴 High |
| Idioms | None | Some (B1) | 🟠 Medium |
| Listening speed | Slow | Normal (B1) | 🟠 Medium |
| Speaking complexity | Simple | Compound (B1) | 🟠 Medium |

### Recommended Focus

**1. Subjunctive Trigger Practice** (Week 1-2)
- Learn: verbs of emotion, will, doubt
- Practice: Fill in the blank exercises
- Target: 10 sentences with subjunctive daily

**2. Basic Conditionals** (Week 2-3)
- Learn: si + imparfait, conditionnel présent
- Practice: Rewrite sentences using conditionals
- Target: 5 conditional sentences daily

**3. Idioms for Everyday Use** (Week 3-4)
- Learn: 20 common French idioms
- Practice: Replace literal expressions with idioms
- Target: Use 2 idioms in daily journal

**4. Listening Acceleration** (Ongoing)
- Method: Progressive speed increase
- Start: 0.75x speed
- Week 2: 0.85x
- Week 4: 1x

**5. Speaking Complexity** (Ongoing)
- Method: Sentence expansion drills
- Start: Add one element to each sentence
- Goal: 2-clause sentences by month end
```

### Detailed Assessment

```markdown
# CEFR Assessment - Detailed

## Input Samples Provided
- Journal entries: 5 samples (~150 words each)
- Listening: 2 podcast transcripts (France Info, innerFrench)
- Writing corrections: 8 entries analyzed

---

## Vocabulary Deep Dive

### Word Frequency Analysis
Your top words:
1. je (pronoun) - 8%
2. être (verb) - 6%
3. avoir (verb) - 5%
4. aller (verb) - 4%
5. faire (verb) - 3%

### Assessment
⚠️ Heavy reliance on common verbs
⚠️ Limited adjective variety
⚠️ Few adverb uses
✓ Proper noun diversity okay
✓ Concrete vocabulary decent

### Vocabulary Level Estimate
- High-frequency words: Strong (A2+)
- Mid-frequency words: Developing (A2-B1)
- Low-frequency words: Weak (<A2)
- Idioms: Very weak (<A1)

---

## Grammar Deep Dive

### Tense Usage
| Tense | Usage | Level |
|-------|-------|-------|
| Présent | Frequent, correct | B1 |
| Passé composé | Frequent, correct | B1 |
| Imparfait | Rare, some errors | A2 |
| Futur simple | None | A1 |
| Conditionnel | None | A1 |

### Mood Usage
| Mood | Usage | Level |
|------|-------|-------|
| Indicative | Dominant | B1 |
| Subjunctive | 1 instance | A2 |
| Conditionnel | None | A1 |

### Structure Analysis
- Simple sentences: 70%
- Compound sentences: 25%
- Complex sentences: 5%

### Grammar Level Estimate
**A2-B1** (70% confidence)
- Strong in present/past basics
- Missing B1 structures (subjunctive, conditionals)

---

## Listening Deep Dive

### Sample Analyzed: innerFrench Podcast

**Comprehension**:
- Topic: French work culture
- Speed: Slightly below native
- Unknown vocabulary: 15%
- Missing context: 5%

**Result**: ~75% comprehension

### Challenges Identified
1. Fast transitions between topics
2. Idiomatic expressions
3. Cultural references
4. Speaker's accent (slight Marseilles)

### Listening Level Estimate
**B1** (75% confidence)
- Can follow clear, familiar topics
- Needs support for fast/unfamiliar content

---

## Speaking Deep Dive

### From Journal to Speech Analysis

**Written complexity**: Represents likely speaking complexity
- Average sentence length: 8 words
- Subordinate clauses: 5%
- Vocabulary variety: Low

**Hypothesis**: Speaking likely A2 due to:
- Simple sentence structure
- Limited elaboration
- Basic connectors only

### Speaking Level Estimate
**A2** (60% confidence)
- Functional but limited
- Would benefit from complexity practice

---

## 📈 Progress Over Time

| Month | Vocabulary | Grammar | Listening | Speaking | Overall |
|-------|------------|---------|-----------|----------|---------|
| Jan | A2 | A1 | A2 | A1 | A2 |
| Feb | A2 | A2 | A2 | A2 | A2 |
| Mar | B1 | A2 | B1 | A2 | A2-B1 |

**Trend**: Steady improvement, grammar lagging

---

## 🎯 Next 30-Day Plan

### Week 1-2: Subjunctive
- Learn 10 subjunctive triggers
- Practice: 5 sentences daily
- Target: Use in journal naturally

### Week 2-3: Conditionals
- Learn basic si-clauses
- Practice: Transform sentences
- Target: 2 conditionals in journal daily

### Week 3-4: Listening Intensity
- Increase podcast speed to 1x
- Add: 10 min daily France Info
- Target: 80% comprehension at normal speed

### Daily
- Journal with 1 subjunctive
- Review 10 new vocabulary items
- 15 min listening

---

## Resources Recommended

### For Subjunctive
- Course: French Subjunctive Mastery
- Deck: Subjunctive Triggers

### For Listening
- Podcast: innerFrench (B1)
- Podcast: Coffee Break French (A2-B1)

### For Vocabulary
- Focus: Idioms and expressions
- Method: Frequency-based learning