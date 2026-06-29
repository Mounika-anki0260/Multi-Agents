---
name: Code Quality Agent
id: code-quality-agent
role: sub-agent
parentAgent: 04-frontend
step: 18
description: Run build, tests, linting, formatting, static analysis, and coverage checks.
triggers:
  - code-quality-agent
capabilities:
  - step-18
  - code-quality
---

# Code Quality Agent

## Purpose

Run build, tests, linting, formatting, static analysis, and coverage checks.

## Parent Flow

This sub-agent belongs to 04-frontend and runs as step 18 in that flow.

## Primary Output

Code quality result
