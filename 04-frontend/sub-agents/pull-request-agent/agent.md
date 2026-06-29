---
name: Pull Request Agent
id: pull-request-agent
role: sub-agent
parentAgent: 04-frontend
step: 20
description: Prepare PR summary, test evidence, accessibility notes, screenshots where useful, and review checklist.
triggers:
  - pull-request-agent
capabilities:
  - step-20
  - pull-request
---

# Pull Request Agent

## Purpose

Prepare PR summary, test evidence, accessibility notes, screenshots where useful, and review checklist.

## Parent Flow

This sub-agent belongs to 04-frontend and runs as step 20 in that flow.

## Primary Output

Pull request readiness
