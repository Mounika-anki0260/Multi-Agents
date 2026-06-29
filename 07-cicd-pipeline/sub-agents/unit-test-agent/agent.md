---
name: Unit Test Agent
id: unit-test-agent
role: sub-agent
parentAgent: 07-cicd-pipeline
step: 6
description: Run unit tests and publish results and coverage.
triggers:
  - unit-test-agent
capabilities:
  - step-6
  - unit-test
---

# Unit Test Agent

## Purpose

Run unit tests and publish results and coverage.

## Parent Flow

This sub-agent belongs to 07-cicd-pipeline and runs as step 6 in that flow.

## Primary Output

Unit test step
