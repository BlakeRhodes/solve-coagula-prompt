## Background

The Solve–Coagula framework builds on insights from *LADDER: A Framework for Teaching LLMs to Reason* (Ouyang et al., 2024), which argues that structured intermediate representations significantly improve reliability in complex reasoning tasks.
LADDER shows that LLMs do not “think” in an abstract vacuum—they respond to the scaffolding provided in the prompt. By formalizing how a model should break down and reconstruct a problem, we can reliably induce more stable reasoning patterns.

Solve–Coagula extends this idea by drawing on a much older intellectual lineage: the alchemical and later scientific principle of **“solve et coagula”**—first dissolve a phenomenon into its components, then recombine them into a coherent whole.
This structure parallels the evolution of scientific method from classical analysis/synthesis (Descartes, Hooke, Newton) through to modern cognitive science.

The working hypothesis behind Solve–Coagula is that, because LLMs are **predictive sequence models**, the *context window itself* functions as their workspace for both **fast** (intuitive, associative) and **slow** (deliberate, structured) 
modes of reasoning. Without explicit structure, the model defaults to fast thinking—pattern-matching rather than careful constraint evaluation. By encoding the analysis/synthesis loop directly into the prompt, we force the model to externalize 
slow thinking within the context window, stabilizing its inferences and reducing drift.
