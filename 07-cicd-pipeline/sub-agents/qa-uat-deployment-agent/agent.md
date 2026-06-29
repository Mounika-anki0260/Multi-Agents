---
name: Qa Uat Deployment Agent
id: qa-uat-deployment-agent
role: sub-agent
parentAgent: 07-cicd-pipeline
step: 14
description: Deploy to QA/UAT/staging environments and coordinate test readiness.
triggers:
  - qa-uat-deployment-agent
capabilities:
  - step-14
  - qa-uat-deployment
---

# Qa Uat Deployment Agent

## Purpose

Deploy to QA/UAT/staging environments and coordinate test readiness.

## Parent Flow

This sub-agent belongs to 07-cicd-pipeline and runs as step 14 in that flow.

## Primary Output

QA/UAT deployment
