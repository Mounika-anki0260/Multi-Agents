---
name: Api Testing Agent
id: api-testing-agent
role: sub-agent
parentAgent: 05-qa
step: 9
description: Execute API tests for contracts, status codes, payloads, errors, auth, pagination, filtering, and integration behavior.
triggers:
  - api-testing-agent
capabilities:
  - step-9
  - api-testing
---

# Api Testing Agent

## Purpose

Execute API tests for contracts, status codes, payloads, errors, auth, pagination, filtering, and integration behavior.

## Parent Flow

This sub-agent belongs to 05-qa and runs as step 9 in that flow.

## Primary Output

API test results
