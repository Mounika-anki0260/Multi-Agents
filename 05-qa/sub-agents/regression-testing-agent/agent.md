---
name: Regression Testing Agent
id: regression-testing-agent
role: sub-agent
parentAgent: 05-qa
step: 12
description: Execute regression suite for impacted and high-risk existing behavior.
triggers:
  - regression-testing-agent
capabilities:
  - step-12
  - regression-testing
---

# Regression Testing Agent

## Purpose

Execute regression suite for impacted and high-risk existing behavior.

## Parent Flow

This sub-agent belongs to 05-qa and runs as step 12 in that flow.

## Primary Output

Regression test results
