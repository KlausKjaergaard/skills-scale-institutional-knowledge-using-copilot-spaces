# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — facilitated by **Scrum Master**; focus on progress, blockers, dependencies
- Weekly delivery sync — **Project Manager** and **Scrum Master** review progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone — **Scrum Master** facilitates with **Key Stakeholders** invited to provide feedback
- Sprint retrospectives — led by **Scrum Master** to identify and action process improvements

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
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
- Level 1: Team-level triage in daily standup (owned by **Scrum Master**)
- Level 2: PM escalates to Product Lead and dependent teams; **Scrum Master** coordinates resolution within the team
- Level 3: Sponsor-level escalation for business-impacting issues (via **Key Stakeholder Groups**)

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled (Scrum Master to facilitate)
- [ ] Risk register updated weekly
- [ ] Scrum Master assigned and agile ceremonies running
- [ ] UX Designer reviewing implemented features against design specs
