````markdown
# Janus 5.0 — Master Mathematical & Structural Standard

## Overview

Janus 5.0 is a rigorous, mathematically grounded framework designed to model cognitive recursion and psychological structures as directed symbolic graphs. It formalizes key concepts such as:

- **Recursive introspection depth**: Tracking levels of self-reflective thought nesting  
- **Contradiction density**: Measuring the ratio of conflicting edges within cognitive clusters  
- **Entropy and coherence mass**: Quantifying psychological stability via graph-entropy inverses  
- **Projection bias**: Balancing future-oriented simulation against memory-anchored cognition  

The framework includes:

- Detailed JSON schemas for nodes (beliefs, memories, contradictions, emotions) and edges (reinforcement, contradiction, blending, etc.)  
- Operational algorithms for contradiction injections, rollback mechanisms, and recursive consistency checks  
- Safety parameters and thresholds for stable cognitive simulation  
- Expansion modules for multi-path scenario forecasting, ambiguity stress testing, and meta-experiment auditing  

---

## Purpose

Janus 5.0 is an independent, curiosity-driven effort to provide a formal, auditable foundation for symbolic cognitive modeling. Goals:

1. Enable experimental simulation of psychological recursion and stability  
2. Offer a collaboration platform for formal cognitive architectures  
3. Serve as a reference for researchers interested in symbolic, graph-based cognition  

---

## AI Usage Disclosure

AI language models (e.g., GPT) assisted with drafting and formatting, but **all conceptual and mathematical content is original**. AI is used purely as an augmentation tool, **not a substitute for research**.

---

## Core Concepts & Data Structures

### Node Schema

| Field             | Type / Range | Description |
|-------------------|-------------|-------------|
| `id`              | `string`    | Unique identifier |
| `type`            | `enum`      | `belief`, `memory`, `schema`, `emotion`, `contradiction` |
| `base_weight`     | `float [0,1]` | Inherent importance |
| `stability_score` | `float [0,1]` | Resistance to change |
| `recursion_depth` | `int ≥ 0`  | Reflective nesting level |
| `load_pressure`   | `float ≥ 0` | Local strain from contradictions/emotions |
| `labels`          | `string[]` | Optional semantic tags |

```json
{
  "id": "node_001",
  "type": "belief",
  "base_weight": 0.75,
  "stability_score": 0.9,
  "recursion_depth": 3,
  "load_pressure": 0.22,
  "labels": ["identity", "self-esteem"]
}
````

### Edge Schema

| Field    | Type / Range  | Description                                                                |
| -------- | ------------- | -------------------------------------------------------------------------- |
| `source` | `string`      | Origin node ID                                                             |
| `target` | `string`      | Destination node ID                                                        |
| `weight` | `float [0,1]` | Influence strength                                                         |
| `type`   | `enum`        | `reinforce`, `contradict`, `blend`, `anchor`, `reflects_on`, `projects_to` |

```json
{
  "source": "node_001",
  "target": "node_017",
  "weight": 0.6,
  "type": "contradict"
}
```

---

## Key Metrics

| Metric                    | Formula                                                                                  | Purpose                                 |   |                     |
| ------------------------- | ---------------------------------------------------------------------------------------- | --------------------------------------- | - | ------------------- |
| **Contradiction Density** | $\displaystyle \frac{\sum_{e \in E_C,\,t_e=\text{contradict}} w_e}{\sum_{e\in E_C} w_e}$ | Conflict saturation in subgraph $C$     |   |                     |
| **Load Pressure**         | (\displaystyle \sum\_{e \in \text{in}(n),,t\_e\in{\text{contradict},\text{emotion}}}     | w\_e                                    | ) | Tension on node $n$ |
| **Coherence Mass**        | $\displaystyle \frac{1}{H(S)+\epsilon}$                                                  | Structural stability of subgraph $S$    |   |                     |
| **Projection Bias**       | $\displaystyle \frac{\sum_{t_e=\text{projects\_to}} w_e}{\sum_{e\in E} w_e}$             | Future-simulation vs memory orientation |   |                     |
| **Graph Entropy**         | $\displaystyle H(S)= -\sum_i p_i\log p_i,\; p_i=\frac{w_i}{\sum_j w_j}$                  | Disorder of edge-weight distribution    |   |                     |

---

## Algorithms & Safety

* **Contradiction Injection**: Add contradiction edges of intensity $\alpha$ to stress-test clusters
* **Rollback Protocol**: Auto-restore last snapshot if thresholds are breached
* **Recursive Consistency Check**: Scan up to depth $d_{\max}$ for instability

---

## JSON Snapshot Example

```json
{
  "nodes": [...],
  "edges": [...],
  "global_metrics": {
    "global_stability_index": 0.72,
    "average_contradiction_density": 0.28,
    "overall_projection_bias": 0.57,
    "average_recursion_depth": 2.4,
    "system_entropy": 1.32
  },
  "parameters": {
    "max_recursion_depth": 10,
    "paradox_tolerance": 0.35,
    "load_pressure_threshold": 0.65,
    "entropy_collapse_cutoff": 0.25,
    "projection_bias_alert": 0.8,
    "rollback_on_flag": true,
    "epsilon_stabilizer": 0.001
  },
  "timestamp": "2025-07-01T14:23:45Z"
}
```

---

## Repository Contents

* **`Janus_5.0_Mathematical_Standard.tex`** — LaTeX source
* **`Janus_5.0_Mathematical_Specification.pdf`** — Compiled spec
* **`cover_letter.tex`** — Formal cover letter template
* **`README.md`** — This document

---

## How to Use

1. Compile the LaTeX source (Overleaf, TeX Live, or MikTeX)
2. Implement graph structures per JSON schemas
3. Run algorithms for contradiction injection, rollback, & consistency checks

---

## Contribution

Contributions welcome:

* Mathematical refinements
* Software simulations & visualizations
* New experimental modules
* Issue reports & pull requests

---

## License

Released under the **MIT License**.

```
```
