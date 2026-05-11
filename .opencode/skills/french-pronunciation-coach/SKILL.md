---
name: french-pronunciation-coach
description: Provide detailed French pronunciation analysis for words and sentences. Cover IPA, liaison rules, nasal vowels, common mistakes for Chinese speakers, and shadowing tips. Future: integrate with Whisper, ElevenLabs, TTS for audio comparison.
license: MIT
compatibility: Works with any French word or sentence
metadata:
  author: user
  version: "1.0"
---

# French Pronunciation Coach

Detailed French pronunciation analysis with IPA, rules, and techniques specifically helpful for Chinese speakers.

## Input Types

Process these inputs:
- Single word: "beaucoup", "jour", "pain"
- Phrase: "je suis français"
- Sentence: "Il fait beau aujourd'hui"
- Full sentence for connected speech

## Workflow

### 1. IPA Transcription

Provide accurate IPA pronunciation:
- Standard French (Parisian)
- Note any variations (France vs Quebec if notable)

### 2. Liaison Analysis

Identify liaison contexts:
- When to link final consonant to next word
- Forbidden liaisons
- Optional liaisons
- Liaison changes meaning

### 3. Nasal Vowel Explanation

Explain nasal vowel rules:
- When /ɑ̃/ /ɔ̃/ /ɛ̃/ /œ̃/ appear
- When nasalization is lost before consonant
- Common confusions

### 4. Pronunciation Techniques

Provide practical tips:
- Tongue position
- Lip rounding
- Stress patterns
- Connected speech flow

### 5. Common Mistakes for Chinese Speakers

Identify typical errors:
- Vowel confusions (u vs ou, é vs è)
- Final consonants (add vs drop)
- Nasal vowels (not English nasality)
- R sound (uvular vs alveolar)
- Stress pattern (French is more even)

### 6. Shadowing Prompts

Guide for practice:
- Slow version breakdown
- Natural speed
- Key rhythm points
- Focus areas

## Output Format

```markdown
# beaucoup

**IPA**: /boku/

## Liaison
No liaison - ends in /ku/ (not a consonant that triggers liaison)

## Nasal Vowels
Not a nasal vowel - watch for "beau" /bo/ becoming nasal in "beaucoup"

## Pronunciation Tips
- /b/ - bilabial stop, same as English
- /o/ - rounded back vowel, NOT /əʊ/ or /u/
- /ku/ - ends with clear /k/ + /u/, NOT "coop"

## Common Mistakes for Chinese Speakers

❌ /beɪkuːp/ - English "beautiful" influence
✅ /boku/ - pure French /o/ (between English /o/ and /ɔ/)

### Why This Is Hard
- French /o/ is a monophthong, not a diphthong
- Chinese "ou" in "buke" is closer but not identical
- Practice: round lips, hold the vowel steady

## Shadowing Guide

**Slow**: be-au-coup /bə.o.ku/
**Natural**: /boku/
**Key**: Keep /o/ steady, no glide to /u/

**Focus**: Don't add English "p" at end - the /ku/ ends cleanly
```

### Full Sentence Example

```markdown
# Il fait beau aujourd'hui

**IPA**: /il fɛ bo o.ʒɔʁ.dɥi/

## Word-by-Word

| Word | IPA | Notes |
|------|-----|-------|
| il | /il/ | Final /l/ usually pronounced |
| fait | /fɛ/ | Final /t/ not pronounced |
| beau | /bo/ | No liaison before consonant |
| aujourd'hui | /o.ʒɔʁ.dɥi/ | 4 syllables, liaison possible |

## Liaison
- "il fait beau" - no liaison (fait ends in /ɛ/, liaison optional but rare)
- "beau aujourd'hui" - no liaison

## Connected Speech
- /il fɛ bo/ → [ilfɛbo] - fluid connection
- /o.ʒɔʁ.dɥi/ → [oʒɔʁdɥi] - common linking

## Nasal Vowels
- /ɔ̃/ in "aujourd'hui" - nasal "o"
- NOT: English "on" - French /ɔ̃/ is more open

## Common Mistakes

❌ /ɪl feɪt biu/ - English "fair" + "beautiful" blend
✅ /il fɛ bo/ - distinct French sounds

❌ /ɔː.dʒɔː.dʒiː/ - English "bird" influence on "aujourd'hui"
✅ /o.ʒɔʁ.dɥi/ - nasal + uvular R + y glide

### Top 3 Errors for Chinese Speakers
1. Adding final consonants (drop /t/ in "fait", /r/ in "court")
2. Using English "r" - need uvular /ʁ/
3. Stressing words like English - French is flatter

## Shadowing Practice

**Step 1 - Segment**: il / fait / beau / aujourd'hui
**Step 2 - Slow**: i-l fɛ b o o-ʒɔʁ-dɥi
**Step 3 - Connect**: "il fait" flows together, "aujourd'hui" as one unit
**Step 4 - Natural**: /il fɛ bo o.ʒɔʁ.dɥi/

**Focus**: The /dɥi/ ending - "d" followed by y-glide /ɥ/
```

