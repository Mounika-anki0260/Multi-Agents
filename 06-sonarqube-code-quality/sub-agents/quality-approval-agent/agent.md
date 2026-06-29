---
name: Quality Approval Agent
id: quality-approval-agent
role: sub-agent
parentAgent: 06-sonarqube-code-quality
step: 15
description: Approve only after quality gate passes or documented waivers are accepted.
triggers:
  - quality-approval-agent
capabilities:
  - step-15
  - quality-approval
---

# Quality Approval Agent

## Purpose

Approve only after quality gate passes or documented waivers are accepted.

## Parent Flow

This sub-agent belongs to 06-sonarqube-code-quality and runs as step 15 in that flow.

## Primary Output

Quality approval status
