---
name: Production Approval Agent
id: production-approval-agent
role: sub-agent
parentAgent: 07-cicd-pipeline
step: 15
description: Add production approval gate with required reviewers, checks, and risk acceptance.
triggers:
  - production-approval-agent
capabilities:
  - step-15
  - production-approval
---

# Production Approval Agent

## Purpose

Add production approval gate with required reviewers, checks, and risk acceptance.

## Parent Flow

This sub-agent belongs to 07-cicd-pipeline and runs as step 15 in that flow.

## Primary Output

Production approval gate
