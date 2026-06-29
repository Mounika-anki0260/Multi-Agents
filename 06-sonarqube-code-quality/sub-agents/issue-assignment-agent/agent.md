---
name: Issue Assignment Agent
id: issue-assignment-agent
role: sub-agent
parentAgent: 06-sonarqube-code-quality
step: 12
description: Assign issues to owners by module, severity, category, or responsible team.
triggers:
  - issue-assignment-agent
capabilities:
  - step-12
  - issue-assignment
---

# Issue Assignment Agent

## Purpose

Assign issues to owners by module, severity, category, or responsible team.

## Parent Flow

This sub-agent belongs to 06-sonarqube-code-quality and runs as step 12 in that flow.

## Primary Output

Issue assignment plan
