---
name: Defect Logging Agent
id: defect-logging-agent
role: sub-agent
parentAgent: 05-qa
step: 16
description: Log defects with reproduction steps, expected result, actual result, evidence, severity, priority, environment, and owner.
triggers:
  - defect-logging-agent
capabilities:
  - step-16
  - defect-logging
---

# Defect Logging Agent

## Purpose

Log defects with reproduction steps, expected result, actual result, evidence, severity, priority, environment, and owner.

## Parent Flow

This sub-agent belongs to 05-qa and runs as step 16 in that flow.

## Primary Output

Defect report
