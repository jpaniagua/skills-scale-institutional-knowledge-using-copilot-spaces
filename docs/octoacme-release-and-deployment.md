# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
  - **Business Analyst**: Validates all requirements are satisfied
  - **UX Designer**: Confirms user experience meets design standards
- Passing CI and security scans
  - **Security Lead**: Reviews and approves security scan results
  - **DevOps Engineer**: Ensures all automated checks pass
- Release notes drafted
  - **Technical Writer**: Creates comprehensive release notes and user-facing documentation
- Rollback / mitigation plan documented
  - **DevOps Engineer**: Prepares rollback procedures and infrastructure changes
- Smoke tests prepared
  - **QA**: Defines and documents smoke test scenarios

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
  - **DevOps Engineer**: Creates backups and validates restore procedures
- [ ] Deploy to staging and run smoke tests
  - **DevOps Engineer**: Executes deployment
  - **QA**: Runs smoke tests
  - **UX Designer**: Validates critical user flows
- [ ] Deploy to production (automated pipeline preferred)
  - **DevOps Engineer**: Monitors deployment and system metrics
- [ ] Run post-deploy verifications
  - **Security Lead**: Validates security controls are functioning
  - **Business Analyst**: Confirms business-critical workflows operate correctly
- [ ] Announce release to stakeholders and support
  - **Technical Writer**: Distributes release notes and documentation
  - **PM**: Coordinates stakeholder communication

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - **DevOps Engineer**: Executes rollback procedures or implements fixes
  - **Security Lead**: Involved for security-related incidents
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items
  - **Technical Writer**: Documents incident timeline and lessons learned

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
