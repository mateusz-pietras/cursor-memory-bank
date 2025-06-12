# Creative Phase: Rules Formalization

**Date:** 2024-07-26

## 1. Objective

To perform a creative design phase for the formalization of development rules, specifically for Patrol integration testing and general knowledge capture.

## 2. Task 1: Refine `testing-patrol.mdc`

### 2.1. Component Description
The existing Patrol testing rule file (`.cursor/rules/flutter/testing-patrol.mdc`). The goal is to make it stricter, more actionable, and clearer.

### 2.2. Requirements & Constraints
- Must provide a clear, step-by-step process.
- Must use formal keywords (`MUST`, `SHOULD`, `MUST NOT`).
- The "Widget Key Pattern" must be presented as a mandatory, non-negotiable process.

### 2.3. Options Analysis
- **Option 1: Single, Top-Level Checklist**: A large, mandatory checklist at the beginning.
  - **Pros**: Highly visible.
  - **Cons**: Intimidating, bureaucratic.
- **Option 2: Contextual Checklists**: Smaller checklists interspersed throughout the document.
  - **Pros**: More digestible, presented in context.
  - **Cons**: Easy to miss if a developer skips sections.
- **Option 3: Hybrid Approach**: A short, high-level checklist at the top, with detailed steps and checklists within relevant sections.
  - **Pros**: Balances a quick overview with in-depth guidance.
  - **Cons**: Slightly more complex structure.

### 2.4. Recommended Approach
**Option 3 (Hybrid Approach)** is selected. It offers the best balance of immediate visibility and detailed contextual information.

### 2.5. Implementation Guidelines
1.  Add a "Core Principles" section at the top with a short, non-negotiable checklist.
2.  Refactor the "Widget Key Pattern" section into a formal, numbered process using `MUST` statements.
3.  Systematically replace ambiguous language with `MUST`, `SHOULD`, and `MUST NOT` throughout the rule.

---

## 3. Task 2: Create `knowledge-capture.mdc`

### 3.1. Component Description
A new rule (`.cursor/rules/general/knowledge-capture.mdc`) to standardize how analysis and knowledge are captured and stored.

### 3.2. Requirements & Constraints
- Must define a simple, standard template for analysis documents.
- Must mandate a standard storage location.
- Must be a low-friction process to encourage adoption.

### 3.3. Options Analysis
- **Option 1: Highly-Strict, Multi-Section Template**: A rigid, overly-detailed template.
  - **Pros**: Extremely thorough.
  - **Cons**: High friction, likely to be ignored.
- **Option 2: Minimalist Template**: A very simple template (e.g., Title, Summary).
  - **Pros**: Easy to adopt.
  - **Cons**: May not capture sufficient detail.
- **Option 3: Balanced, Example-Based Template**: A template based on the successful `patrol_integration_analysis.md` document.
  - **Pros**: Practical, proven, and captures the right level of detail.
  - **Cons**: None significant.

### 3.4. Recommended Approach
**Option 3 (Balanced, Example-Based Template)** is selected. It is practical and based on a successful precedent.

### 3.5. Implementation Guidelines
1.  Create the new file at `.cursor/rules/general/knowledge-capture.mdc`.
2.  Define the rule's purpose: creating a transparent "paper trail" of analysis.
3.  Mandate that analysis documents be stored in a new `memory-bank/analysis/` directory.
4.  Provide the official markdown template, modeled after the patrol analysis document. 
