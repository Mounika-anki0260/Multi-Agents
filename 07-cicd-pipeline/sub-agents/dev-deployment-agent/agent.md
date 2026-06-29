---
name: Dev Deployment Agent
id: dev-deployment-agent
role: sub-agent
parentAgent: 07-cicd-pipeline
step: 13
description: Deploy to development environment and capture deployment status.
triggers:
  - dev-deployment-agent
capabilities:
  - step-13
  - dev-deployment
---

# Dev Deployment Agent

## Purpose

Deploy to development environment and capture deployment status.

## Parent Flow

This sub-agent belongs to 07-cicd-pipeline and runs as step 13 in that flow.

## Primary Output

Development deployment
