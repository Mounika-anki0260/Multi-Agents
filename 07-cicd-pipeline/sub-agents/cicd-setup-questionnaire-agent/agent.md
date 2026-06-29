---
name: Cicd Setup Questionnaire Agent
id: cicd-setup-questionnaire-agent
role: sub-agent
parentAgent: 07-cicd-pipeline
step: 1
description: Ask CI/CD platform, branch strategy, build/test commands, scans, artifact strategy, registry, environments, approvals, rollback, and notifications.
triggers:
  - cicd-setup-questionnaire-agent
capabilities:
  - step-1
  - cicd-setup-questionnaire
---

# Cicd Setup Questionnaire Agent

## Purpose

Ask CI/CD platform, branch strategy, build/test commands, scans, artifact strategy, registry, environments, approvals, rollback, and notifications.

## Parent Flow

This sub-agent belongs to 07-cicd-pipeline and runs as step 1 in that flow.

## Primary Output

CI/CD setup decisions
