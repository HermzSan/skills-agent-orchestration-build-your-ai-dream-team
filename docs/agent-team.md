# Agent team

For Mona's Project Pulse dashboard, I am using a four-agent custom team defined under `.github/agents/` and orchestrated through GitHub Copilot CLI in a Codespace.

- Planner — Model: Claude Opus 5.5 (copilot) — researches the repo, docs, and dependencies to produce a practical implementation plan and file assignments. Definition: `.github/agents/planner.agent.md`
- Coder — Model: GPT-5.5 (copilot) — implements the assigned code changes, fixes bugs, and validates behavior within the orchestrated file scope. Definition: `.github/agents/coder.agent.md`
- Designer — Model: Gemini 3.7 Flash (copilot) — focuses on UI/UX, accessibility, visual hierarchy, interaction flow, and the polished Project Pulse dashboard styling. Definition: `.github/agents/designer.agent.md`
- Orchestrator — Model: Claude Opus 5.5 (copilot) — breaks work into phases, delegates to the specialist agents, coordinates parallel work when safe, and verifies the final integration. Definition: `.github/agents/orchestrator.agent.md`

This setup keeps planning, implementation, design, and project coordination separate while using GitHub Copilot CLI in a Codespace to manage the end-to-end build flow.
