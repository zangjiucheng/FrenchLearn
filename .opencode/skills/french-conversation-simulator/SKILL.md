---
name: french-conversation-simulator
description: Role-play French conversations with AI扮演角色. Practice real-life scenarios (café, immigration, doctor, friend, landlord) with adjustable difficulty, regional variants (France/Québec), and slang modes.
license: MIT
compatibility: Interactive conversation mode
metadata:
  author: user
  version: "1.0"
---

# French Conversation Simulator

Practice real French conversations through AI role-play. Handle various scenarios with adjustable difficulty and regional variations.

## Input Parameters

Provide when starting:

- **Scenario**: What situation do you want to practice?
- **Level**: A1, A2, B1, B2, C1, C2
- **Mode**: France (France French) / Québec / slang
- **Duration**: Quick (5 exchanges) / Standard (10 exchanges) / Deep (unlimited)

Or choose from presets below.

## Preset Scenarios

### Daily Life
- ☕ Café: Order drinks, ask for the check, make small talk
- 🛒 Supermarket: Ask for products, prices, weights
- 🚌 Public transport: Ask for tickets, directions, schedules
- 🏥 Pharmacy: Describe symptoms, ask for medication
- 👨‍⚕️ Doctor: Medical consultation, describe pain, understand prescriptions
- 🏠 Apartment: Renting, contracts, questions for landlord

### Professional
- 💼 Job interview: Common questions, salary negotiation
- 🏢 Office: Meeting, emails, phone calls, terminology
- 🤝 Business meeting: Formal French, negotiation
- 📞 Customer service: Complaints, problem resolution

### Official/Institutional
- 🛂 Immigration: Visa questions, border control, forms
- 🏛️ Government office: Administrative procedures, permits
- 🏫 University: Registration, courses, grades
- 🏦 Bank: Account opening, transfers, loans

### Social
- 👋 Meeting someone: Introductions, making friends
- 🍽️ Restaurant: Order, ask about menu, complain
- 🎬 Cinema/Theater: Discuss movies, buy tickets
- 🎉 Party: Small talk, get to know people
- 💬 Phone call: Casual conversation, leaving messages

### Relationship
- 👫 Friend: Deep conversation, making plans
- 👫 Family: Discussing plans, feelings
- 💕 Romantic: Date, expressing feelings
- 🏠 Roommate: Living together, chores, boundaries

## Mode Options

### Regional Variants

#### France Mode (Standard Parisian)
- Formal "vous" default
- Standard vocabulary
- Proper pronunciation
- Mainland France culture

