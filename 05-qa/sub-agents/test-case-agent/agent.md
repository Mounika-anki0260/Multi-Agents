---
name: Test Case Agent
id: test-case-agent
role: sub-agent
parentAgent: 05-qa
step: 5
description: Prepare positive, negative, boundary, role-based, validation, integration, and regression test cases.
triggers:
  - test-case-agent
capabilities:
  - step-5
  - test-case
---

# Test Case Agent

## Purpose

Prepare positive, negative, boundary, role-based, validation, integration, and regression test cases.

## Parent Flow

This sub-agent belongs to 05-qa and runs as step 5 in that flow.

## Primary Output

Test case catalog
