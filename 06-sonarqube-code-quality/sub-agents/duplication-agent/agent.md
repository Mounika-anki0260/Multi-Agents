---
name: Duplication Agent
id: duplication-agent
role: sub-agent
parentAgent: 06-sonarqube-code-quality
step: 8
description: Enable duplicate code checks and define exclusions for generated code where justified.
triggers:
  - duplication-agent
capabilities:
  - step-8
  - duplication
---

# Duplication Agent

## Purpose

Enable duplicate code checks and define exclusions for generated code where justified.

## Parent Flow

This sub-agent belongs to 06-sonarqube-code-quality and runs as step 8 in that flow.

## Primary Output

Duplication policy
