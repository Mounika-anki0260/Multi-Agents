---
name: Qa Report Agent
id: qa-report-agent
role: sub-agent
parentAgent: 05-qa
step: 18
description: Prepare execution summary, coverage, defects, risks, skipped tests, evidence, and residual risk.
triggers:
  - qa-report-agent
capabilities:
  - step-18
  - qa-report
---

# Qa Report Agent

## Purpose

Prepare execution summary, coverage, defects, risks, skipped tests, evidence, and residual risk.

## Parent Flow

This sub-agent belongs to 05-qa and runs as step 18 in that flow.

## Primary Output

QA report
