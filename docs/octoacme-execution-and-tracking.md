# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Board Stage Definitions

Use the project board (e.g., GitHub Projects) with columns: **Backlog → Ready → In Progress → In Review → QA → Done**.

| Stage | Meaning | Entry Criteria |
|---|---|---|
| **Backlog** | Work identified but not yet scheduled | Issue exists; rough description present |
| **Ready** | Prioritized and prepared for a developer to start | Acceptance criteria written; designs attached (if applicable); estimates agreed; no unresolved blockers |
| **In Progress** | Actively being implemented | Developer assigned; branch created; regular standup updates |
| **In Review** | Code complete; awaiting peer review | PR open; CI passes; self-tested in dev environment; PR description links issue |
| **QA** | In testing by QA Lead | Deployed to staging; Dev → QA handoff checklist complete (see [Ownership & Handoffs](octoacme-ownership-and-handoffs.md)) |
| **Done** | Shipped or accepted | All acceptance criteria verified; QA sign-off received; merged and deployed (or ready for scheduled release) |

### Definition of Ready Checklist

Before moving an item from Backlog → Ready:

- [ ] Problem statement and user story written
- [ ] Acceptance criteria defined (specific, testable, agreed by Product Manager and QA Lead)
- [ ] UX designs attached or linked (if UX work required)
- [ ] Dependencies identified and resolved (or explicitly deferred with a plan)
- [ ] Work estimated by the team
- [ ] No open blockers

### Definition of Done Checklist

Before moving an item from QA → Done:

- [ ] All acceptance criteria verified by QA Lead
- [ ] Automated tests written and passing (unit + integration as applicable)
- [ ] No P1/P2 defects open (exceptions documented and approved)
- [ ] Code reviewed and merged
- [ ] Documentation updated (if user-facing or API changes)
- [ ] Release notes entry added
- [ ] Monitoring / alerting updated if new signals introduced
- [ ] Support Engineer notified of changes (if customer-visible)

## Pull Request Workflow
- Small PRs (<= 400 lines when possible)
- Include issue link and acceptance criteria in PR description
- Run automated tests and linting in CI before requesting review
- Require at least one approval before merging (or team-defined policy)

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
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
