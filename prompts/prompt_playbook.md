# Prompt Playbook
**How I work with LLMs as a reasoning partner, not an answer engine.**

This project treats large language models as tools for **stress-testing ideas, clarifying structure, and exposing weak inference**, not as sources of authority or prediction.

The goal is not speed or output volume, but **credibility under uncertainty**.

---

## Core principles

### 1. Clarification before completion
If a question cannot be answered unambiguously, the model is instructed to request clarification rather than infer intent.

This avoids false confidence and hallucinated certainty.

Example:
> “If a single unambiguous answer is required, identify missing constraints before responding.”

---

### 2. Behaviour over narrative
Prompts prioritise **revealed behaviour** over stated intent, press narratives, or executive commentary.

Example:
> “Analyse this situation using observed consumer behaviour, not public statements or strategic messaging.”

---

### 3. Traits vs. states
Models are explicitly asked to separate:
- **Traits**: stable incentives, structural constraints
- **States**: temporary conditions, shocks, or reactions under pressure

Example:
> “Which elements here reflect durable incentives, and which appear to be short-term responses?”

---

### 4. Inference strength labelling
All outputs are encouraged to distinguish between:
- strong inference (multi-year pattern consistency)
- speculative inference (plausible but unverified)

Example:
> “Flag where conclusions are strongly supported vs. where they remain speculative.”

---

### 5. Second- and third-order effects
Prompts regularly push beyond first-order outcomes.

Example:
> “What second- or third-order effects might emerge if this behaviour persists for 3–5 years?”

---

## Common prompt patterns used in this project

### Stress-testing a thesis
> “Break this argument. Identify where it could collapse under alternative assumptions or missing data.”

### Removing pundit tone
> “Rewrite this in a case-study tone suitable for a strategy consultant or board-level reader. Remove emotional language and certainty theatre.”

### Separating platform from behaviour
> “Does this outcome reflect a change in consumer preference, or a change in delivery mechanism? Explain the difference.”

### Metric validation
> “Which metrics here measure urgency rather than engagement? What behaviours might they fail to capture?”

### Ambiguity containment
> “Allow multiple interpretations, but identify the structural invariants that hold regardless of outcome.”

---

## Guardrails

- No predictions framed as certainty  
- No hero/villain narratives  
- No platform evangelism  
- No deal-specific speculation without structural relevance  

If an insight feels emotionally satisfying but analytically weak, it is explicitly challenged.

(Internal guardrail phrase used during development: **“STOP RIGHT THERE”**.)

---

## Role of the human vs. the model

- **Human**: framing, judgment, boundary-setting, final accountability  
- **Model**: pattern surfacing, counter-arguments, language tightening, blind-spot exposure  

The model assists reasoning; it does not replace it.

---

## Why this matters

This approach reflects how LLMs can be integrated into decision intelligence, strategy, and analytical workflows where:
- ambiguity is unavoidable
- credibility matters more than speed
- outputs may be reviewed by senior stakeholders

The emphasis is on *how* conclusions are reached, not just *what* they are.
