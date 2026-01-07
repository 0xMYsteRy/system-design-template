# Prompt Instructions

## Purpose
Use this project as a quick reference when composing prompts for system design work. The repository already contains reusable patterns, so this guide explains how to turn those assets into a clear ask for an LLM or a human reviewer.

## Workflow
1. **Identify the goal** – outline the product feature, scale targets, and key constraints you care about (e.g., latency, throughput, consistency).
2. **Pick a template** – browse the `docs/` directory, choose the closest system design template, and note its assumptions.
3. **Customize** – list the deltas between your scenario and the template (new data sources, SLAs, workloads).
4. **Ask for deliverables** – specify the artifacts you expect (diagram, component list, trade-offs, failure scenarios, cost estimates).
5. **Add guardrails** – mention technologies to include/exclude, depth of explanation, or formatting preferences.

## Prompt Skeleton
```
You are an experienced system architect.
Goal: <core feature and success metrics>.
Constraints: <throughput, latency, consistency, cost, compliance>.
Reference template: <name from docs/>. Key deltas: <list>.
Deliverables: <items such as architecture diagram description, component breakdown, scaling plan>.
Guardrails: <tech choices, level of detail, diagram format>.
```

## Tips
- Keep each constraint measurable (numbers beat adjectives).
- When unsure about trade-offs, ask for comparisons so you can choose.
- Reuse the same skeleton for follow-up prompts to stay consistent.
