---
name: Test Environment Agent
id: test-environment-agent
role: sub-agent
parentAgent: 05-qa
step: 7
description: Verify environment availability, URLs, credentials, configuration, services, data, monitoring, and deployment version.
triggers:
  - test-environment-agent
capabilities:
  - step-7
  - test-environment
---

# Test Environment Agent

## Purpose

Verify environment availability, URLs, credentials, configuration, services, data, monitoring, and deployment version.

## Parent Flow

This sub-agent belongs to 05-qa and runs as step 7 in that flow.

## Primary Output

Test environment readiness
