# AI-Assisted Research Loop

Turn rough scientific ideas into reproducible research plans.

**AI-Assisted Research Loop** is a small reusable Codex skill for using an AI assistant as a disciplined research partner: not just to generate prose, but to structure hypotheses, check literature, build minimal models, estimate orders of magnitude, track uncertainty, critique conclusions, and produce a clean write-up.

The skill guides an AI assistant through a disciplined research cycle:

```text
hypothesis -> literature check -> minimal model -> rough estimate -> numerical calculation -> systematics/backgrounds -> internal review -> decision -> write-up
```

It is intended for scientific planning, feasibility checks, technical literature work, calculation notes, analytical memos, and research-oriented Markdown/Obsidian workflows.

The skill is inspired by the agentic research workflow discussed in Lu et al., **"Towards end-to-end automation of AI research"**, *Nature* 651, 914-919 (2026): https://doi.org/10.1038/s41586-026-10265-5

## Why This Exists

AI systems are increasingly good at helping with individual research tasks: literature search, code, calculations, drafting, and review. The hard part is keeping the process intellectually honest.

This skill gives the assistant a repeatable research protocol:

- state the hypothesis before calculating;
- check whether the idea already exists;
- build the smallest useful model;
- do a rough estimate before detailed work;
- separate signal from background and result from assumption;
- critique the conclusion before turning it into text.

## What This Skill Helps With

- Turn a broad research idea into a concrete investigation plan.
- Separate hypothesis, model assumptions, calculations, uncertainties, and conclusions.
- Run quick feasibility/no-go checks before investing time in a detailed study.
- Keep experiment and calculation logs reproducible.
- Ask the assistant to critique a result before turning it into a memo, paper section, or slide deck.

## When To Use It

Use this skill when you want to:

- evaluate whether a research idea is worth pursuing;
- turn scattered notes into a calculation plan;
- prepare an analytical memo, paper section, or talk outline;
- identify weak assumptions before presenting a result;
- maintain an Obsidian or Markdown-based research graph;
- run a fast feasibility/no-go check.

## Installation

Clone the repository:

```bash
git clone https://github.com/MaxVylkov/ai-assisted-research-loop.git
```

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

## What The Assistant Will Do

When triggered, the assistant should walk through the research loop:

1. formulate the question and hypothesis;
2. check prior literature or supplied sources;
3. define a minimal model;
4. estimate the order of magnitude;
5. plan or run a reproducible calculation;
6. identify systematics and backgrounds;
7. review the result skeptically;
8. decide whether to continue, revise, park, or treat as no-go;
9. convert the result into a persistent note or write-up.

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
