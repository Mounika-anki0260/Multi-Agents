---
name: Pull Request Agent
id: pull-request-agent
role: sub-agent
parentAgent: 03-backend
step: 19
description: Prepare PR summary, changed files, tests run, risk notes, screenshots/logs where useful, and review checklist.
triggers:
  - pull-request-agent
capabilities:
  - step-19
  - pull-request
---

# Pull Request Agent

## Purpose

Prepare PR summary, changed files, tests run, risk notes, screenshots/logs where useful, and review checklist.

## Parent Flow

This sub-agent belongs to 03-backend and runs as step 19 in that flow.

## Primary Output

Pull request readiness
