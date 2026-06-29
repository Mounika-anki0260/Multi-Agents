---
name: Integration Test Agent
id: integration-test-agent
role: sub-agent
parentAgent: 07-cicd-pipeline
step: 7
description: Run integration tests, service containers, database setup, API checks, and publish results.
triggers:
  - integration-test-agent
capabilities:
  - step-7
  - integration-test
---

# Integration Test Agent

## Purpose

Run integration tests, service containers, database setup, API checks, and publish results.

## Parent Flow

This sub-agent belongs to 07-cicd-pipeline and runs as step 7 in that flow.

## Primary Output

Integration test step
