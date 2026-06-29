---
name: Test Scenario Agent
id: test-scenario-agent
role: sub-agent
parentAgent: 05-qa
step: 4
description: Prepare end-to-end scenarios by feature, role, API, workflow, integration, and risk area.
triggers:
  - test-scenario-agent
capabilities:
  - step-4
  - test-scenario
---

# Test Scenario Agent

## Purpose

Prepare end-to-end scenarios by feature, role, API, workflow, integration, and risk area.

## Parent Flow

This sub-agent belongs to 05-qa and runs as step 4 in that flow.

## Primary Output

Test scenarios
