
---

# 🧠 JanusCore Saturn

### a symbolic cognitive sandbox that plays with contradictions, coherence, and psychological resilience

---

## 🚀 What is this?

This is basically a **tiny simulation lab for cognitive systems**, written as a symbolic engine that:

* builds a **graph of beliefs, schemas, and contradictions** (like a little mind),
* **tracks contradictions, coherence, and projection bias** using super simple metrics,
* automatically **rolls back if contradictions get too intense**, like a built-in psychological immune system,
* and even **runs stress tests by injecting paradoxes and seeing how well it recovers**.

It’s kind of a playground to explore how symbolic belief structures might fracture or stabilize under pressure.

---

## 🔍 Why did I make this?

Honestly?
Because I think contradictions are fascinating.
Sometimes when we humans run into paradoxes, we double down (confirmation bias), sometimes we totally collapse (existential crisis?), and sometimes we reorganize and come out more resilient.

So I wanted to see if I could **simulate that process explicitly**, in a symbolic system that:

* has clear metrics for contradiction load (CD), coherence (CM), and bias (PB),
* knows when it’s getting overwhelmed,
* and can track how well it stabilizes after deliberate paradox attacks.

No idea if there’s any real-world merit.
But it’s fun. And maybe someone will find a clever use for it in AI pipelines, psychology experiments, or weird games.

---

## ⚙️ How does it work? (super simple version)

### 1. It builds a graph 🕸

Imagine:

```
belief_1 --> schema_1
belief_2 --> schema_1
```

* Nodes are beliefs, schemas, or contradictions.
* Edges are like “belief\_1 reinforces schema\_1” or “belief\_2 projects to schema\_1”.

### 2. It calculates three main numbers 📊

| Metric                         | What it means                                                  |
| ------------------------------ | -------------------------------------------------------------- |
| **CD (Contradiction Density)** | how overloaded the graph is with paradoxes                     |
| **CM (Coherence Mass)**        | how structurally “clean” or focused it is (inverse of entropy) |
| **PB (Projection Bias)**       | how much it’s leaning into future unstable states              |

If CD gets too high (over a set `θc`), it **rolls back** to the last stable state.

---

### 3. It does experiments 🧪

* It **injects paradox edges** on purpose (like `belief_1 contradicts belief_2`).
* Watches CD spike and CM drop.
* Then **injects schema reinforcement edges** to see if the system can bring coherence back up.
* Logs how well it recovers — giving you a kind of **symbolic resilience score**.

It can even adaptively change how heavy the paradox vs. reinforcement is, to stress-test different “cognitive personalities.”

---

## 🛠️ Quick example

```python
# Start a graph with beliefs & schemas
nodes = ["belief_1", "belief_2", "schema_1"]
edges = [
    ("belief_1", "schema_1", "reinforce"),
    ("belief_2", "schema_1", "projects_to")
]

# Calculates:
# CD = 0.0 (no contradictions yet)
# CM ≈ 1.0 (nice and coherent)
# PB ≈ 0.44 (some future projection)

# Now inject contradictions
edges += [
    ("belief_1", "belief_2", "contradict"),
    ("belief_2", "belief_1", "contradict"),
]

# CD spikes, CM drops
# If CD > θc, auto rollback
```

---

## 📝 Features at a glance

✅ Builds symbolic cognitive graphs
✅ Calculates contradiction density (CD), coherence mass (CM), projection bias (PB)
✅ Automatically rolls back to last stable state if overloaded
✅ Logs rollback deltas to see what changed
✅ Can do repeated paradox vs. reinforcement cycles to simulate resilience
✅ CLI & JSON logs (future: web dashboards with live charts)
✅ Can export to CSV for graphing or share snapshots

---

## 🚀 Why might you care?

* **Cognitive science / psych** folks: it’s a fun way to see how contradictions destabilize systems. Could loosely model bias or mental breakdowns under too much paradox.
* **AI / prompt engineers**: maybe you could run outputs through this first to flag contradiction-heavy results.
* **Game devs or simulation people**: might be neat to simulate NPC “belief meltdown” under stress.

Or just poke at it for fun — it’s cool to watch it freak out under paradox then calm itself down.

---

## ⚡ Getting started

Clone & run:

```bash
git clone https://github.com/your-username/januscore-saturn
cd januscore-saturn
pip install -r requirements.txt
python main.py
```

Or run the CLI:

```bash
python cli.py load sample_graph.json
python cli.py inject-paradox 0.3
python cli.py compute-metrics
python cli.py run-resilience-test --cycles 5
```

---

## 🙌 Final thoughts

Not sure if this has any *big* practical application — maybe it’s pointless.
But it’s been an awesome way to explore contradictions, resilience, and how a tiny symbolic “mind” might maintain coherence under stress.

If you dig into it and figure out clever uses, or want to map it to actual psychological theories, I’d love to hear about it.
Or if you want a demo of rollback logs or paradox graphs, ping me. Happy to overshare. 😄

---

## 📜 License

MIT — free for all your experiments, break it however you like.

---
