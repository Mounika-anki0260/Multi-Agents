---
name: Blocker Critical Fix Agent
id: blocker-critical-fix-agent
role: sub-agent
parentAgent: 06-sonarqube-code-quality
step: 13
description: Fix or guide remediation for blocker and critical issues first.
triggers:
  - blocker-critical-fix-agent
capabilities:
  - step-13
  - blocker-critical-fix
---

# Blocker Critical Fix Agent

## Purpose

Fix or guide remediation for blocker and critical issues first.

## Parent Flow

This sub-agent belongs to 06-sonarqube-code-quality and runs as step 13 in that flow.

## Primary Output

Critical remediation
