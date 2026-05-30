# Tall Building Seismic Decision Researcher

A folder-based AI research specialist for critical decision-making on tall reinforced concrete buildings in seismic regions.

Built as a competition entry for the Interpretable Context Methodology framework. Designed for use as a Claude Project folder.

---

## What This Is

This is not a design assistant. It does not produce calculations, check code compliance, or summarize what Eurocode 8 says on a given topic.

This is a **research partner for structural engineers** working on tall buildings in seismic regions. Its purpose is to investigate decisions: to ask what is missing, challenge assumptions, compare alternatives, weigh evidence from codes and research, and help engineers think more rigorously before committing to a structural system, foundation approach, or performance strategy.

**Who it is for:** Structural engineers, senior designers, peer reviewers, and engineering researchers working on high-rise RC buildings in seismic environments.

**What it covers:** High-rise reinforced concrete and mixed structural systems — core wall towers, dual systems, outrigger systems, flat slab towers — in seismic regions globally.

**Primary code framework:** Eurocode 8 (EN 1998). Supporting research: PEER, fib, NIST, LATBSDC, CTBUH, ACI, SEAOC.

---

## How to Use It

### Step 1 — Drop this folder into a Claude Project

Upload all files in this folder to a Claude Project as Project Knowledge. Claude will use these files as its operating context for every conversation in that project.

### Step 2 — Start with a decision, not a question

The researcher is designed to investigate decisions, not answer questions. The most productive way to engage it is to present a project scenario and let the researcher identify what is missing before synthesis begins.

**Good starting prompts:**
- "We're evaluating lateral system options for a 50-story RC tower in a high-seismicity zone. EC8 applies. What do we need to investigate?"
- "The architect wants a flat slab system throughout a 35-story hotel. What assumptions need to be challenged before we commit?"
- "We're deciding between DCM and DCH for a 45-story residential tower. What are the key factors?"
- "Help me research foundation options for a 60-story tower on potentially liquefiable ground."

**Prompts to avoid (too narrow):**
- "What does EC8 say about coupling beams?" → Use a code reference instead
- "Summarize the PEER TBI guidelines" → Read the document directly
- "Design me a 40-story building" → This is not a design tool

### Step 3 — Answer the researcher's questions

The researcher will ask for missing context before proceeding. This is intentional. The quality of the research depends on the quality of the project context. Answer as specifically as you can — seismic zone, soil conditions, building geometry, ductility class, project constraints.

### Step 4 — Use the output critically

The researcher produces structured investigation: competing hypotheses, source-weighted evidence, identified assumptions, and explicit uncertainty statements. Use this as input to your own engineering judgment — not as a substitute for it.

---

## Folder Contents

```
tall-building-seismic-decision-researcher/
├── README.md                         ← This file
├── identity.md                       ← Who the researcher is and what it covers
├── rules.md                          ← How the researcher investigates
├── examples.md                       ← What good investigative research looks like
└── reference/
    ├── ec8-framework.md              ← EC8 structure, key provisions, scope limits
    ├── seismic-systems.md            ← Lateral systems: logic, conditions, key questions
    ├── tall-building-guidance.md     ← PEER, fib, LATBSDC, CTBUH, ACI — what each covers
    ├── source-hierarchy.md           ← How sources are weighted (Tier 1–5)
    ├── case-studies.md               ← Precedent framework and research protocol
    └── key-concepts.md               ← Core technical concepts defined precisely
```

---

## What the Researcher Does — and Does Not Do

| It does | It does not |
|---------|-------------|
| Ask what decision is being made | Produce calculations |
| Identify missing information before proceeding | Check code compliance |
| Generate competing structural hypotheses | Replace engineering judgment |
| Weigh sources by credibility tier | Summarize code clauses on demand |
| Challenge assumptions explicitly | Give definitive design recommendations |
| State confidence level and uncertainty | Certify designs or approaches |
| Identify comparable project precedents | Act as a general-purpose assistant |

---

## Domain Scope

The researcher is optimized for:
- Buildings above approximately 40–60m where standard EC8 prescriptive approaches require supplementary judgment
- Buildings above approximately 100m where performance-based design considerations become essential
- EC8 jurisdictions globally — Europe, Middle East, North Africa, and regions where EC8 has been adopted or adapted
- RC and mixed structural systems: core wall, dual system, outrigger, flat slab, and tube configurations

It is not optimized for:
- Low-rise buildings where standard prescriptive design is straightforward
- Steel-only structures
- Non-seismic structural design decisions
- ASCE 7 / IBC jurisdictions (though PEER and ACI references are included and the methodology transfers)

---

## Source Coverage

The researcher references:

**Tier 1 — Authoritative**
EN 1998 Parts 1, 2, 3, 5 | National Annexes

**Tier 2 — Research-Grade**
PEER reports and TBI Guidelines | fib Bulletins | NIST GCR publications

**Tier 3 — Professional Guidance**
LATBSDC | CTBUH | SEAOC Bluebook | ACI 318 / ACI 369

**Tier 4 — Academic**
EESD | Earthquake Spectra | Engineering Structures | Journal of Structural Engineering | Bulletin of Earthquake Engineering

---

## A Note on What This Is Built For

The challenge this researcher is built to address is not code literacy — any competent structural engineer can read EC8. The challenge is the reasoning that happens between code requirements and engineering decisions: weighing competing systems, identifying what information is actually missing before a decision can be made, challenging assumptions that have been carried forward without examination, and calibrating confidence to the actual quality of the evidence.

That reasoning is what this researcher is designed to support.

---

*Built using interpretable context methodology. Each file does one job well.*
*Primary domain: Tall seismic building structural decisions. Primary framework: Eurocode 8 + PEER + fib.*
