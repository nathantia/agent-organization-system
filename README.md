# Agent Organization System

A composable, GitHub-native framework for building agent teams around a goal.

Instead of treating every prompt as a one-off, this repository separates **who does the work**, **how capabilities are performed**, **who works together**, and **how a specific project executes**.

## Core model

```text
GOAL
  ↓
WORKFLOW ARCHITECT
  ↓
TEAM
  ↓
ROLES
  ↓
SKILLS
  ↓
WORKFLOW
  ↓
ARTIFACTS
  ↓
DELIVERABLE
```

## Concepts

- **Role** — who does the work.
- **Skill** — how a reusable capability is performed.
- **Team** — who should work together.
- **Workflow** — when work happens, dependencies, artifacts, and quality gates.
- **Architect** — decides which teams, roles, and skills are required for a goal.

## Repository structure

```text
architects/   meta-agents that design systems of work
roles/        reusable specialist and leadership agents
skills/       focused reusable capabilities
teams/        reusable team compositions
workflows/    project-specific or example workflows
templates/    authoring templates for new components
```

## Example

A request like:

> Conduct consumer research on apparel to identify emerging behaviors, unmet needs, and market opportunities.

might cause the Workflow Architect to assemble:

```text
Research Lead
├── Consumer Researcher
├── Cultural Strategist
└── Competitive Intelligence Analyst

Synthesis Strategist
└── Red Team Reviewer
```

The architect then generates a project-specific `workflow.md` with responsibilities, artifacts, dependencies, handoffs, quality gates, and stopping rules.

## Design principles

1. Use the smallest effective team.
2. Reuse existing roles and skills before creating new ones.
3. Keep roles, skills, teams, and workflows separate.
4. Design around durable artifacts rather than conversational memory.
5. Make handoffs and approval authority explicit.
6. Preserve evidence lineage for research-heavy work.
7. Separate facts, inferences, hypotheses, and recommendations.
8. Add independent critique when stakes justify it.
9. Treat teams as adaptable patterns, not rigid org charts.
10. Optimize for decision sufficiency, not endless research.

## Version

Current release: **v0.1.0**

This first release establishes the ontology, Workflow Architect, starter role library, starter skills, two team archetypes, and authoring templates.