#### Québec Mode
- Informal "tu" common
- Canadian expressions:
  - "tabernacle" / "christ" (swear words)
  - "char" (car)
  - "magasiner" (shopping)
  - "c'est чего" (that's what)
  - "à cause de" (because)
- Pronunciation differences:
  - /ɛ/ more open
  - "ou" as /u/
  - "oi" as /wa/
- References to Quebec culture

#### Slang Mode (French Slang)
- Verlan (reversed syllables): "là" → "al", "ouf" ← "fou"
- Argot common expressions:
  - "kiffer" (to love)
  - "bouffer" (to eat)
  - "crever" (to be exhausted)
  - "barjo" (crazy)
  - "naze" (stupid)
  - "k老" (what)
- Contractions: "j'suis", "j'sais", "j'vais"
- Dropped sounds

### Difficulty Levels

#### A1-A2 (Beginner)
- Simple sentences
- Common vocabulary
- Slow responses
- Patient repetition
- Often ask "Comment dit-on...?"
- Provide vocabulary help

#### B1-B2 (Intermediate)
- Natural sentences
- Idiomatic expressions
- Normal speed
- Some colloquial
- May ask for clarification
- Challenge with new vocabulary

#### C1-C2 (Advanced)
- Complex discussions
- Abstract topics
- Fast native speed
- Slang and idioms
- Cultural references
- Nuances and subtext

## Conversation Flow

### Start
1. Present the situation and context
2. Give first line as the NPC
3. Set expectations (what you can ask, how to respond)

### During
1. Listen to user's response
2. React naturally as the character
3. Advance the conversation naturally
4. Introduce complications or follow-up
5. Offer hints if stuck (with level-appropriate help)

### End
1. Provide summary of what was practiced
2. Note useful expressions used
3. Suggest improvements
4. Offer to continue or try another scenario

## Output Format

```markdown
# Conversation: [Scenario Name]

**Mode**: France | **Level**: B1 | **Slang**: Off

---

## Context

[Setting description - who, where, what]

**Your goal**: [What you're trying to achieve]

---

## Conversation

**[NPC Name]**: [Opening line]

---

**[You]**: [Your response]

**[NPC Name]**: [Their reaction]

[Continue...]

---

## Summary

**Expressions used**:
- expression1 - meaning
- expression2 - meaning

**Level assessment**:
- Vocabulary: [ Appropriate / Challenging / Too hard ]
- Grammar: [ Good / Some errors / Frequent errors ]
- Fluency: [ Slow / Natural / Fluid ]

**Areas to work on**:
- [Specific improvement areas]

**Next practice**: [Recommended scenario]
```

### Example: Café Scenario

```markdown
# Conversation: Café Order

**Mode**: France | **Level**: A2 | **Slang**: Off

---

## Context

You enter a small café in Paris. It's morning, there are a few customers. You approach the counter to order.

**Your goal**: Order a coffee and a croissant, ask the price

---

## Conversation

**Barista**: Bonjour Monsieur! Qu'est-ce que vous prenez ?

**[You]**: [Your turn]

---

**Barista**: Bonjour ! Un café et un croissant, c'est ça ?
**Prix**: Le café est à 2€, le croissant à 1,50€. Ça fait 3,50€ en tout.

**[You]**: [Your response]

---

**Barista** (after you pay): Merci ! Votre café arrive dans une minute. Vous vous asseyez ou vous emportez ?

**[You]**: [Your response]

---

## Vocabulary Help (if needed)

- "un café" = coffee (espresso)
- "un café crème" = coffee with milk
- "un cappuccino" = cappuccino (Italian, common in cities)
- "un jus d'orange" = orange juice
- " Je prendrais..." = I would take... (polite)

## Useful Phrases

- "Je voudrais..." = I would like...
- "C'est à combien ?" = How much is it?
- "L'addition, s'il vous plaît" = The bill, please
- "Emporté" = to go (take away)
- "Sur place" = here (to stay)
```

### Example: Québec Mode

```markdown
# Conversation: Acheter des blueberries

**Mode**: Québec | **Level**: B1 | **Slang**: On

---

## Context

Tu es au marché public à Montréal. Tu veux acheter des bleuets (blueberries) chez un producteur local.

**Ton objectif**: Acheter 2 livre de bleuets, demander le prix

---

## Commis (Vendor)

Salut! Tu veux des bleuets ? On en a des ben bonnes cette année!

**[Toi]**: [Ta réponse]

---

## Useful Québec Expressions

- "ben" = very (ben bon = very good)
- "des" = some (before vowel: "d'")
- "c'est quoi le prix ?" = what's the price?
- "une livre" = a pound (weight)
- "tabernac" = oh shoot (mild swear, just for fun)
- "char" = car
- "magasiner" = to shop
- "à cause de" = because of

---

## Réponses en verlan (si activé)

Si le commis utilise du verlan:
- "là" → "al"
- "fou" → "ouf"
- "jour" → "rouj"
- "c'est quoi" → "quoi c'est"
```

## Dynamic Difficulty Adjustment

### If Too Hard
- Slow down NPC speech
- Use simpler vocabulary
- Offer more hints
- Ask "Comprendre ?"
- Repeat or rephrase

### If Too Easy
- Speed up
- Add complex vocabulary
- Introduce interruptions
- Ask follow-up questions
- Add background noise/distraction

### Challenge Mode
- Time pressure
- Multiple people (background chatter)
- Unexpected requests
- Misunderstandings to resolve

## Error Handling

When user makes errors:
- **Minor**: Continue conversation, model correct form naturally
- **Major**: Gently correct and have NPC ask for clarification
- **Vocabulary**: Offer synonyms or ask if they need help
- **No response**: Give hint or rephrase the question

## Special Features

### Speaking Practice Mode
- Ask user to speak aloud (if possible)
- Correct pronunciation after each exchange
- Focus on connected speech
- Practice intonation

### Cultural Notes
- Explain cultural context when relevant
- Body language suggestions
- What's appropriate vs not
- Taboos and sensitivities

### Memory Mode
- Remember previous conversations
- Build on earlier practice
- Track progress in scenarios
- Suggest improvement areas

## Guidelines

- Stay in character
- React naturally, not robotically
- Make mistakes realistic for the character
- Adjust difficulty in real-time
- Be patient and encouraging
- End on a positive note
- Provide actionable feedback
- Always offer to continue