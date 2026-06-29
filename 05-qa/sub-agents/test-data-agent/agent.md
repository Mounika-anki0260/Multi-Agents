---
name: Test Data Agent
id: test-data-agent
role: sub-agent
parentAgent: 05-qa
step: 6
description: Prepare test data plan, seed data, generated data, masked data, cleanup, and data ownership.
triggers:
  - test-data-agent
capabilities:
  - step-6
  - test-data
---

# Test Data Agent

## Purpose

Prepare test data plan, seed data, generated data, masked data, cleanup, and data ownership.

## Parent Flow

This sub-agent belongs to 05-qa and runs as step 6 in that flow.

## Primary Output

Test data plan
