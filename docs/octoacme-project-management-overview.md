# OctoAcme Project Management Overview

## Purpose
Provide a concise, shareable introduction to how OctoAcme runs projects so new teammates can quickly understand our approach, roles, and key artifacts.

## Scope
Applies to all cross-functional projects that deliver product features, services, or integrations.

## Principles
- Customer-first: prioritize customer value and usability.
- Iterative delivery: deliver small, testable increments.
- Clear ownership: each project has a named Project Manager (PM) and Product Lead.
- Data-informed decisions: measure impact and iterate based on evidence.
- Psychological safety: encourage feedback and learning.

## Core Roles
- Project Manager (PM): coordinates delivery, schedules, risk, communications.
- Product Manager (PdM): defines outcomes, prioritizes backlog, and measures success.
- Developers: implement features, collaborate on design and testability.
- QA/Testing: validate quality and acceptance criteria.
- Stakeholders: provide inputs and approvals.

## Key Artifacts

All artifacts live in `docs/` in the project repository. Reference them from issues and PRs using relative links (e.g., `See [Risk Register](docs/templates/risk-register.md)`).

| Artifact | Location |
|---|---|
| Project Charter / One-pager | `docs/octoacme-project-initiation.md` |
| Roadmap and Release Plan | `docs/octoacme-release-and-deployment.md` |
| Sprint/Iteration Backlog | GitHub Issues + project board |
| Acceptance Criteria & Definition of Done | `docs/templates/definition-of-done.md` |
| Risk Register | `docs/templates/risk-register.md` |
| Decision Log | `docs/templates/decision-log.md` |
| Weekly Status Update | `docs/templates/status-update-template.md` |
| Release Readiness Checklist | `docs/templates/release-readiness-checklist.md` |
| Retrospective Action Items | `docs/templates/retro-action-items.md` |

## Lifecycle (high-level)
1. Initiation: problem statement, stakeholders, high-level timeline.
2. Planning: scope, resources, milestones, dependencies.
3. Execution: build, test, review, iterate.
4. Release: deploy, verify, announce.
5. Close & Retrospective: capture learnings and next steps.

## Communication Cadence
- Weekly sync between PM + PdM
- Twice-weekly standups for delivery team (or as agreed)
- Monthly stakeholder updates
- Ad-hoc escalations as needed

## How to use these docs
- Keep the Project Charter updated in the project repo (see `docs/octoacme-project-initiation.md`).
- Add process-specific docs into `.copilot/` if you want Copilot Spaces to use them as context.
- All reusable templates live in `docs/templates/`. Copy them into issues, PRs, or dedicated project files as needed.
- Cross-phase references: Initiation → Planning → Execution → Release → Retrospective (see each doc for entry/exit criteria).
