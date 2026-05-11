---
name: french-daily-immersion
description: Generate a daily French immersion package tailored to user level. Include a short video, podcast, article, meme, and expression with learning notes.
license: MIT
compatibility: Requires user level preference and interests
metadata:
  author: user
  version: "1.0"
---

# French Daily Immersion Generator

Generate a curated daily French learning package with diverse content sources matched to user's level and interests.

## Input

- **Current level**: A1, A2, B1, B2, C1, or C2
- **Interests** (optional): news, culture, humor, tech, travel, food, sports, etc.
- **Time available**: 5 min / 15 min / 30 min / 1 hour

## Workflow

### 1. Video Selection

Find a short video (1-5 min) appropriate for level:
- YouTube short
- News clip
- Cultural snippet
- Tutorial

**For each video, provide:**
- Title and link
- Why it's good for your level
- 3 new vocabulary items
- 1 pattern to notice

### 2. Podcast Selection

Recommend a podcast episode or segment:
- News summary (1-3 min)
- Conversation snippet
- Storytelling excerpt

**For each podcast, provide:**
- Podcast name and episode
- Level appropriateness
- Key listening focus (numbers, names, opinions, etc.)
- Transcript timestamp for review

### 3. Article Selection

Suggest a short read (100-300 words):
- News headline
- Blog post
- Social media long-form

**For each article, provide:**
- Title and source
- Reading time
- 5 key vocabulary items
- 1 sentence structure to notice

### 4. Meme/Social Content

Find something entertaining:
- French meme
- Tweet/X post
- Instagram caption
- TikTok text

**For each, provide:**
- Content with translation
- Slang/colloquial expression used
- Why it's culturally relevant

### 5. Expression of the Day

Provide one valuable expression:
- Idiomatic phrase
- Useful connector
- Verbal phrase

**For each, provide:**
- The expression
- Meaning and usage
- Example in context
- Related expressions

## Output Format

```markdown
# Daily French Immersion - [DATE]

**Your Level**: B1 | **Time**: 15 min

---

## 🎬 Video (3 min)

**Title**: [Video Title]
**Source**: YouTube/France.tv/other
**Link**: [URL]

**Why this works**: [Level-appropriate explanation]

**Vocabulary to note**:
- mot1 - meaning
- mot2 - meaning
- mot3 - meaning

**Pattern to notice**: [Grammar/structure in the video]

---

## 🎧 Podcast (5 min)

**Name**: [Podcast Name]
**Episode**: [Title or number]
**Link**: [URL]

**Listening focus**: What to listen for

**For review** (transcript): [timestamp]

---

## 📖 Article (5 min read)

**Title**: [Article Title]
**Source**: [Le Monde/01net/other]
**Link**: [URL]

**Key vocabulary**:
- mot1
- mot2
- mot3
- mot4
- mot5

**Structure to notice**: [Sentence pattern]

---

## 😂 Meme/Social

**Content**: [Text/description]
**Translation**: [English]

**Colloquial**: [Expression used]

**Cultural note**: [Why this is funny/relevant]

---

## 💬 Expression of the Day

**Expression**: [French phrase]

**Meaning**: [English]

**Usage**: [When to use this]

**Example**: [Example sentence]

**Related**: [Similar expressions]
```

### Example Output

```markdown
# Daily French Immersion - 2024-01-15

**Your Level**: B1 | **Time**: 15 min

---

## 🎬 Video (2 min)

**Title**: Comment faire un café parfait
**Source**: YouTube - French Coffee Academy
**Link**: [youtube link]

**Why this works**: Simple imperatives, practical vocabulary, clear visuals

**Vocabulary to notice**:
- torréfier - to roast (coffee beans)
- l'extraction - extraction
- la mouture - grind (noun)

**Pattern to notice**: "Il faut + infinitif" structure for instructions

---

## 🎧 Podcast (4 min)

**Name**: Le journal en français facile
**Episode**: 15 janvier 2024
**Link**: [TV5Monde link]

**Listening focus**: Numbers, dates, places

**For review**: 1:30-2:45 (weather report section)

---

## 📖 Article (3 min read)

**Title**: Les Français boivent moins de vin
**Source**: Le Figaro
**Link**: [lefigaro link]

**Key vocabulary**:
- la consommation - consumption
- en baisse - declining
- les jeunes - young people
- le marché - market
- la tendance - trend

**Structure to notice**: "de plus en plus" / "de moins en moins" comparisons

---

## 😂 Meme

**Content**: "Moi: Il faut que je dorme tôt ce soir | Mon cerveau: Tu te souviens de 2009?"
**Translation**: "Me: I should go to bed early tonight | My brain: Do you remember 2009?"

**Colloquial**: "Il faut que" (informal: "faut que")

**Cultural note**: Relatable French internet humor about insomnia

---

## 💬 Expression of the Day

**Expression**: C'est la cerise sur le gâteau

**Meaning**: The cherry on top (the final touch that makes everything perfect)

**Usage**: When something already good becomes even better

**Example**: "Le repas était excellent, et le dessert était la cerise sur le gâteau."

**Related**: "C'est le bouquet" (the finale), "Faire le point" (to sum up)
```

## Content Sources

### Video
- YouTube: French learning channels (innerFrench, Oui à la France)
- France.tv short clips
- TikTok French creators
- Yandex Zen articles as video

### Podcast
- TV5Monde Journal en français facile
- Coffee Break French (various levels)
- InnerFrench Podcast
- French for Today
- Learning Spanish: InnerFrench, Coffee Break French

### Article
- Le Monde simplify (lemondedimanche)
- 01net (tech)
- Slate.fr (culture)
- Le Bonbon (urban culture)
- Paris Match (general)

### Meme/Social
- @memepediafr (X/Twitter)
- French TikTok comments
- r/FrenchMemes subreddit
- @french_people (Instagram)

### Expression Sources
- Langue Française dictionary
- French expression websites
- Native speaker usage patterns

## Level Guidelines

### A1-A2
- Focus: Basic phrases, everyday vocabulary
- Content: Short, visual, repetitive
- Length: 1-3 min for audio/video

### B1-B2
- Focus: Nuance, opinion, storytelling
- Content: Intermediate podcasts, news
- Length: 3-8 min for audio/video

### C1-C2
- Focus: Idioms, abstract topics, nuance
- Content: Native content without simplification
- Length: 5-15 min for audio/video

## Automation Notes

This skill can be semi-automated:
1. Maintain a curated list of sources per level
2. Rotate through content types
3. Pre-fill templates with new content
4. User fills in personalization

### Future Enhancements
- RSS feed integration for automatic article selection
- YouTube API for video recommendations
- Podcast directory API
- ML-based content matching to user level
- Spaced repetition integration for vocabulary

## Guidelines

- Variety: Mix content types each day
- Level-appropriate: Don't frustrate with too-hard content
- Engaging: Include at least one fun/light item
- Actionable: Give specific things to notice
- Repeatable: Structure that works for daily use