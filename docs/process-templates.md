# OctoAcme Process Templates

## Purpose
This document provides reusable templates and checklists to standardize common project activities across OctoAcme teams. Copy and paste these templates as needed to maintain consistency and reduce onboarding time.

---

## Weekly Status Template

Use this template for regular status updates to stakeholders. Paste into project README, meeting notes, or status update channels.

```markdown
### Weekly Status — [Week of YYYY-MM-DD]

**Progress this week:**
- [Key accomplishments and completed work items]
- [Metrics/milestones achieved]

**Next steps:**
- [Planned work for upcoming week]
- [Key deliverables and dates]

**Risks & blockers:**
- [Current risks with severity and mitigation plans]
- [Blockers requiring escalation or external help]

**Ask / decisions needed:**
- [Specific questions or decisions requiring stakeholder input]
- [Resource requests or approvals needed]
```

**How to use:**
- Update weekly (typically Friday or Monday)
- Share with PM, stakeholders, and project channel
- Keep concise and action-oriented
- Escalate blockers proactively

---

## Pull Request Checklist

Use this checklist in your PR description to ensure completeness before requesting review. This helps reviewers and speeds up the review process.

```markdown
## Pull Request Checklist

**Context:**
- Closes #[issue-number]
- [Brief description of changes and why they're needed]

**Changes:**
- [Summary of technical changes made]
- [Any architectural decisions or trade-offs]

**Testing:**
- [ ] Unit tests added/updated
- [ ] Integration tests added/updated where applicable
- [ ] Manual testing completed
- [ ] All tests passing locally

**Quality:**
- [ ] Code follows project style guidelines
- [ ] Documentation updated (README, API docs, comments)
- [ ] No new linting errors or warnings
- [ ] CI pipeline passing
- [ ] Security scan passing (no new vulnerabilities)

**Review Readiness:**
- [ ] PR is <= 400 lines (or split into smaller PRs with explanation)
- [ ] Breaking changes documented in description
- [ ] Changelog/release notes updated if applicable
- [ ] Screenshots/demos included for UI changes
- [ ] Migration steps documented if needed

**Reviewers:** @[reviewer-handles]

**Additional Notes:**
[Any context reviewers should know, areas needing extra attention, or follow-up work planned]
```

**How to use:**
- Copy this template into your PR description
- Check off items as you complete them
- Add the template to your repository's `.github/pull_request_template.md` for automatic inclusion
- Customize for your team's specific requirements

---

## Release Checklist / Smoke Test Template

Use this template to prepare for releases and verify deployments. This augments the guidance in `octoacme-release-and-deployment.md`.

```markdown
## Release Checklist — [Release Name/Version]

**Release Information:**
- **Release Version:** [e.g., v1.2.0]
- **Release Date:** [YYYY-MM-DD]
- **Release Type:** [Patch / Minor / Major]
- **Release Manager:** [@handle]

### Pre-Release
- [ ] All acceptance criteria met and PRs merged
- [ ] CI/CD pipeline passing (all tests, lints, security scans)
- [ ] Release notes drafted and reviewed
- [ ] Migration steps documented (if applicable)
- [ ] Rollback plan documented
- [ ] Deployment window scheduled (if needed)
- [ ] Stakeholders notified of release timeline
- [ ] Support team briefed on changes

### Deployment
- [ ] Backup/snapshot created (if applicable)
- [ ] Deploy to staging environment
- [ ] Smoke tests passed on staging
- [ ] Deploy to production (via automated pipeline)
- [ ] Verify deployment completed successfully

### Post-Deployment Verification (Smoke Tests)
- [ ] Application starts and is accessible
- [ ] Critical user flows functional (login, core features)
- [ ] API endpoints responding correctly
- [ ] Database migrations applied successfully
- [ ] Monitoring and alerting operational
- [ ] No critical errors in logs
- [ ] Performance metrics within acceptable range

### Post-Release
- [ ] Release notes published
- [ ] Stakeholders and support team notified of completion
- [ ] Known issues documented
- [ ] Monitoring dashboard reviewed for anomalies
- [ ] Rollback plan ready if issues arise

### Rollback Procedure (if needed)
1. [Step-by-step rollback instructions]
2. [Communication plan during rollback]
3. [Post-rollback verification steps]

**Notes:**
[Additional context, known issues, or special considerations for this release]
```

**How to use:**
- Create a release checklist issue or document for each release
- Use during release planning meetings
- Assign checklist items to specific team members
- Review and update smoke test items based on your application's critical paths
- Archive completed checklists for retrospectives and process improvement

---

## Additional Templates

### Decision Log Entry
When making significant technical or product decisions, document them for future reference:

```markdown
**Decision:** [One-line summary]
**Date:** [YYYY-MM-DD]
**Participants:** [@handles]
**Context:** [Why this decision was needed]
**Options Considered:** [Alternative approaches evaluated]
**Decision:** [What was decided and why]
**Consequences:** [Expected impact and trade-offs]
**Status:** [Proposed / Accepted / Deprecated]
```

### Incident Summary
For post-incident documentation:

```markdown
**Incident:** [Brief title]
**Severity:** [Critical / High / Medium / Low]
**Start Time:** [YYYY-MM-DD HH:MM UTC]
**Resolution Time:** [YYYY-MM-DD HH:MM UTC]
**Impact:** [User impact, affected systems]
**Root Cause:** [What caused the incident]
**Resolution:** [How it was fixed]
**Action Items:** [Follow-up tasks to prevent recurrence]
**Retrospective:** [Link to blameless retrospective doc]
```

---

## Template Customization Guide

### Adapting Templates for Your Team
- Add team-specific checklist items
- Adjust severity levels and escalation paths
- Include links to team-specific tools and dashboards
- Modify based on retrospective feedback

### Where to Store Templates
- **PR Template**: `.github/pull_request_template.md` in your repository
- **Issue Templates**: `.github/ISSUE_TEMPLATE/` directory
- **Release Checklists**: Release issue template or release tracking document
- **Status Updates**: Project README or team wiki
- **Decision Logs**: `docs/decisions/` directory (using ADR format)

### Keeping Templates Updated
- Review templates during retrospectives
- Update based on process improvements
- Version control templates alongside code
- Communicate changes to the team

---

## Related Documentation
- [OctoAcme Execution & Tracking](octoacme-execution-and-tracking.md) - Day-to-day workflow guidance
- [OctoAcme Release & Deployment](octoacme-release-and-deployment.md) - Release process details
- [OctoAcme Risk Management & Communication](octoacme-risks-and-communication.md) - Communication strategies
- [OctoAcme Roles & Personas](octoacme-roles-and-personas.md) - Team role definitions
