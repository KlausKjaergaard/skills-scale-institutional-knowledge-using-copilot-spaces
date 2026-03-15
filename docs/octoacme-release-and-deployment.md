# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Manager Responsibilities
The **Release Manager** owns the end-to-end release process and is accountable for:
- Maintaining the release calendar and coordinating deployment windows with engineering and operations
- Running release readiness reviews to confirm all criteria are met before deployment
- Ensuring release notes, runbooks, and rollback plans are prepared and approved
- Communicating release schedules, changes, and outcomes to stakeholders and support teams
- Overseeing post-release verification and coordinating incident response if issues arise

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted (owned by **Release Manager**)
- Rollback / mitigation plan documented and reviewed
- Smoke tests prepared
- Stakeholder approval obtained for major or breaking releases (**Key Stakeholder Groups**)
- Release Manager sign-off confirming all readiness criteria are met

## Deployment Checklist
- [ ] Release Manager has confirmed readiness criteria are met
- [ ] Deployment window scheduled and communicated (Release Manager)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support (Release Manager)

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
