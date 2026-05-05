# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Operational Readiness Checklist

Complete before every production release to confirm the team is prepared to operate and support the new functionality:

- [ ] Runbook created or updated for new/changed features
- [ ] Monitoring dashboards updated to include new signals and thresholds
- [ ] Alerts configured (latency, error rate, availability) with appropriate owners
- [ ] Support Engineer briefed and knowledge base updated
- [ ] Customer-facing communications drafted and approved (if user-visible change)
- [ ] Rollback procedure documented and tested
- [ ] On-call rotation confirmed for the release window and 48 hours post-release
- [ ] Dependencies (third-party services, feature flags, config changes) verified ready

## Post-Release Validation Responsibilities

| Responsibility | Owner | Timeline |
|---|---|---|
| Smoke test critical user paths in production | QA Lead + Developer | Within 1 hour of deploy |
| Monitor error rates and latency dashboards | Developer (on-call) | First 2 hours |
| Confirm no spike in support tickets | Support Engineer | First 24 hours |
| Verify feature flag gradual rollout (if applicable) | Developer + Product Manager | Per rollout plan |
| Send release announcement to stakeholders | Project Manager | Within 4 hours of deploy |
| Post-release support review meeting | Project Manager | 24–48 hours post-release |
| Retrospective on release process (for major releases) | Project Manager | Within one week |

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
