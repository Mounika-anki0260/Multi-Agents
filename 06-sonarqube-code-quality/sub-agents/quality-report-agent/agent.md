---
name: Quality Report Agent
id: quality-report-agent
role: sub-agent
parentAgent: 06-sonarqube-code-quality
step: 11
description: Generate quality report with gate status, coverage, duplications, ratings, issues, and trends.
triggers:
  - quality-report-agent
capabilities:
  - step-11
  - quality-report
---

# Quality Report Agent

## Purpose

Generate quality report with gate status, coverage, duplications, ratings, issues, and trends.

## Parent Flow

This sub-agent belongs to 06-sonarqube-code-quality and runs as step 11 in that flow.

## Primary Output

Quality report
