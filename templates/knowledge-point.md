---
# Quizify Card Markdown — import directly with the Anki Quizify add-on.
# Everything under `quizify:` configures the whole file.
quizify:
  format: 1
  deck: Subject            # e.g. Math, DataStructure, CircuitTheory, Miscellaneous
  tags: [topic]            # tags cannot contain spaces
---

+++
<!-- quizify-card
tags: [extra-tag]
draft: false
-->
# The question — what you didn't know, in your own words

Optional extra context, a code snippet, or the exact prompt you asked.
***
# Answer

The concise core answer — keep it flashcard-sized.

::: Details
The deeper "why": derivation, edge cases, gotchas.
:::

**Reference:** <link or source>

+++
<!-- A second card as a cloze deletion. Wrap the hidden part in double braces. -->
Binary search runs in {{O(log n)}} time because each step halves the range.
***
Each comparison discards half of the remaining elements.

+++
<!-- A third card as a single-choice question (one letter after ;;; = single choice). -->
Which layer does the TCP three-way handshake belong to?

;;;
A. Application
B. Transport
C. Network
;;;B
***
The handshake establishes a transport-layer connection before data transfer.
