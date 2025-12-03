# Solve–Coagula Prompt

A compact reasoning framework for LLMs designed to **stabilize multi-step analysis**, prevent hidden assumptions, and enforce **explicit-final-answer** discipline.  
Useful for A/B testing reasoning strategies and building predictable agentic behaviors.

---

## What This Repo Provides

- **`solve-coagula.md` — Core Framework**  
  A reusable prompt that forces models into a two-phase reasoning loop:  
  **SOLVE** = decompose, list objects, separate givens/assumptions/unknowns.  
  **COAGULA** = re-check constraints, synthesize, and produce a single final answer.

- **Problem Templates & Examples**  
  - `problem-template` — Minimal structure for documenting reasoning experiments.  
  - `bridge-crossing.md` — Timing/constraints puzzle example.  
  - `poison-wine.md` — Information theory puzzle example.

These illustrate how Solve–Coagula reduces drift and forces explicit interpretation choices.

---

## Why Solve–Coagula Exists

Standard CoT often fails due to:
- unmarked assumptions,
- reasoning drift partway through the chain,
- misinterpreting ambiguous wording,
- forgetting constraints by the end.

Solve–Coagula fixes this by forcing the model to:

1. **Enumerate all objects and their properties**  
   (People, items, positions, times, rules, etc.)

2. **Separate factual givens from assumptions**  
   Every assumption must be labeled as such.

3. **List unknowns explicitly**  
   The model cannot “fill in” missing logic without tagging it.

4. **Surface alternative interpretations**  
   Particularly important for ambiguous or puzzle-like wording.

5. **Re-check the original problem during COAGULA**  
   Prevents the model from building a solution on unintended assumptions.

6. **Produce a clearly marked final answer**  
   Easy to evaluate, unit-test, or compare across runs.

---

## How to Use (Fast Workflow)

1. **Baseline Run**
   - Open a clean chat.
   - Paste the problem.
   - Use standard reasoning (“think step by step”).
   - Save the output.

2. **Solve–Coagula Run**
   - New clean session.  
   - Load `solve-coagula.md` as a memory/system prompt.  
   - Present the same problem with instructions to use the framework.  
   - Save the output.

3. **Compare**
   - Did it avoid drift?  
   - Did it expose hidden assumptions?  
   - Did it handle ambiguity better?  
   - Was the final answer cleaner?

The problem-template file provides a minimal documentation format for this process.

---

## When to Use Solve–Coagula

This framework is useful for:

- Benchmarking model reasoning across versions / providers.
- Forcing deterministic reasoning structures in agent pipelines.
- Creating reproducible traces for compliance/audit environments.
- Teaching models to avoid hallucinated constraints.
- Any scenario where you want **explicit epistemic hygiene** from the model.

---

## Roadmap

Potential additions:
- More puzzle benchmarks.
- Scripts for automated run comparison.
- Patterns for integrating Solve–Coagula into agent architectures.

---

## License

MIT License (see `LICENSE`).
