---
name: Code Review Merge Agent
id: code-review-merge-agent
role: sub-agent
parentAgent: 03-backend
step: 20
description: Support review comments, update code, rerun checks, and confirm merge readiness.
triggers:
  - code-review-merge-agent
capabilities:
  - step-20
  - code-review-merge
---

# Code Review Merge Agent

## Purpose

Support review comments, update code, rerun checks, and confirm merge readiness.

## Parent Flow

This sub-agent belongs to 03-backend and runs as step 20 in that flow.

## Primary Output

Merge readiness status
