---
name: Deployment Process Agent
id: deployment-process-agent
role: sub-agent
parentAgent: 01-reverse-engineering-documents
step: 11
description: Capture build, packaging, environment configuration, infrastructure, deployment scripts, release process, and rollback evidence.
triggers:
  - deployment-process-agent
capabilities:
  - step-11
  - deployment-process
---

# Deployment Process Agent

## Purpose

Capture build, packaging, environment configuration, infrastructure, deployment scripts, release process, and rollback evidence.

## Parent Flow

This sub-agent belongs to 01-reverse-engineering-documents and runs as step 11 in that flow.

## Primary Output

Deployment process summary
