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
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

### Pull Request & Branching Checklist

**Branch Naming Conventions:**
- `feature/` - New features (e.g., `feature/add-user-profile`)
- `fix/` - Bug fixes (e.g., `fix/login-timeout`)
- `chore/` - Maintenance tasks (e.g., `chore/update-dependencies`)
- `hotfix/` - Urgent production fixes (e.g., `hotfix/security-patch`)

**Pull Request Checklist:**
Before requesting review, ensure your PR includes:
- [ ] Links to related issue(s) and references acceptance criteria
- [ ] Unit tests added/updated for new logic
- [ ] Integration tests added where applicable
- [ ] Documentation updated (README, API docs, inline comments where needed)
- [ ] CI pipeline passing (tests, linting, security scans)
- [ ] PR is <= 400 lines when possible (split larger changes into multiple PRs)
- [ ] At least one reviewer assigned
- [ ] Changelog or release notes updated if applicable
- [ ] Breaking changes clearly documented

**Draft Pull Requests:**
- Use draft PRs for work in progress or to gather early feedback
- Mark as "Ready for Review" only when the checklist above is complete
- Draft PRs should still have CI passing before requesting review

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

**For incidents and production issues:**
- Involve Support Lead for customer-impacting incidents
- Involve DevOps/Platform Engineer for infrastructure or deployment issues
- Follow the incident response playbook (see Release & Deployment Guide)

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
