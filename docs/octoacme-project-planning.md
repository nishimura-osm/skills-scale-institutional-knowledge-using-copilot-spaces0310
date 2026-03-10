# OctoAcme — Project Planning

## Purpose
Turn an approved initiative into an actionable plan and backlog for delivery.

## Objectives
- Break work into shippable increments
- Identify dependencies and risks
- Align timelines, releases, and responsibilities

## Activities
1. Kickoff meeting with stakeholders and delivery team
2. Create prioritized backlog with acceptance criteria
3. Estimate scope (T-shirt sizing or story points)
4. Define Definition of Done (DoD) — use the template in `docs/templates/definition-of-done.md`
5. Identify dependencies and integration points
6. Create release plan and milestone map

## Backlog Item Template
- Title:
- Description:
- Acceptance criteria:
- Priority:
- Estimate:
- Owner:
- Related docs/links:

## Sprint / Iteration Planning
- Timebox planning to agreed sprint length
- Pull items that meet DoD and have clear acceptance criteria
- Ensure team capacity is respected

## Risk & Dependency Management

### Risk Register
Capture risks in the project's Risk Register (`docs/templates/risk-register.md`):
- ID, Description, Impact, Probability, Owner, Mitigation, Status
- Update status at every weekly sync.
- Link high-impact risks to GitHub Issues so they appear on the project board.

### Dependency Tracking
For each identified dependency:
1. **Document it**: Add a comment to the dependent issue with `Depends on #<issue-number>` and apply the `dependency` label.
2. **Project board field**: Set a custom "Blocked by" field on the project card with the upstream issue/team reference.
3. **Escalation**: Surface unresolved cross-team dependencies during the weekly delivery sync. If unresolved after one sync cycle, the PM escalates to the Product Lead.

### Blocker Escalation (time-based SLAs)
- **Day 0**: Blocker raised in daily standup; team attempts same-day resolution.
- **By Day 1 EOD** (Level 1): If unresolved, PM documents the blocker in the weekly status update and tags the owning team.
- **By Day 2 EOD** (Level 2): PM escalates to Product Lead and dependent team leads via direct message or dedicated channel.
- **By Day 3 EOD** (Level 3): PM escalates to Sponsor / leadership with a written impact summary.

See also: [Execution & Tracking — Blocker Escalation](octoacme-execution-and-tracking.md#blocker-escalation).

## Planning Checklist
- [ ] Project kickoff held
- [ ] Backlog prioritized and estimated
- [ ] Release timeline and milestones agreed
- [ ] Definition of Done documented (use `docs/templates/definition-of-done.md`)
- [ ] Dependencies identified, labeled, and linked in GitHub Issues
- [ ] Risk Register initialized (`docs/templates/risk-register.md`)
- [ ] Initial test plan / QA approach drafted
