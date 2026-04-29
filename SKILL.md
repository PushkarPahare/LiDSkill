---
name: leben-in-deutschland
description: |
  Study guide and quiz for the German "Leben in Deutschland" citizenship test (300 questions).
  Use when the user asks to study, quiz, practice, or take a test for the Leben in Deutschland,
  Einbürgerungstest, or Orientierungskurstest.
tags: [german, citizenship, test-prep, quiz]
version: 1.0.0
---

# Leben in Deutschland

## Overview

Study companion for the German "Leben in Deutschland" test covering all 300 federal questions. Provides narrative study guides per category and quiz/test modes using the original PDF as question source.

## Usage

Use this skill when:
- User asks to study, quiz, or practice for the "Leben in Deutschland" test
- User mentions Einbürgerungstest or Orientierungskurstest
- User wants to review a specific topic (e.g. Grundrechte, Wahlen, Geschichte)

## Test Format

- 33 questions randomly selected from 300
- 60 minutes
- 15 correct = pass
- 17 correct = Einbürgerung credit
- 4 options per question, exactly 1 correct

## Category Index

| # | Category | Fragen | Questions | Study Guide |
|---|----------|--------|-----------|-------------|
| 1 | Staat & Verfassung | 83 | 1-4,6-20,22,24-28,30-32,34,37-39,41-44,48-49,51-55,57-58,60-61,63-65,67,70-72,74-75,80-91,98,101,129,135,143-145,147-148,262,274,277-278,281,289 | `references/01_Staat_und_Verfassung.md` |
| 2 | Wahlen & Beteiligung | 37 | 5,59,62,73,76,78-79,92-94,103,107-134 | `references/02_Wahlen_und_Beteiligung.md` |
| 3 | Staat & Gesellschaft | 36 | 21,23,29,33,35-36,40,45-47,56,66,68-69,77,95-97,99-100,105-106,131,214,216,248-249,253,255-256,259-260,265,273,282,285,288 | `references/03_Staat_und_Gesellschaft.md` |
| 4 | Recht & Alltag | 36 | 102,104,136-142,146,149-150,241-243,245-247,251-252,254,258,263,266-268,272,275-276,279-280,283,286-287,290-291 | `references/04_Recht_und_Alltag.md` |
| 5 | NS-Zeit & Nachkriegsgeschichte | 53 | 50,151-170,171-172,174-190,193,199,202-203,207-212,215,217,220 | `references/05_NS_und_Nachkriegsgeschichte.md` |
| 6 | Wiedervereinigung & Europa | 36 | 173,191-192,194-198,200-201,204-206,213,218-219,221-240,228 | `references/06_Wiedervereinigung_und_Europa.md` |
| 7 | Gesellschaft & Kultur | 19 | 244,250,257,261,264,269-271,284,292-300 | `references/07_Gesellschaft_und_Kultur.md` |

## Answer Key

Compact answer key for all 300 questions (1a = question 1 answer a):

```
001-010: d b a c c d a b c d
011-020: a c d b b a d a a d
021-030: a c d c a b b c b b
031-040: b c a c b a d b d b
041-050: a b b b a a a c b b
051-060: c a d d a b d b b b
061-070: d b b d d d d d c d
071-080: d d a c a d d c d c
081-090: d d c c c a b a c a
091-100: c d d b b b a b a a
101-110: b a b d d d b b b c
111-120: a b a b c d c d c c
121-130: a a c c b a c a c a
131-140: c b b a d b c c b a
141-150: a b a b a d b d b b
151-160: b c d b c c a a a b
161-170: a d c c a d d d c a
171-180: d d c b b c b d b c
181-190: b a b c a b d d c d
191-200: b a c a b a a c b c
201-210: b b b b a b c c d b
211-220: b c c a b a d b d d
221-230: a d c b d b b c d a
231-240: d c a d c d b b b c
241-250: b c a a d b b b b b
251-260: d a a d c d b b b d
261-270: b a a a d d a d c c
271-280: b d d b d d d a c c
281-290: b b b b d a c c c b
291-300: a c c a b c d a b a
```

Letter-to-position: a=1st option, b=2nd, c=3rd, d=4th as they appear in the PDF.

## Question Source

The original PDF is at `assets/Test_Lernkarten_Beilage_zum_Kursbuch.pdf`. Read it when you need the exact question text and options for quiz/test modes. Questions are on pages 5-30, answer key on page 31.

## Modes

### Study

User says: "study topic 3", "learn about Wahlen", "read Recht und Alltag"

1. Identify the category from the index
2. Read the corresponding study guide from `references/`
3. Present it to the user
4. Offer to quiz them on that category

### Quiz

User says: "quiz me", "quiz topic 2", "quiz Grundrechte"

1. If no category specified, ask which one (show the 7 categories)
2. Read the PDF to get question text and options for that category's question numbers
3. Pick 10 random questions from that category
4. Ask one at a time, 4 options (a/b/c/d)
5. After each answer: say correct/wrong, give the right answer, briefly explain
6. After 10: report score (e.g. "7/10")

### Test

User says: "practice test", "simulate the test", "Probetest"

1. Pick 33 random questions from all 300
2. Ask one at a time, 4 options
3. After each answer: say correct/wrong
4. After 33: report final score
   - Below 15: "Nicht bestanden. Du brauchst mindestens 15."
   - 15-16: "Bestanden! Orientierungskurstest geschafft."
   - 17+: "Bestanden! Das reicht auch für die Einbürgerung."

### Practice

User says: "practice topic 5", "I want to learn and then quiz NS-Zeit"

1. Read and present the study guide
2. Then immediately start a 10-question quiz on that category
3. For wrong answers, quote the relevant sentence from the study guide

## Rules

- Questions and options are always in German
- Explanations can be in the user's preferred language
- Never reveal the answer before the user responds
- Always show all 4 options
- Use the answer key above to check answers (don't rely on PDF parsing for correctness)
- Reference the study guide when explaining wrong answers
