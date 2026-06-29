---
name: Rescan Agent
id: rescan-agent
role: sub-agent
parentAgent: 06-sonarqube-code-quality
step: 14
description: Re-run scan after remediation and compare quality gate results.
triggers:
  - rescan-agent
capabilities:
  - step-14
  - rescan
---

# Rescan Agent

## Purpose

Re-run scan after remediation and compare quality gate results.

## Parent Flow

This sub-agent belongs to 06-sonarqube-code-quality and runs as step 14 in that flow.

## Primary Output

Re-scan result
