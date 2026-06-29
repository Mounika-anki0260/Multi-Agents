---
name: Integration Testing Agent
id: integration-testing-agent
role: sub-agent
parentAgent: 05-qa
step: 11
description: Execute integration tests across frontend, backend, database, external systems, queues, files, and batch jobs.
triggers:
  - integration-testing-agent
capabilities:
  - step-11
  - integration-testing
---

# Integration Testing Agent

## Purpose

Execute integration tests across frontend, backend, database, external systems, queues, files, and batch jobs.

## Parent Flow

This sub-agent belongs to 05-qa and runs as step 11 in that flow.

## Primary Output

Integration test results
