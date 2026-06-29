---
name: Frontend Ui Testing Agent
id: frontend-ui-testing-agent
role: sub-agent
parentAgent: 05-qa
step: 10
description: Execute UI tests for screens, navigation, forms, errors, loading, accessibility basics, and browser behavior.
triggers:
  - frontend-ui-testing-agent
capabilities:
  - step-10
  - frontend-ui-testing
---

# Frontend Ui Testing Agent

## Purpose

Execute UI tests for screens, navigation, forms, errors, loading, accessibility basics, and browser behavior.

## Parent Flow

This sub-agent belongs to 05-qa and runs as step 10 in that flow.

## Primary Output

UI test results
