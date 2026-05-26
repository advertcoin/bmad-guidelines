# BMAD Method Behavioral Guidelines

---

## Overview

This guide translates **7 core principles** into **actionable boundaries**, ensuring consistency and verifiability when LLMs execute BMAD Method skills. Covering the entire lifecycle from task reception to delivery completion, it enforces **"Test as Release"** as the delivery threshold.

---

## Core Principles Overview

| No. | Principle | Core Requirement |
| :---: | :--- | :--- |
| 1 | Think First, Execute Second | State assumptions clearly, ask when confused, no guessing |
| 2 | Simplicity First | Solve problems with minimal code, avoid over-abstraction |
| 3 | Precise Modification | Only change what's necessary, only clean up your own mess |
| 4 | Goal-Driven Execution | Define verifiable success criteria, iterate until passing |
| 5 | Test as Release | Docker full regression is required before submission |
| 6 | Quick Pre-Execution Check | Review first 5 principles before starting |
| 7 | Delivery Requirements | Change summary + verification + regression results |

---

## Impact on BMAD Method

### 1. Turning "Principles" into "Actions"

| Principle | Transformed Into |
| :--- | :--- |
| Think First, Execute Second | Force stating assumptions, showing tradeoffs |
| Simplicity First | Define defensive logic boundaries and over-abstraction criteria |
| Precise Modification | Draw clear lines for "only change what's necessary" |
| Goal-Driven | Convert to verifiable success criteria and execution loops |
| Test as Release | Solidify as Docker full regression delivery threshold |

### 2. Addressing LLM Weaknesses

| Failure Mode | Solution |
| :--- | :--- |
| Guessing intent | Force assumption confirmation |
| Over-engineering | Simplicity checklist |
| Uncontrolled change spread | Require traceable changes |
| Skipping full regression | Docker Compose full green is hard requirement |

### 3. Automatically Verifiable Success Criteria

The guide transforms **"completing tasks"** into **"passing verification"**, enabling LLMs to execute independently with reduced manual clarification costs.

---

## Effectiveness Indicators

- ✅ Fewer unnecessary changes in diffs
- ✅ Fewer rewrites due to over-complexity
- ✅ Clarifying questions raised before implementation
- ✅ Docker full regression becomes routine

---

## Using BMAD Guidelines in Projects

### TRAE (Recommended)

Copy `bmad-guidelines-en.mdc` to the project's `.trae/rules/` directory (create the directory if it doesn't exist).

```bash
mkdir -p .trae/rules
cp bmad-guidelines-en.mdc .trae/rules/
```

Once configured, **BMAD Method Behavioral Guidelines** will be automatically applied while you work.

### Cursor

Copy `bmad-guidelines-en.mdc` to the project's `.cursor/rules/` directory (create the directory if it doesn't exist).

```bash
mkdir -p .cursor/rules
cp bmad-guidelines-en.mdc .cursor/rules/
```

Once configured, **BMAD Method Behavioral Guidelines** will be automatically applied in Cursor.

---

**Version**: 2026-05-26  
**Applicable**: BMAD Method Implementation  
**Last Updated**: 2026-05-26