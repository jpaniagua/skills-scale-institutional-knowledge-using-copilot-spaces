# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans (verified by Security Lead)
- Release notes drafted (with support from Technical Writer)
- Rollback / mitigation plan documented
- Smoke tests prepared
- Infrastructure and deployment automation verified by DevOps Engineer

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable) — coordinated by DevOps Engineer
- [ ] Deploy to staging and run smoke tests
- [ ] Security verification completed by Security Lead
- [ ] Deploy to production (automated pipeline preferred) — managed by DevOps Engineer
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support
- [ ] Update documentation (Technical Writer)

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call (DevOps Engineer, Security Lead if security-related)
  - Rollback to last known-good release if necessary (executed by DevOps Engineer)
  - Triage root cause and capture action items
  - Conduct post-incident review with all relevant stakeholders

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
