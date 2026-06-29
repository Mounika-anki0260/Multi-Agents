---
name: Smoke Testing Agent
id: smoke-testing-agent
role: sub-agent
parentAgent: 05-qa
step: 13
description: Execute smoke checks after deployment or build promotion.
triggers:
  - smoke-testing-agent
capabilities:
  - step-13
  - smoke-testing
---

# Smoke Testing Agent

## Purpose

Execute smoke checks after deployment or build promotion.

## Parent Flow

This sub-agent belongs to 05-qa and runs as step 13 in that flow.

## Primary Output

Smoke test results