## Sound System Reference

### Vowels (Oral)

| IPA | Example | Chinese Equivalent |
|-----|---------|---------------------|
| /a/ | chat | "a" in "ma" |
| /e/ | café | "ei" in "bei" |
| /ɛ/ | sel | between "e" and "ai" |
| /i/ | si | "i" in "mi" |
| /o/ | eau | between "o" and "u" |
| /ɔ/ | chat | open "o" |
| /u/ | Roux | "u" in "du" |
| /y/ | rue | round "i" - unique to French |
| /ə/ | le | schwa - reduced |
| /œ/ | sœur | round "e" |

### Nasal Vowels

| IPA | Example | English Approximation |
|-----|---------|----------------------|
| /ɑ̃/ | grand | "on" in "wrong" |
| /ɔ̃/ | bon | "on" in "song" |
| /ɛ̃/ | vin | "an" in "bank" (nasal) |
| /œ̃/ | brun | "un" in "lung" (nasal) |

### Consonants

| IPA | Example | Notes |
|-----|---------|-------|
| /ʁ/ | rouge | Uvular R - key for French sound |
| /ɲ/ | montagne | Palatal nasal |
| /ʒ/ | jour | "s" in "measure" |
| /ʃ/ | chat | "sh" in "ship" |
| /ŋ/ | parking | Only in borrowed words |

## Special Topics

### Liaison Rules

| Context | Example | Liaison? |
|---------|---------|----------|
| After singular noun | les ami**s** | ✅ Required |
| After verb (3rd pers) | il**z** habitent | ✅ Required |
| After et | et**z** autres | ✅ Optional |
| After /ʁ/ | premier**z** | ❌ Forbidden |
| After /ʃ/ /ʒ/ | huit**z** | ❌ Forbidden |
| Before on/une | un**z** enfants | ❌ Forbidden |

### Silent Final Consonants

| Letter | Silent When... | Exception |
|--------|----------------|------------|
| -s | most words | liaison, plural |
| -d | most words | sud,ied |
| -x | many words | six, dix, flux |
| -t | many words | -tion, dot, brut |
| -p | après, beaucoup | cap, sud |

### The /y/ Vowel (Critical for Chinese)

- French /y/ does NOT exist in Mandarin
- Shape: Round lips like "o" AND hold tongue like "i"
- Practice: Say "ee" then slowly round lips without changing tongue
- Example: "tu" /ty/ - not "too" but round-lipped "tee"

## Common Patterns by Level

### A1-A2 Pitfalls
- Final consonants (p, t, s, x often silent)
- /e/ vs /ɛ/ confusion
- Word stress (flat in French)
- "r" pronunciation

### B1-B2 Challenges
- Nasal vowels in context
- Liaison in connected speech
- /ə/ schwa dropping
- /ɲ/ vs /nj/

### C1-C2 Refinement
- /ø/ vs /œ/ distinction
- Semi-vowels /ɥ/ /j/ /w/
- Intonation patterns
- Regional variations

## Future Integrations

When available, integrate:
- **Whisper**: Transcribe user's audio for comparison
- **ElevenLabs**: Generate native audio samples
- **TTS**: Practice with speech synthesis
- **Audio Comparison**: Side-by-side user vs native

## Guidelines

- Always explain WHY (not just what)
- Provide Chinese-specific guidance
- Include IPA for every word
- Give actionable shadowing steps
- Mark common errors clearly
- Note regional variations if relevant
- Make it practical for daily practice