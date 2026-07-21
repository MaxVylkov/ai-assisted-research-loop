# AI-Assisted Research Loop

A reusable Codex skill for structuring scientific research ideas into a reproducible workflow.

The skill guides an AI assistant through a disciplined research cycle:

```text
hypothesis -> literature check -> minimal model -> rough estimate -> numerical calculation -> systematics/backgrounds -> internal review -> decision -> write-up
```

It is intended for scientific planning, feasibility checks, technical literature work, calculation notes, analytical memos, and research-oriented Obsidian workflows.

## What This Skill Helps With

- Turn a broad research idea into a concrete investigation plan.
- Separate hypothesis, model assumptions, calculations, uncertainties, and conclusions.
- Run quick feasibility/no-go checks before investing time in a detailed study.
- Keep experiment and calculation logs reproducible.
- Ask the assistant to critique a result before turning it into a memo, paper section, or slide deck.

## Installation

Copy the skill folder into your Codex skills directory:

```bash
cp -R ai-assisted-research-loop ~/.codex/skills/
```

Then start a new Codex session and ask:

```text
Use ai-assisted-research-loop to structure this research question.
```

## Example Prompts

```text
Use ai-assisted-research-loop to evaluate whether this detector concept is feasible.
```

```text
Run this idea through the research loop and identify the weakest assumptions.
```

```text
Use the short mode of ai-assisted-research-loop for an early no-go check.
```

```text
Apply the research loop to turn these notes into a calculation plan.
```

## Repository Structure

```text
.
├── README.md
├── LICENSE
└── ai-assisted-research-loop/
    ├── SKILL.md
    └── agents/
        └── openai.yaml
```

## License

MIT License.
