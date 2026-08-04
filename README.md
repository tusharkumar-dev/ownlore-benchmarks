# OwnLore-RAG Benchmarks

Question sets used to evaluate the retrieval and answer-generation quality of [OwnLore-RAG](https://github.com/tusharkumar-dev/ownlore-rag) — an open-source RAG (Retrieval-Augmented Generation) assistant.

This repository exists so the evaluation results published in the main OwnLore-RAG README can be independently reproduced rather than taken at face value.

---

## What's Here

- **500 questions** total
- **10 books**, spanning Computer Science, Machine Learning, Medicine, Physics, History, Psychology, Finance, and Self-Improvement
- **50 questions per book**
- Plain text format — one question per line, no answers or metadata included

## Structure

```
questions/
├── Atomic Habits Original.txt
├── Bailey_and_Love's_Short_Practice_of_Surgery_28th_Edition_1.txt
├── Black Holes and Time Warps - Kip Thorne.txt
├── Hands-on-Machine-Learning.txt
├── Ikigai _ the Japanese secret to a long and happy life.txt
├── Introduction to Algorithms-The MIT Press (2022).txt
├── Operating System Concepts.txt
├── Sapiens-A-Brief-History-of-Humankind.txt
├── The psychology of money - Morgan Housel; Harriman House.txt
└── Thinking, Fast and Slow - Daniel Kahneman.txt
```

Each file name corresponds to the source book the questions were written against. Each file contains 50 plain-text questions, one per line.

## Books &amp; Categories

| Book | Category |
|---|---|
| Atomic Habits | Self-Improvement |
| Bailey & Love's Short Practice of Surgery | Medicine |
| Black Holes and Time Warps | Physics |
| Hands-On Machine Learning | Machine Learning |
| Ikigai | Self-Improvement |
| Introduction to Algorithms (CLRS) | Computer Science |
| Operating System Concepts | Computer Science |
| Sapiens | History |
| The Psychology of Money | Finance |
| Thinking, Fast and Slow | Psychology |

## How These Are Used

Each question is run through the OwnLore-RAG pipeline against the corresponding source book, and the generated answer is graded for correctness, completeness, relevance, and hallucination. Full methodology and results are documented in the [OwnLore-RAG README](https://github.com/yourusername/ownlore-rag#evaluation) under the Evaluation section.

## Reproducing the Evaluation

1. Clone this repository.
2. Ingest the corresponding source book into OwnLore-RAG.
3. Run each question from that book's `.txt` file through the app (RAG Mode) and record the answer.
4. Compare against your own grading criteria, or the methodology described in the main repo.

These files intentionally contain only questions — no answer key is provided.
