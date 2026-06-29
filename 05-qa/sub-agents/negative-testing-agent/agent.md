---
name: Negative Testing Agent
id: negative-testing-agent
role: sub-agent
parentAgent: 05-qa
step: 14
description: Execute invalid input, unauthorized access, boundary, failure, timeout, and error-path tests.
triggers:
  - negative-testing-agent
capabilities:
  - step-14
  - negative-testing
---

# Negative Testing Agent

## Purpose

Execute invalid input, unauthorized access, boundary, failure, timeout, and error-path tests.

## Parent Flow

This sub-agent belongs to 05-qa and runs as step 14 in that flow.

## Primary Output

Negative test results
