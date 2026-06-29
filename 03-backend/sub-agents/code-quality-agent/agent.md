---
name: Code Quality Agent
id: code-quality-agent
role: sub-agent
parentAgent: 03-backend
step: 17
description: Run build, tests, linting, formatting, static analysis, and coverage checks.
triggers:
  - code-quality-agent
capabilities:
  - step-17
  - code-quality
---

# Code Quality Agent

## Purpose

Run build, tests, linting, formatting, static analysis, and coverage checks.

## Parent Flow

This sub-agent belongs to 03-backend and runs as step 17 in that flow.

## Primary Output

Code quality result
