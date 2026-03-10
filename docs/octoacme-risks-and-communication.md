# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain the Risk Register in `docs/templates/risk-register.md` (copy into your project's `docs/` folder). The register is the single source of truth for project risks. Update it at every weekly sync and link high-impact risks to GitHub Issues.

Fields per risk:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Score (Impact × Likelihood)
- Owner
- Mitigation plan
- Status
- Last updated

See `docs/templates/risk-register.md` for the full template and scoring guide.

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

## Communication Templates

Use the Weekly Status Update template in `docs/templates/status-update-template.md`. Key sections:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:
- Metrics snapshot (velocity, open blockers, P0/P1 bugs)

For significant technical or architectural decisions, log them in `docs/templates/decision-log.md` and reference the log entry from the related issue or PR.

Incident Communication
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled

## Escalation Paths
- Team-level -> PM (Day 0) -> Product Lead (Day 2) -> Sponsor (Day 3)
- Time-based SLAs mirror those in [Execution & Tracking — Blocker Escalation](octoacme-execution-and-tracking.md#blocker-escalation).
- For security incidents, follow the security incident runbook and notify Security on-call immediately.
