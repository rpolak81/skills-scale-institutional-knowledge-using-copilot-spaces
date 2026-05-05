# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## UX Designer

### Role Summary
UX Designers create intuitive, user-centered experiences. They translate user research and product requirements into wireframes, prototypes, and interaction patterns that developers can build from.

### Responsibilities
- Conduct user research, interviews, and usability testing
- Produce wireframes, mockups, and interactive prototypes
- Define interaction patterns, accessibility requirements, and design standards
- Collaborate on acceptance criteria related to user experience
- Review implemented features to verify design fidelity

### Goals
- Ensure every feature is easy to use and meets accessibility standards
- Reduce rework caused by late-stage usability issues
- Build a shared design language across the product

### Typical Communication
- Design reviews and critiques with Product Managers and Developers
- Usability test reports shared with the full team
- Design handoff documentation (Figma, Storybook, or similar)

### Interactions with Existing Roles
- **Product Managers**: Align on user stories, success metrics, and acceptance criteria; participate in backlog refinement to ensure UX requirements are captured early.
- **Developers**: Hand off designs with annotated specs; review in-progress and completed implementations; surface design-to-implementation gaps before QA.
- **Project Managers**: Flag design-related dependencies or blockers; provide estimates for discovery and design tasks during planning.

---

## Data Analyst

### Role Summary
Data Analysts gather, interpret, and communicate data insights that inform product decisions, measure outcomes, and surface improvement opportunities across the project lifecycle.

### Responsibilities
- Define and maintain key metrics aligned to project success criteria
- Build and maintain dashboards for product and delivery health
- Analyze usage data and provide insights during planning and retrospectives
- Support A/B test design, execution, and analysis
- Identify data quality issues and work with engineering to resolve them

### Goals
- Enable data-driven decision-making at every stage
- Make project health and product impact visible to stakeholders
- Reduce guesswork in prioritization and post-release evaluation

### Typical Communication
- Metrics reports shared with Product Managers and Project Managers
- Dashboard walkthroughs during sprint reviews and retrospectives
- Ad-hoc analysis in response to incidents or feature launches

### Interactions with Existing Roles
- **Product Managers**: Partner on defining success metrics for features; provide post-release data to evaluate outcomes and inform roadmap decisions.
- **Project Managers**: Supply delivery metrics (velocity, cycle time, defect rates) for status reports and retrospectives.
- **Developers**: Collaborate on instrumentation and data pipeline requirements; surface data quality issues that need engineering fixes.

---

## QA Lead

### Role Summary
The QA Lead owns the team's quality strategy, ensuring that features meet acceptance criteria and that risks are identified before they reach production. They coordinate testing across the delivery lifecycle and act as the quality gate between development and release.

### Responsibilities
- Define and maintain the test strategy (unit, integration, end-to-end, exploratory)
- Write, review, and maintain test plans and test cases
- Execute and coordinate manual and automated testing
- Manage defect tracking: log, triage, and verify bug fixes
- Own the Definition of Done criteria related to quality
- Collaborate with Developers on test automation and coverage targets
- Sign off on release readiness from a quality perspective

### Goals
- Prevent quality issues from reaching production
- Reduce the cost of defects through early detection
- Build sustainable test automation that supports continuous delivery

### Typical Communication
- Test plans and test results shared before and after each sprint
- Defect reports and triage in the issue tracker
- Release readiness sign-off communicated to the Project Manager and release team

### Interactions with Existing Roles
- **Product Managers**: Clarify acceptance criteria and edge cases; escalate scope gaps that risk quality; validate that user-facing behavior matches expectations.
- **Developers**: Review PRs for testability; pair on automated tests; reproduce and verify bug fixes; align on coverage standards.
- **Project Managers**: Provide quality metrics (pass rates, open defects, test coverage) for status updates; flag quality-related risks that may affect timelines.

---

## Support Engineer

### Role Summary
Support Engineers are the bridge between users and the development team after a feature ships. They handle incidents, escalate bugs, and channel customer pain points back into the planning cycle to drive continuous improvement.

### Responsibilities
- Triage and resolve incoming support tickets and incidents
- Reproduce reported issues and create detailed bug reports for engineering
- Maintain runbooks and troubleshooting guides for common issues
- Monitor alerts and escalate production incidents per the incident response playbook
- Participate in post-incident reviews and contribute to action items
- Provide customer feedback summaries during sprint retrospectives and planning

### Goals
- Minimize customer impact from production issues
- Reduce time-to-resolution for incidents and bug fixes
- Ensure operational knowledge is documented and accessible

### Typical Communication
- Incident reports and postmortems shared with Developers and Project Managers
- Weekly support summaries (ticket volume, top issues) shared with Product Managers
- Runbook and knowledge base updates in the project wiki or docs

### Interactions with Existing Roles
- **Product Managers**: Provide customer feedback and top-issue trends to inform prioritization; flag recurring pain points that warrant backlog items.
- **Developers**: Escalate confirmed bugs with reproduction steps; collaborate on hotfix prioritization; review runbooks for accuracy after releases.
- **Project Managers**: Report on support SLA health and open incident counts; raise operational risks before and after releases.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

