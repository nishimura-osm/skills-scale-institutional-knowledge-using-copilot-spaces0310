# Release Readiness Checklist

## Purpose
Confirm that all pre-release conditions are satisfied **before** the deployment window opens. Complete this checklist in a dedicated GitHub Issue (tagged `release`) and link it to the release PR.

## How to use
1. Open a new GitHub Issue titled `Release Readiness — vX.Y.Z` and paste this checklist.
2. Assign the Release Manager (typically the PM) as the owner.
3. Work through each section before triggering the deployment pipeline.
4. After deployment, complete the **Post-Release Verification** section.

---

## Pre-Deployment Readiness

### Code & Quality
- [ ] All planned PRs merged to the release branch
- [ ] All items in the release scope meet the [Definition of Done](definition-of-done.md)
- [ ] No open critical or high-severity bugs in scope
- [ ] CI pipeline is green (tests, lint, security scan)
- [ ] Dependency and license scan completed

### Documentation & Communication
- [ ] Release notes drafted and reviewed (`See` [Release Notes Template](../octoacme-release-and-deployment.md))
- [ ] Internal stakeholder notification sent (or scheduled)
- [ ] Support team briefed on new features and known issues
- [ ] Public changelog or release page updated (if applicable)

### Infrastructure & Operations
- [ ] Deployment window confirmed with on-call team
- [ ] Staging deployment successful and smoke tests passed
- [ ] Database migrations tested in staging (if applicable)
- [ ] Feature flags configured correctly for rollout strategy
- [ ] Rollback plan documented and tested
- [ ] Monitoring alerts and dashboards updated for new signals

### Approvals
- [ ] PdM sign-off received
- [ ] PM sign-off received
- [ ] Security review completed (for changes touching auth/data)

---

## Deployment Checklist

- [ ] Deployment window open; on-call notified
- [ ] Backup or snapshot taken (if applicable)
- [ ] Deploy to staging — smoke tests passed
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Post-deploy verifications complete (see section below)
- [ ] Release announcement sent to stakeholders and support

---

## Post-Release Verification

Complete within **2 hours** of production deployment:

- [ ] Key user journeys verified in production (smoke test)
- [ ] Error rates are within expected baseline (check dashboard/alerts)
- [ ] Latency / performance metrics within SLA
- [ ] No unexpected spike in support tickets or alerts
- [ ] Feature flags set to intended production state
- [ ] Release issue updated with deployment timestamp and status

If any verification item fails, follow the [Rollback & Incident Playbook](../octoacme-release-and-deployment.md#rollback--incident-playbook).

---

## Post-Release Communication

- [ ] "Release complete" message sent to stakeholders (Slack / email)
- [ ] Support and customer-facing teams notified with user-facing summary
- [ ] Release retrospective or brief debrief scheduled (for Major releases)
