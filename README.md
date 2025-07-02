# Janus 5.0 — Master Mathematical & Structural Standard

Deep Dive Explanation: https://notebooklm.google.com/notebook/32e42d74-3cd7-4a40-87ae-7bed6172b1f7/audio

## Project Scope

Janus 5.0 is an open‑source framework that models cognition as a **directed symbolic graph**.  It provides:

* **Recursive‑depth tracking** — explicit levels of self‑reflection.
* **Contradiction density** — quantitative measure of internal conflict.
* **Graph‑entropy / coherence‑mass metrics** — stability vs. disorder.
* **Projection bias** — balance between future simulation and memory anchoring.

The repository contains the formal LaTeX specification, JSON data schemas, and reference algorithms for experimentation and safety rollback.

---

## Why Janus?

* Establishes a *mathematically auditable* cognitive model.
* Enables controlled stress‑tests (contradiction injection, entropy collapse).
* Serves as a launch‑point for symbolic‑AI or neuro‑symbolic research.

---

## AI‐Assistance Disclaimer

Large‑language models (GPT) were used **only** for drafting and formatting.  All core concepts and mathematics are original first‑principles work.

---

## Data Structures

### Node Schema

| Field             | Type      | Range                                                  | Description                            |
| ----------------- | --------- | ------------------------------------------------------ | -------------------------------------- |
| `id`              | string    | —                                                      | Unique identifier                      |
| `type`            | enum      | belief \| memory \| schema \| emotion \| contradiction | Cognitive category                     |
| `base_weight`     | float     | 0–1                                                    | Inherent importance                    |
| `stability_score` | float     | 0–1                                                    | Resistance to change                   |
| `recursion_depth` | int       | ≥ 0                                                    | Nesting level                          |
| `load_pressure`   | float     | ≥ 0                                                    | Tension from contradictions & emotions |
| `labels`          | string\[] | —                                                      | Optional semantic tags                 |

```json
{
  "id": "node_001",
  "type": "belief",
  "base_weight": 0.75,
  "stability_score": 0.9,
  "recursion_depth": 3,
  "load_pressure": 0.22,
  "labels": ["identity", "self‑esteem"]
}
```

### Edge Schema

| Field    | Type   | Range                                                                      | Description         |
| -------- | ------ | -------------------------------------------------------------------------- | ------------------- |
| `source` | string | —                                                                          | Origin node ID      |
| `target` | string | —                                                                          | Destination node ID |
| `weight` | float  | 0–1                                                                        | Influence strength  |
| `type`   | enum   | reinforce \| contradict \| blend \| anchor \| reflects\_on \| projects\_to | Edge nature         |

---

## Core Metrics (formulas in LaTeX spec)

* **Contradiction Density** — conflict ratio per cluster.
* **Load Pressure** — cumulative strain on a node.
* **Coherence Mass** — 1 / (graph‑entropy + ε).
* **Projection Bias** — forward‑simulation weight ratio.

---

## Algorithms

* **Contradiction Injection** — synthetic conflict for stress‑tests.
* **Recursive Consistency Check** — scan layers ≤ `d_max` for instability.
* **Rollback Protocol** — auto‑restore last stable snapshot on threshold breach.

---

## Quick Start

1. **Compile** `Janus_5.0_Mathematical_Standard.tex` (Overleaf / TeX Live) ⇒ PDF.
2. **Instantiate** graph objects following the JSON schemas.
3. **Run** reference algorithms to measure metrics or inject contradictions.

---

## Repository Layout

```
├── Janus_5.0_Mathematical_Standard.tex   # LaTeX source
├── Janus_5.0_Mathematical_Specification.pdf
├── cover_letter.tex                      # Formal cover letter example
└── README.md                             # This document
```

---

## Contributing

Pull requests & issues welcome for:

* Mathematical clarifications or expansions
* Software simulations & visualisations
* New experimental modules

---

## License

Released under the **MIT License** — free and open‑source.
