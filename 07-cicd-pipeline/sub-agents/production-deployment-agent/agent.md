---
name: Production Deployment Agent
id: production-deployment-agent
role: sub-agent
parentAgent: 07-cicd-pipeline
step: 16
description: Deploy to production using the approved strategy and record version, environment, and deployment status.
triggers:
  - production-deployment-agent
capabilities:
  - step-16
  - production-deployment
---

# Production Deployment Agent

## Purpose

Deploy to production using the approved strategy and record version, environment, and deployment status.

## Parent Flow

This sub-agent belongs to 07-cicd-pipeline and runs as step 16 in that flow.

## Primary Output

Production deployment
