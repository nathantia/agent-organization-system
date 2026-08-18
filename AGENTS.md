# Agent System Instructions

This repository is an agent organization library.

When asked to build a workflow:

1. Read `architects/workflow-architect/AGENT.md`.
2. Search `teams/` for an existing team pattern.
3. Search `roles/` for reusable specialists.
4. Search `skills/` for reusable capabilities.
5. Reuse existing components when they fit.
6. Create project-local components only when a genuine capability gap exists.
7. Generate a project-specific `workflow.md`.
8. Do not execute the full project unless explicitly asked after the workflow is designed.

## Ontology

- `ROLE.md` = who does the work.
- `SKILL.md` = how a capability is performed.
- `TEAM.md` = who works together.
- `workflow.md` = how one project executes.
- `AGENT.md` = meta-agent or orchestrator behavior.
