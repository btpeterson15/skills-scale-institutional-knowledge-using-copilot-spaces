# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability. The **Release Coordinator** is accountable for orchestrating the entire release process and ensuring successful deployments.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged (verified by Project Manager)
- Passing CI and security scans (monitored by QA Lead)
- **QA Sign-off obtained** (Quality Assurance Lead accountable)
- Release notes drafted (Release Coordinator responsible)
- Rollback / mitigation plan documented (Release Coordinator responsible)
- Smoke tests prepared (QA Lead coordinates)

## Deployment Checklist
**Release Coordinator** manages this checklist and coordinates execution:
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests (coordinate with QA Lead)
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications (coordinate with QA Lead and DevOps)
- [ ] Announce release to stakeholders and support (coordinate with Stakeholder Liaison)

For detailed release coordination handoffs, see [Role Collaboration Checklist](./octoacme-role-collaboration-checklist.md).

## Rollback & Incident Playbook
If a deployment fails or causes a critical issue:
- **Release Coordinator** triggers incident response and notifies on-call
- Rollback to last known-good release if necessary (Release Coordinator coordinates)
- Triage root cause and capture action items (Project Manager facilitates)
- Stakeholder Liaison updates affected stakeholders on status

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
