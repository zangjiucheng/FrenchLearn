---
name: french-weekly-review
description: Automatically summarize weekly French learning progress. Track vocabulary stats, identify repeated errors, recommend review content, and detect forgetting points for long-term retention.
license: MIT
compatibility: Requires learning data input
metadata:
  author: user
  version: "1.0"
---

# French Weekly Review Agent

Automate your French learning review. Get weekly summaries, track progress, and identify areas needing reinforcement.

## Input

Provide one or more:
- Flashcard review data (spaced repetition stats)
- Writing corrections from the week
- Vocabulary learned (new words)
- Sentence mining results
- Listening/watching time
- Speaking practice notes
- Journal entries

Or grant access to your learning vault/databases.

## Workflow

### 1. Summarize This Week's Learning

**Quantities**:
- New vocabulary learned
- Sentences mined
- Writing corrections reviewed
- Listening/watching hours
- Speaking practice time
- Cards reviewed vs new

**Quality**:
- Completion rate
- Accuracy trends
- Streak data

### 2. Vocabulary Statistics

**Breakdown by**:
- Level distribution (A1-A2, B1-B2, C1-C2)
- Category (noun, verb, adjective, expression)
- Source (video, reading, conversation)

**Trends**:
- Words added this week vs last
- Most common categories
- Domain vocabulary (travel, work, etc.)

### 3. Identify Repeated Errors

From writing corrections and practice:
- Grammar patterns missed
- Vocabulary confusion
- Pronunciation issues
- Preposition mistakes
- Gender errors

**Pattern Analysis**:
```
This Week's Error Patterns:
├── Verb: Subjunctive triggers (3 times)
├── Preposition: "à" vs "de" after verbs (5 times)
├── Gender: "le problème" vs "la problème" (2 times)
└── Pronunciation: /y/ vs /u/ (4 times)
```

### 4. Recommend Review Content

Based on:
- Spaced repetition due dates
- Error patterns
- Forgetting curve

**Priority**:
- High: Items due + error patterns
- Medium: Items due this week
- Low: Future reviews

### 5. Detect Forgetting Points

**Symptoms**:
- "Knew it yesterday, forgotten today"
- Recognition but no production
- Confused between similar words
- Grammar rules that won't stick

**Forgetting Detection**:
- Review success rate < 70%
- Same card failed multiple times
- Words in "learning" phase too long
- Gap between recognition and production

## Output Format

```markdown
# French Weekly Review - Week [X]

**Date**: [Start] - [End]

---

## 📊 Learning Summary

| Metric | This Week | vs Last Week |
|--------|-----------|--------------|
| New vocabulary | 45 | +12 |
| Sentences mined | 8 | +3 |
| Writing corrections | 12 | -2 |
| Listening hours | 5.5 | +1.5 |
| Speaking practice | 45 min | +15 min |
| Flashcards reviewed | 156 | +34 |
| New cards added | 52 | +10 |

**Streak**: 7 days 🔥

---

## 📈 Vocabulary Statistics

### By Level
- A1: 15 (33%)
- A2: 18 (40%)
- B1: 10 (22%)
- B2: 2 (5%)

### By Type
- Nouns: 20 (44%)
- Verbs: 12 (27%)
- Expressions: 8 (18%)
- Adjectives: 5 (11%)

### Source
- YouTube: 18
- Podcast: 12
- Reading: 10
- Conversation: 5

---

## ⚠️ Repeated Errors

### Top Error Patterns

| Error Type | Frequency | Priority |
|------------|-----------|----------|
| Subjunctive after "il faut que" | 4 | 🔴 High |
| Preposition "à" vs "de" | 5 | 🔴 High |
| Gender: le/la words | 3 | 🟠 Medium |
| Pronunciation: /y/ sound | 4 | 🟠 Medium |
| Passé composé vs Imparfait | 2 | 🟡 Low |

### Specific Issues

**Subjunctive triggers**:
- ❌ "Il faut que tu viens" → ✅ "Il faut que tu viennes"
- ❌ "Je veux que tu fais" → ✅ "Je veux que tu fasses"

**Prepositions**:
- ❌ "payer avec carte" → ✅ "payer avec la carte"
- ❌ "arriver à" (time) → ✅ "arriver à" sometimes wrong

---

## 🎯 Review Recommendations

### Priority 1 - Due Now + Errors
- 23 cards (subjunctive, prepositions)
- 8 grammar rules to reinforce

### Priority 2 - This Week
- 45 cards in review
- 15 new cards close to graduation

### Priority 3 - Maintenance
- 89 cards in learning
- 12 "young" cards needing more reps

---

## 🧠 Forgetting Detection

### At-Risk Items

| Word/Pattern | Failed | Last Seen | Action |
|--------------|--------|-----------|--------|
| se rendant compte | 3x | 3 days ago | Re-learn |
| subjunctive after fear | 2x | 5 days ago | Review rule |
| avoir peur que | 2x | 4 days ago | Add examples |

### Warning Signs
- 12 cards in "learning" > 10 days
- 3 grammar patterns re-appearing in errors
- Vocabulary recognition up, production down

### Recommended Actions
1. Re-review subjunctive triggers tonight
2. Add 5 more example sentences for "avoir peur que"
3. Change 12 "learning" cards to "review" mode
```

### Focus Area Recommendations

```markdown
## 🎯 Next Week Focus

### Recommended Focus
1. **Subjunctive triggers** - Daily 5 minutes
2. **Preposition patterns** - 10 sentences
3. **Gender habits** - New cards, mark clearly

### Suggested Materials
- Grammar: French Subjunctive Triggers deck
- Practice: Writing correction review
- Listening: "Il faut que" in native content

### Time Allocation
- Review: 15 min/day (maintain)
- New: 10 min/day (reduce to focus on review)
- Error correction: 10 min/day (increase)
```

## Long-Term Tracking

### Monthly Trends
- Vocabulary grown: [number]
- Accuracy improvement: [percentage]
- Time invested: [hours]
- Areas improved: [list]
- Areas regressing: [list]

### Quarterly Goals
- Current level estimate
- Distance to next level
- Recommended adjustments

## Automation Setup

For automated weekly reviews:
- Connect to Obsidian vault
- Connect to Anki stats
- Connect to learning logs
- Schedule: Every Sunday evening

### Data Sources to Track
- Anki: Review logs, new cards, retention rate
- Obsidian: Flashcards, vocabulary notes
- Logs: Listening time, speaking practice
- Corrections: Writing, speaking errors

## Guidelines

- Be specific about numbers
- Focus on actionable insights
- Balance positive and improvement areas
- Prioritize error patterns
- Detect forgetting early
- Make recommendations concrete
- Keep it encouraging but honest