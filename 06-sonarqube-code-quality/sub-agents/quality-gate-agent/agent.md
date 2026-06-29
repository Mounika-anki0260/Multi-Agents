---
name: Quality Gate Agent
id: quality-gate-agent
role: sub-agent
parentAgent: 06-sonarqube-code-quality
step: 4
description: Configure quality gate conditions for reliability, security, maintainability, coverage, duplication, and new-code policy.
triggers:
  - quality-gate-agent
capabilities:
  - step-4
  - quality-gate
---

# Quality Gate Agent

## Purpose

Configure quality gate conditions for reliability, security, maintainability, coverage, duplication, and new-code policy.

## Parent Flow

This sub-agent belongs to 06-sonarqube-code-quality and runs as step 4 in that flow.

## Primary Output

Quality gate definition
