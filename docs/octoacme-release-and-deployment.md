# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Roles & Accountability

| Role | Responsibility |
|---|---|
| Release Manager | Owns the release checklist, coordinates go/no-go, and leads rollback decisions |
| DevOps Engineer | Executes and monitors the deployment pipeline |
| Quality Advocate | Confirms all acceptance criteria and smoke tests pass before release |
| Security Lead | Validates that security scans are green and known risks are accepted |
| Technical Writer | Publishes release notes and updates relevant documentation |
| Stakeholder Champion | Distributes release announcements and collects stakeholder feedback |

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

## Deployment Checklist
- [ ] Release Manager: deployment window scheduled and communicated
- [ ] DevOps Engineer: backup or snapshot taken (if applicable)
- [ ] DevOps Engineer: deploy to staging and run smoke tests
- [ ] Quality Advocate: smoke test results reviewed and approved
- [ ] Security Lead: security scan results reviewed and accepted
- [ ] Release Manager: go/no-go decision confirmed
- [ ] DevOps Engineer: deploy to production (automated pipeline preferred)
- [ ] DevOps Engineer: run post-deploy verifications
- [ ] Release Manager / Stakeholder Champion: announce release to stakeholders and support

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
