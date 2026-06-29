---
name: Eslint Prettier Agent
id: eslint-prettier-agent
role: sub-agent
parentAgent: 04-frontend
step: 17
description: Configure ESLint, Prettier, formatting scripts, lint rules, import rules, and repo-specific style standards.
triggers:
  - eslint-prettier-agent
capabilities:
  - step-17
  - eslint-prettier
---

# Eslint Prettier Agent

## Purpose

Configure ESLint, Prettier, formatting scripts, lint rules, import rules, and repo-specific style standards.

## Parent Flow

This sub-agent belongs to 04-frontend and runs as step 17 in that flow.

## Primary Output

Lint and format setup
