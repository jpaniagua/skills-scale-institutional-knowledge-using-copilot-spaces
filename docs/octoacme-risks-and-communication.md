# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner (may include specialized roles: Security Lead for security risks, DevOps Engineer for infrastructure risks, UX Designer for usability risks)
- Mitigation plan
- Status

## Risk Lifecycle
- Identify: during planning and ongoing execution
  - **Security Lead**: Identifies security and compliance risks
  - **DevOps Engineer**: Identifies infrastructure and deployment risks
  - **UX Designer**: Identifies usability and accessibility risks
  - **Business Analyst**: Identifies requirement and business process risks
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status
  - **Scrum Master**: Ensures risks are tracked and escalated appropriately

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
  - **Technical Writer**: Ensures stakeholder communications are clear and well-structured
  - **Business Analyst**: Tailors communication to business stakeholder needs
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status
  - **Technical Writer**: Maintains centralized documentation

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
- **DevOps Engineer**: Leads technical incident response and recovery
- **Security Lead**: Leads security incident response and forensics
- **Technical Writer**: Documents incident communications and postmortems

## Escalation Paths
- Team-level -> PM -> Product Lead -> Sponsor
- For security incidents, follow the security incident runbook and notify Security Lead and Security on-call
- For infrastructure incidents, escalate to DevOps Engineer and on-call rotation
- For critical UX issues impacting release, escalate to UX Designer and Product Lead
