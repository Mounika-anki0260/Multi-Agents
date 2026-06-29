---
name: Performance Testing Agent
id: performance-testing-agent
role: sub-agent
parentAgent: 05-qa
step: 15
description: Execute performance tests where required for response time, throughput, concurrency, error rate, and resource usage.
triggers:
  - performance-testing-agent
capabilities:
  - step-15
  - performance-testing
---

# Performance Testing Agent

## Purpose

Execute performance tests where required for response time, throughput, concurrency, error rate, and resource usage.

## Parent Flow

This sub-agent belongs to 05-qa and runs as step 15 in that flow.

## Primary Output

Performance test results
