# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged; items satisfy the [Definition of Done](templates/definition-of-done.md)
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared
- Release Readiness Checklist completed (see `docs/templates/release-readiness-checklist.md`)

## Deployment Checklist
- [ ] Release Readiness Checklist completed (`docs/templates/release-readiness-checklist.md`)
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications (see Post-Release Verification below)
- [ ] Announce release to stakeholders and support

## Post-Release Verification

Complete within **2 hours** of production deployment:

- [ ] Key user journeys verified in production (smoke test)
- [ ] Error rates within expected baseline (check dashboard/alerts)
- [ ] Latency / performance metrics within SLA
- [ ] No unexpected spike in support tickets or alerts
- [ ] Feature flags set to intended production state

If any item fails, follow the [Rollback & Incident Playbook](#rollback--incident-playbook).

## Post-Release Communication

- [ ] "Release complete" message sent to stakeholders (Slack / email)
- [ ] Support and customer-facing teams notified with user-facing summary
- [ ] Release retrospective or brief debrief scheduled (for Major releases)

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
