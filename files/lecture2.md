# Lecture 2: Prompting and Workflow Patterns for Policy-Grade AI Use

**Course:** AI Tools for Central Bankers (2 hours)  
**Lecture:** 2 of X  
**Goal:** Turn AI from a novelty into a disciplined tool by learning how to specify tasks, constrain outputs, and verify results to a central bank standard.

---

## 1) Learning objectives

By the end of this lecture, participants will be able to:

1. Write prompts that function as clear task specifications (purpose, audience, constraints, format).
2. Use reliable workflow patterns for drafting, summarising, coding support, and research synthesis.
3. Reduce common failure modes (invented facts, spurious precision, misleading coherence) using structured checks.
4. Create outputs that are easier to audit, including assumptions lists, verification items, and decision logs.
5. Apply safe-use practices for confidentiality and institutional credibility.

---

## 2) The core idea: prompting is specification, not conversation

In central banking, good outputs come from good specifications. Treat the prompt like a terms of reference:

- **Task:** What you want produced.
- **Audience:** Who will read it and what they care about.
- **Scope:** What is in and what is out.
- **Constraints:** What the tool must not do (no invented facts, no guessing numbers).
- **Format:** Memo, bullets, table, slide notes, code, checklist.
- **Verification:** What must be checked before use.

**Practical rule:** If you cannot explain the task clearly to a colleague, the tool will also struggle.

---

## 3) Prompt templates you can reuse

### 3.1 Policy memo template (safe, auditable)
Copy and adapt:

> You are assisting a central bank analyst.  
> **Task:** Draft a 1-page memo on [topic].  
> **Audience:** [Governor, MPC, supervision committee].  
> **Scope:** Include [A, B, C]. Exclude [D, E].  
> **Constraints:** Do not invent facts. Do not guess numbers or citations. If uncertain, write “unknown” and propose how to verify.  
> **Output format:** Headings, short paragraphs, and a final bullet list titled “Items to verify.”  
> **Also provide:** (i) assumptions, (ii) counterarguments, (iii) what would change the recommendation.

### 3.2 Research synthesis template (triangulation built in)
> Summarise the main mechanisms and empirical strategies in this material.  
> Then list: (i) key claims, (ii) what evidence supports each claim, (iii) what remains uncertain, (iv) the most plausible alternative interpretation.

### 3.3 Coding support template (keeps humans in control)
> Generate pseudocode and then Python code for [task].  
> Explain the logic and include unit tests.  
> Do not assume access to external data.  
> If there are multiple approaches, present two and state trade-offs.

---

## 4) Workflow patterns that work in practice

### Pattern A: Draft, critique, revise
1. Ask for a draft.
2. Ask for a critique that lists weaknesses, missing caveats, and likely objections.
3. Ask for a revision that fixes only those weaknesses.

**Why it helps:** You create a built-in quality-control loop, which matters in policy settings.

### Pattern B: Decompose the task
Instead of “write the whole briefing,” do:
1. Define terms and scope.
2. Produce an outline.
3. Draft each section with explicit constraints.
4. Assemble and tighten.

**Why it helps:** Large tasks invite hallucination and accidental overreach.

### Pattern C: Make verification explicit
Always request:
- A list of assumptions.
- A list of items requiring verification.
- A list of data needs and where to source them.
- A short “risk of misuse” section.

### Pattern D: Retrieval-first when facts matter
If the task depends on facts, base the output on a controlled document set:
- internal notes (sanitised)
- published statistical releases
- official speeches and reports
- legislation and regulatory guidance

**If you cannot provide the documents, require the model to label facts as “needs verification.”**

---

## 5) Common failure modes and fixes

### 5.1 Invented facts or citations
**Fix:** Explicitly ban invention and require “unknown” plus a verification path.

### 5.2 Spurious precision
**Fix:** Tell the tool to avoid numbers unless provided, and to use ranges only when justified.

### 5.3 Confident but shallow reasoning
**Fix:** Request counterarguments, alternative mechanisms, and what evidence would falsify the claim.

### 5.4 Policy tone without policy content
**Fix:** Require a structured logic chain:
- mechanism
- evidence
- trade-offs
- risks
- decision points

---

## 6) Video for this lecture

Watch the video below, then use the discussion questions to connect the themes to central bank work.

[![Watch on YouTube](https://img.youtube.com/vi/G5teYbovYJ0/0.jpg)](https://www.youtube.com/watch?v=G5teYbovYJ0)

**Suggested viewing focus**
- Where does AI raise the productivity of researchers and knowledge workers?
- What new bottlenecks appear (verification, evaluation, coordination, incentives)?
- What complements matter (data, institutions, skills, governance)?

---

## 7) Discussion questions (10 minutes)

1. Which parts of a typical central bank workflow look most “R&D-like” (idea generation, testing, iteration)?
2. Where would AI tools most likely improve productivity in your team: drafting, coding, literature mapping, or internal knowledge management?
3. What would be your minimum governance standard before scaling AI use across a department?
4. How would you prevent “policy laundering,” where a weak argument is dressed up as a coherent memo?

---

## 8) Mini-lab (20 minutes)

### Exercise 1: Policy brief rewrite with verification
Take a paragraph from a recent briefing (use a non-confidential excerpt or a synthetic example).

Prompt:
> Rewrite for an MPC audience in 150 words.  
> Preserve all caveats.  
> Add a final section titled “Items to verify” with 5 bullets.

Deliverable:
- Revised paragraph
- “Items to verify” list

### Exercise 2: Build a prompt that prevents hallucination
Prompt:
> Create a structured outline for a note on [topic].  
> For each section, list what data or sources are required.  
> If any claim would require external confirmation, label it “needs verification.”

Deliverable:
- Outline
- Source and data requirements
- Marked “needs verification” items

---

## 9) Practical guardrails for central banks

- Do not paste confidential, market-sensitive, or personally identifiable information into tools that are not approved for such data.
- Use abstraction and redaction. Replace institution names, dates, and figures with placeholders when needed.
- Keep an audit trail for high-stakes outputs: prompt, model version (if known), edits made, and verification steps taken.
- Treat final accountability as human, even when drafting is AI-assisted.

---

## 10) Key takeaways

- Better prompts are better specifications.
- Reliable workflows reduce risk more than clever one-shot prompts.
- Verification is a feature, not an afterthought.
- Central bank credibility depends on disciplined use, not just productivity gains.

#DISCLAIMER

This github module is intended solely as a learning exercise. All the output is largely AI-generated. It is a fictional course setup. Videos are selected from Youtube
