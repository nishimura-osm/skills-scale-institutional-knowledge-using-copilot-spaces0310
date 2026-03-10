# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Paste the [Definition of Done checklist](templates/definition-of-done.md) into the PR and verify all items before requesting review
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Dependency & Blocker Handling
- Label blocked issues with `blocked` and add a comment: `Blocked by #<issue-number>` or `Blocked by <team/system>`.
- Set the "Blocked by" project board field to the upstream dependency reference.
- Raise blockers at the start of each daily standup so the full team is aware.
- Escalation SLAs (see also [Planning — Blocker Escalation SLAs](octoacme-project-planning.md#blocker-escalation-time-based-slas)):
  - **Day 0**: Team-level triage in daily standup.
  - **By Day 1 EOD** (Level 1): PM documents blocker in status update and notifies owning team.
  - **By Day 2 EOD** (Level 2): PM escalates to Product Lead and dependent team leads.
  - **By Day 3 EOD** (Level 3): PM escalates to Sponsor with written impact summary.

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1 — Day 0: Team-level triage in daily standup; attempt same-day resolution.
- Level 2 — By Day 1 EOD: PM documents blocker in status update; notifies owning team directly.
- Level 3 — By Day 2 EOD: PM escalates to Product Lead and dependent team leads.
- Level 4 — By Day 3 EOD: Sponsor-level escalation for business-impacting issues (written impact summary required).

For security incidents, follow the security incident runbook and notify Security on-call immediately (no SLA delay).

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Definition of Done checklist added to all active issues and PRs (`docs/templates/definition-of-done.md`)
- [ ] Blocked issues labeled `blocked` with upstream dependency noted
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly (`docs/templates/risk-register.md`)
