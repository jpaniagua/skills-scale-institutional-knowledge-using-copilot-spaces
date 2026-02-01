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
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support, security)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status
- Coordinate with Technical Writer for external communications
- Include Security Lead in communications about security-related changes
- Ensure UX Designer communicates design decisions to stakeholders

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
- Involve Security Lead for security incidents
- Engage DevOps Engineer for infrastructure incidents
- Update Technical Writer for public-facing incident communications

## Escalation Paths
- Team-level -> Scrum Master (if using Agile) -> PM -> Product Lead -> Sponsor
- For security incidents, follow the security incident runbook and notify Security Lead and on-call
- For infrastructure issues, escalate to DevOps Engineer and PM
- For design or UX concerns, coordinate with UX Designer and Product Manager
