# Definition of Done (DoD) Checklist

## Purpose
A shared, reusable checklist that defines when a backlog item (story, task, or bug) is considered **complete**. Paste this checklist into GitHub Issues and PRs as a starting point, then add feature-specific acceptance criteria below it.

## How to use
1. Copy the **Standard DoD Checklist** section into every GitHub Issue or PR description.
2. Add any feature-specific acceptance criteria under the checklist.
3. All boxes must be checked before an item can move to **Done** on the project board.
4. The PM and PdM are responsible for confirming acceptance criteria are met before the sprint closes.

---

## Standard DoD Checklist

```markdown
### Definition of Done
- [ ] Code implemented and peer-reviewed (PR approved by ≥ 1 reviewer)
- [ ] All CI checks pass (tests, lint, security scan)
- [ ] Unit tests written for new logic (coverage not regressed)
- [ ] Integration/end-to-end tests added or updated where applicable
- [ ] Acceptance criteria below are all met and verified
- [ ] Documentation updated (inline comments, README, or relevant `docs/` file)
- [ ] No known critical/high severity bugs introduced
- [ ] Feature flag or rollback plan in place (for production-impacting changes)
- [ ] Demo'd to or signed off by PdM / stakeholder
```

---

## Acceptance Criteria Template

Use the format below when writing acceptance criteria for an issue or PR:

```markdown
### Acceptance Criteria
- [ ] Given <context>, when <action>, then <expected outcome>
- [ ] Given <context>, when <action>, then <expected outcome>
```

**Example**
```markdown
### Acceptance Criteria
- [ ] Given a logged-in user, when they submit the form, then a success toast appears within 2 seconds.
- [ ] Given an invalid email, when the user submits, then an inline validation error is shown.
```

---

## Sprint / Release-Level DoD

In addition to the per-item checklist above, the sprint or release is only done when:

- [ ] All committed items meet the per-item DoD above
- [ ] Release notes or changelog updated
- [ ] Smoke tests passed in staging
- [ ] Stakeholder demo completed (or recording shared)
- [ ] Retrospective scheduled (for sprint close) or completed (for release close)
