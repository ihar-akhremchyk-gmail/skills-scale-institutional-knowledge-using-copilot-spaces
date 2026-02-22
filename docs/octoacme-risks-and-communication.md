# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

## Communication Templates
Weekly Status Template:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:

Incident Communication
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled

## Escalation Paths
- Team-level -> PM -> Product Lead -> Sponsor
- For security incidents, follow the security incident runbook and notify Security on-call

## Security Lead Integration
- The Security Lead is the owner of the security risk register and security-related escalations
- Security reviews are required before releasing any feature with data handling, authentication, or infrastructure changes
- Security Lead participates in weekly risk register reviews and flags any changes in security posture

## Security Review Checklist
- [ ] Threat model reviewed or updated for the feature/change
- [ ] CI security scan results triaged (no unaccepted critical or high findings)
- [ ] Compliance requirements verified (e.g., data retention, access controls)
- [ ] Incident response runbook up to date
- [ ] Security Lead sign-off recorded in the release doc
