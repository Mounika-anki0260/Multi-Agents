---
name: Coverage Threshold Agent
id: coverage-threshold-agent
role: sub-agent
parentAgent: 06-sonarqube-code-quality
step: 5
description: Define coverage thresholds and connect unit, integration, frontend, and backend coverage report paths.
triggers:
  - coverage-threshold-agent
capabilities:
  - step-5
  - coverage-threshold
---

# Coverage Threshold Agent

## Purpose

Define coverage thresholds and connect unit, integration, frontend, and backend coverage report paths.

## Parent Flow

This sub-agent belongs to 06-sonarqube-code-quality and runs as step 5 in that flow.

## Primary Output

Coverage configuration
