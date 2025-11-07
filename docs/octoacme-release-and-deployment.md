# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Manager Role
The Release Manager coordinates all aspects of the release process, from planning through deployment. They maintain the release calendar, verify that all pre-release requirements are met, coordinate deployment activities across teams, and ensure smooth rollouts with minimal risk. The Release Manager serves as the central point of contact for release status and is responsible for initiating rollback procedures if issues arise during deployment.

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

## Release Calendar
The Release Manager owns and maintains the release calendar, which tracks all planned and scheduled releases. Each release entry should include a release name or number, target date, release owner, release type (patch/minor/major), rollback plan reference, and any special notes. Teams should record upcoming releases in the calendar as early as possible during sprint planning to ensure visibility and coordination across stakeholders.

**Release entry template:**
- **Release name/number:** e.g., v2.3.0
- **Target date:** YYYY-MM-DD
- **Owner:** Name or team responsible for the release
- **Release type:** Patch / Minor / Major
- **Rollback plan:** Link to documented rollback procedure
- **Notes:** Special considerations, dependencies, or deployment windows

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Release Manager verifies staging readiness
- [ ] Release notes and rollback plans published
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

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
