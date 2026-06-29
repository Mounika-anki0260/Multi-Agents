---
name: Registry Push Agent
id: registry-push-agent
role: sub-agent
parentAgent: 07-cicd-pipeline
step: 12
description: Push packages, artifacts, Docker images, or Helm charts to the configured registry.
triggers:
  - registry-push-agent
capabilities:
  - step-12
  - registry-push
---

# Registry Push Agent

## Purpose

Push packages, artifacts, Docker images, or Helm charts to the configured registry.

## Parent Flow

This sub-agent belongs to 07-cicd-pipeline and runs as step 12 in that flow.

## Primary Output

Published artifact/image
