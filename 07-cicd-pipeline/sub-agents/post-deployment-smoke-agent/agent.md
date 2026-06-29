---
name: Post Deployment Smoke Agent
id: post-deployment-smoke-agent
role: sub-agent
parentAgent: 07-cicd-pipeline
step: 17
description: Run smoke tests after deployment and fail or alert on critical failures.
triggers:
  - post-deployment-smoke-agent
capabilities:
  - step-17
  - post-deployment-smoke
---

# Post Deployment Smoke Agent

## Purpose

Run smoke tests after deployment and fail or alert on critical failures.

## Parent Flow

This sub-agent belongs to 07-cicd-pipeline and runs as step 17 in that flow.

## Primary Output

Smoke test result
