# Lecture 1: AI Basics for Central Bankers

**Course:** AI Tools for Central Bankers (2 hours)  
**Lecture:** 1 of X  
**Audience:** Central bank economists, supervisors, and policy professionals  
**Goal:** Build a clear mental model of what modern AI is, what it is not, and how to use it responsibly in policy and supervision settings.

---

## 1) Why central bankers should care about AI

AI is not a new mandate, but it is a new production technology for knowledge work. It can lower the cost of drafting, summarising, coding, and searching. It can also amplify errors, bias, and overconfidence if it is used without governance. Central banks care for three reasons:

1. **Productivity in analysis and communication:** faster drafting, clearer synthesis, better internal documentation.
2. **Risk management:** model risk, operational risk, confidentiality, and reputational risk.
3. **Policy and supervision relevance:** AI is changing the private sector, including credit allocation, payment systems, and risk management tools.

---

## 2) A simple taxonomy of AI

### 2.1 Artificial intelligence (AI)
A broad term for systems that perform tasks that usually require human intelligence, such as perception, prediction, and language.

### 2.2 Machine learning (ML)
A subset of AI where systems learn patterns from data to make predictions or decisions.  
Examples: credit scoring models, fraud detection, forecasting models.

### 2.3 Deep learning
A subset of ML using neural networks with many layers. It performs well in areas like speech, images, and language.

### 2.4 Generative AI
Models that generate text, images, code, audio, or other content.  
Examples: drafting a briefing note, proposing code, summarising a paper.

**Key point:** Generative AI is often a language and pattern engine, not a truth engine.

---

## 3) What a modern language model is doing

A large language model (LLM) is trained to predict the next token (a piece of a word) given the previous tokens. Through training on large text corpora, the model learns statistical regularities of language and of the content embedded in that language.

### 3.1 Why it can feel intelligent
- It can produce fluent, coherent text.
- It can follow instructions reasonably well.
- It can mimic styles and formats.
- It can generalise across domains.

### 3.2 Why it can be wrong even when confident
- It optimises for plausible continuation, not verified truth.
- It may fill gaps with invented details.
- It may cite sources that do not exist if you do not constrain it.
- It may be sensitive to prompt wording and context.

**Rule for policy work:** Treat outputs as drafts and hypotheses, not as evidence.

---

## 4) Core concepts you should know

### 4.1 Training, fine-tuning, and prompting
- **Training:** learning general patterns from large datasets.
- **Fine-tuning:** adjusting a model to do better on a narrower task or domain.
- **Prompting:** giving instructions and context to guide outputs at use time.

### 4.2 Context window
Models have a limit to how much text they can consider at once. Long documents may need chunking or summarisation, which can lose nuance.

### 4.3 Retrieval-Augmented Generation (RAG)
A method where the model pulls relevant information from a trusted document store before answering. This can reduce hallucinations and improve traceability.

### 4.4 Temperature and variability
Some systems allow you to control how deterministic the output is. Higher variability can help brainstorming but can hurt consistency.

---

## 5) Where AI is useful in central banking

### 5.1 High-value, lower-risk tasks
- Drafting internal notes and outlines.
- Summarising papers and meeting notes.
- Converting bullet points to clear prose.
- Editing for clarity and consistency.
- Generating code scaffolds and documentation.
- Creating checklists, templates, and standard operating procedures.

### 5.2 High-value, higher-risk tasks (needs safeguards)
- Interpreting market-moving information.
- Producing policy recommendations.
- Analysing supervisory cases with confidential data.
- Generating quantitative claims or statistics.
- Drafting external communications under time pressure.

**Practical guidance:** Use AI most aggressively for structure, wording, and workflow acceleration. Use it more cautiously for facts, numbers, and causal claims.

---

## 6) Typical failure modes and how to defend against them

### 6.1 Hallucination (fabricated facts)
**Defence:** request sources, verify against primary material, and require an assumptions list.

### 6.2 Spurious precision
Models can produce confident numbers, dates, or references.  
**Defence:** disallow invented statistics and require explicit citation or “unknown”.

### 6.3 Misleading coherence
A coherent narrative can hide weak logic.  
**Defence:** ask for alternative explanations, counterarguments, and what would falsify the claim.

### 6.4 Prompt sensitivity
Small wording changes can shift outputs.  
**Defence:** use standard prompt templates and keep an audit trail of key prompts.

### 6.5 Data confidentiality risk
Sensitive information may be pasted into tools without safeguards.  
**Defence:** classify data, redact, abstract, and follow institutional rules.

---

## 7) A central bank standard for verification

Before you rely on an AI-assisted output, apply a verification routine:

1. **Label the output:** draft, hypothesis, or final.
2. **Check the foundations:** definitions, assumptions, and scope.
3. **Verify key claims:** numbers, dates, citations, and institutional details.
4. **Triangulate:** cross-check with primary sources and internal data.
5. **Stress test reasoning:** ask for counterarguments and failure cases.
6. **Document your edits:** what you changed and why.

---

## 8) Prompting basics you can reuse

### 8.1 A safe general template
Copy and adapt:

> You are assisting a central bank analyst.  
> Task: [what you want].  
> Audience: [who will read it].  
> Scope: [what to include and exclude].  
> Constraints: do not invent facts, do not guess numbers, flag uncertainty.  
> Output format: [bullets, table, memo].  
> Provide: assumptions, items requiring verification, and risks.

### 8.2 A “no hallucination” add-on
> If you are unsure, write “unknown” and propose how to verify.

### 8.3 A review add-on
> After drafting, critique your answer: list the weakest points, missing caveats, and what a sceptical reader would challenge.

---

## 9) Short exercises (10 minutes total)

### Exercise A: Rewrite for policy clarity
Take a dense paragraph from a recent internal note. Prompt the tool to rewrite it for a Governor-level audience in 150 words.  
Then check: what did it simplify, and did it remove necessary caveats?

### Exercise B: Generate a verification checklist
Ask the tool to produce a checklist to validate a macro claim made in a draft briefing.  
Then compare it to your standard empirical habits.

---

## 10) Key takeaways

- AI tools are best treated as accelerators for drafting, organisation, and exploration.
- The model optimises for plausibility, not truth, so verification is not optional.
- Governance matters because errors scale quickly in high-trust institutions.
- The best results come from clear prompts, constrained outputs, and disciplined checking.

---

## Suggested further reading
- Model risk management and validation principles (internal guidance, plus relevant supervisory standards).
- Practical notes on retrieval and citation-based workflows for institutional use.
- Recent central bank speeches or BIS notes on AI in finance and public institutions (use your institution’s curated list).


