# Knowledge Inbox

This document stores reusable research knowledge from my LLM-based multi-agent research sprint.

It is not a paper note file.  
It is a semi-structured and expandable knowledge collection.

Principle:

> Capture first, organize gradually.

The structure below is temporary and can be revised as my understanding of the field improves.

---

## 0. Current Knowledge Buckets

These buckets are not fixed.  
They are only used to make the current knowledge easier to browse.

---

### 0.1 Field-Level Understanding

For high-level consensus, field structure, mainstream directions, historical shifts, or general judgments about the area.

Related entries:

- 

---

### 0.2 Methods / Tricks / Design Patterns

For reusable methods, experimental tricks, prompting patterns, agent interaction designs, training strategies, or implementation choices.

Related entries:

- 

---

### 0.3 Evaluation / Benchmark Issues

For problems related to evaluation quality, baseline design, benchmark contamination, metrics, ablation, or experimental rigor.

Related entries:

- 

---

### 0.4 Open Problems / Research Gaps

For unsolved problems, weakly explored questions, unclear mechanisms, or research opportunities.

Related entries:

- 

---

### 0.5 Personal Research Ideas

For my own possible project ideas, experiment designs, hypotheses, or proposal fragments.

Related entries:

- 

---

### 0.6 Useful Comparisons

For comparing two methods, two papers, two assumptions, two research directions, or two experimental designs.

Related entries:

- 

---

### 0.7 Miscellaneous but Potentially Useful

For knowledge that feels important but does not yet fit into existing buckets.

Related entries:

- 

---

## 1. Knowledge Entries

Each entry should be short, searchable, and reusable.

Entry rules:

- One entry should capture one knowledge unit.
- Do not force a perfect category.
- Use keywords generously.
- Link to Paper IDs when possible.
- If unsure, put it under Miscellaneous first.
- Preserve Entry IDs when reorganizing this document later.

---

### E001 - [Short Title]

**Primary Bucket:**  
**Possible Secondary Buckets:**  
**Date:**  
**Source:**  
**Related Papers:**  
**Keywords:**  

**Content:**  

**Why it matters:**  

**Possible future use:**  

---

### E002 - [Short Title]

**Primary Bucket:**  
**Possible Secondary Buckets:**  
**Date:**  
**Source:**  
**Related Papers:**  
**Keywords:**  

**Content:**  

**Why it matters:**  

**Possible future use:**  

---

### E003 - [Short Title]

**Primary Bucket:**  
**Possible Secondary Buckets:**  
**Date:**  
**Source:**  
**Related Papers:**  
**Keywords:**  

**Content:**  

**Why it matters:**  

**Possible future use:**  

---

## 2. Reorganization Notes

Use this section when I notice that the current buckets are no longer enough.

---

### 2.1 Possible New Buckets

- 

---

### 2.2 Buckets That May Need Splitting

- 

---

### 2.3 Buckets That May Need Merging

- 

---

### 2.4 Entries That Need Reclassification

- 

---

## 3. AI Reorganization Prompt

When this file becomes too long or messy, use the following prompt to ask AI to reorganize it.

```text
You are helping me reorganize my research Knowledge_Inbox.md.

Context:
I am a first-year CS student preparing for a summer research internship. My current focus is LLM-based multi-agent systems, agent memory, evaluation, and RL-for-LLM-agents.

I will provide a semi-structured Knowledge_Inbox.md containing raw research knowledge entries.

Your tasks:
1. Summarize the major knowledge themes currently appearing in the file.
2. Identify whether the current buckets are still appropriate.
3. Suggest new buckets if necessary.
4. Identify buckets that should be split or merged.
5. Classify each entry into a better structure, but preserve all Entry IDs.
6. Mark entries that may support a summer research proposal, reproduction project, or cold email discussion.
7. Do not force uncertain entries into a category. Keep them as miscellaneous if needed.
8. Return a cleaner Knowledge_Map.md structure that I can copy and use.

Important rules:
- Do not delete any Entry ID.
- Do not invent papers not present in my Paper_Index.csv.
- If a connection is speculative, label it as speculative.
- Prioritize usefulness for LLM-based multi-agent research preparation.