---
name: Docker Image Agent
id: docker-image-agent
role: sub-agent
parentAgent: 07-cicd-pipeline
step: 11
description: Build Docker images, tag with version/commit, scan image, and prepare for registry push when required.
triggers:
  - docker-image-agent
capabilities:
  - step-11
  - docker-image
---

# Docker Image Agent

## Purpose

Build Docker images, tag with version/commit, scan image, and prepare for registry push when required.

## Parent Flow

This sub-agent belongs to 07-cicd-pipeline and runs as step 11 in that flow.

## Primary Output

Docker image
