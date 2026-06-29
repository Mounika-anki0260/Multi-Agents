---
name: Environment Profile Agent
id: environment-profile-agent
role: sub-agent
parentAgent: 03-backend
step: 4
description: Configure local, dev, QA/UAT, staging, and production profiles using environment-safe configuration.
triggers:
  - environment-profile-agent
capabilities:
  - step-4
  - environment-profile
---

# Environment Profile Agent

## Purpose

Configure local, dev, QA/UAT, staging, and production profiles using environment-safe configuration.

## Parent Flow

This sub-agent belongs to 03-backend and runs as step 4 in that flow.

## Primary Output

Environment profile setup
