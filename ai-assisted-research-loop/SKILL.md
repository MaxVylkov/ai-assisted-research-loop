---
name: ai-assisted-research-loop
description: Use when the user wants to structure, evaluate, or expand a scientific research idea using Dlan Nauki / Длань Науки, an AI-assisted research loop; triggers include Dlan Nauki, Длань Науки, research loop, research recipe, feasibility/no-go check, literature-to-calculation workflow, scientific planning, experiment journal, calculation journal, research memo, or Obsidian research notes. Guides Codex through hypothesis, literature check, minimal model, rough estimate, numerical calculation, systematics/backgrounds, internal review, decision, and write-up.
---

# Dlan Nauki

## Purpose

Use **Dlan Nauki** / **Длань Науки** to turn a broad scientific idea into a reproducible research workflow. Treat AI as a controlled research assistant: it may search, summarize, calculate, critique, and draft, but it must keep assumptions, sources, uncertainty, and decisions explicit.

## Core Workflow

For every new research direction, proceed through this loop unless the user asks for only one stage:

1. **Hypothesis** - formulate the main question and the working hypothesis. State what would count as a useful positive, negative, or no-go result.
2. **Literature Check** - identify close prior work, what is already known, and what is different in the user's formulation. Browse or inspect supplied files when current or source-specific accuracy matters.
3. **Minimal Model** - define the smallest physical, mathematical, or computational model that can test the idea. List included effects, neglected effects, parameters, and units.
4. **Back-of-the-envelope Estimate** - compute order-of-magnitude numbers before building a detailed model. Use this to catch impossible ideas early.
5. **Numerical Calculation** - make calculations reproducible: formulas, inputs, data files, code, plots, and versioned assumptions.
6. **Systematics and Backgrounds** - identify dominant uncertainties, backgrounds, degeneracies, calibration needs, and sensitivity to assumptions.
7. **Internal Review** - critique the result as a skeptical reviewer: missing citations, weak assumptions, overclaimed conclusions, numerical fragility, and required validation.
8. **Decision** - classify the direction as continue, revise, park, or no-go/feasibility-limited. Explain the reason in one paragraph.
9. **Write-up** - convert the result into an Obsidian note, analytical memo, paper section, slide outline, task list, or other requested artifact.

## Short Mode

When the user asks for a quick screening or early feasibility check, use the compressed loop:

```text
question -> literature -> rough estimate -> dominant background/systematic -> decision
```

Use short mode for early screening. Move to the full workflow if the idea survives the first pass.

## Experiment And Calculation Journal

When doing calculations or iterative analysis, keep a compact journal entry with:

- date or session context;
- question;
- input parameters;
- data/source used;
- approximations;
- result;
- what seems reliable;
- what remains uncertain;
- next step.

## Scientific Defaults

When the task involves a physical, mathematical, or computational model, explicitly track:

- process or mechanism being studied;
- source spectrum, input data, or generative assumptions;
- detector, instrument, dataset, or simulation configuration;
- threshold, exposure, efficiency, sample size, or relevant scale parameters;
- irreducible backgrounds and ordinary experimental or computational backgrounds;
- systematic uncertainties needed to distinguish signal from background;
- whether the result is limited by physics, instrumentation, statistics, systematics, data quality, or model assumptions.

## Internal Review Checklist

Before presenting a conclusion as reliable, check:

- Is the main claim supported by the calculation or only suggested by it?
- Are all numerical inputs sourced or clearly labeled as assumptions?
- Does the result change qualitatively under reasonable parameter variation?
- Is there an obvious background, systematic, or prior paper that could invalidate the claim?
- Is the conclusion phrased at the right strength: continue, revise, park, or no-go?

## Output Style

Keep outputs operational. Prefer concrete tables, equations, assumptions, and next actions over broad motivational prose. When creating persistent notes or documents, preserve the user's existing naming conventions and file organization.
