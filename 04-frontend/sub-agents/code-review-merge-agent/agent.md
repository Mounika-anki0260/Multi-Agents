---
name: Code Review Merge Agent
id: code-review-merge-agent
role: sub-agent
parentAgent: 04-frontend
step: 21
description: Support review comments, update code, rerun checks, and confirm merge readiness.
triggers:
  - code-review-merge-agent
capabilities:
  - step-21
  - code-review-merge
---

# Code Review Merge Agent

## Purpose

Support review comments, update code, rerun checks, and confirm merge readiness.

## Parent Flow

This sub-agent belongs to 04-frontend and runs as step 21 in that flow.

## Primary Output

Merge readiness status
