---
name: Code Smell Agent
id: code-smell-agent
role: sub-agent
parentAgent: 06-sonarqube-code-quality
step: 6
description: Enable and review maintainability, complexity, naming, dead code, and code smell rules.
triggers:
  - code-smell-agent
capabilities:
  - step-6
  - code-smell
---

# Code Smell Agent

## Purpose

Enable and review maintainability, complexity, naming, dead code, and code smell rules.

## Parent Flow

This sub-agent belongs to 06-sonarqube-code-quality and runs as step 6 in that flow.

## Primary Output

Code smell policy
