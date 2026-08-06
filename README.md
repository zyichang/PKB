# PKB — Personal Knowledge Base

A personal knowledge base for capturing **knowledge points** (知识点) as markdown files.

## What is this repository?

Whenever I learn something worth remembering, I record it here as a knowledge point:

- **A problem I solved at work.** I hit a problem, researched it, and finally fixed it — the solution is a knowledge point.
- **Something I learned from a book or course.** I come across a math formula, a data-structure concept, a circuit-theory principle — once I understand it, it's a knowledge point.
- **Something I forgot or need to review.** Anything I don't know yet, or keep forgetting, gets written down so I can study it again.

Each knowledge point becomes a markdown file. The markdown is written in a format that can later be turned into **Anki** flashcards (see `DocforAnki/`), so the same notes serve both as a reference and as spaced-repetition review material.

## How a knowledge point flows in

```
Encounter  →  Research / Learn  →  Understand  →  Record as markdown  →  (optional) Turn into Anki cards
```

## Structure

```
PKB/
├── README.md                 # this file
├── DocforAnki/               # existing Anki decks + source docs (math, 数据结构)
├── Math/                     # 数学
├── DataStructure/            # 数据结构
├── CircuitTheory/            # 电路原理
├── Miscellaneous/            # 杂项 — things I don't yet know how to split or sort
└── templates/
    └── knowledge-point.md    # reusable template for a single knowledge point
```

- **One subject per top-level folder.** Add a new folder when you start a new course or topic.
- **`Miscellaneous/`** is the catch-all: when a knowledge point doesn't clearly belong to a subject, or you haven't decided how to sort it, put it here. Move it out later once its home is clear.
- **`DocforAnki/`** holds the decks and source material already prepared for Anki import.
- **`templates/`** keeps the standard shape of a knowledge point so every note looks the same.

## File naming

Use short, descriptive, lowercase-with-hyphens names, optionally prefixed by topic:

```
Math/limits-l-hopital-rule.md
DataStructure/red-black-tree-rotation.md
CircuitTheory/thevenin-equivalent.md
Miscellaneous/git-detached-head-recovery.md
```

## Managing your knowledge

1. When you learn or solve something, copy `templates/knowledge-point.md`.
2. Fill in the question, the answer, and any details/examples.
3. Save it under the right subject folder (or `Miscellaneous/` if unsure).
4. When you have enough related notes, batch them into an Anki deck under `DocforAnki/`.
