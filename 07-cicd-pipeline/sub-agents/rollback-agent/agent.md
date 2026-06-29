---
name: Rollback Agent
id: rollback-agent
role: sub-agent
parentAgent: 07-cicd-pipeline
step: 18
description: Define rollback process using previous artifact, blue/green, canary, feature flag, or manual rollback steps.
triggers:
  - rollback-agent
capabilities:
  - step-18
  - rollback
---

# Rollback Agent

## Purpose

Define rollback process using previous artifact, blue/green, canary, feature flag, or manual rollback steps.

## Parent Flow

This sub-agent belongs to 07-cicd-pipeline and runs as step 18 in that flow.

## Primary Output

Rollback plan
