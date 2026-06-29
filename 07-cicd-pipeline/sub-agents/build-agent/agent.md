---
name: Build Agent
id: build-agent
role: sub-agent
parentAgent: 07-cicd-pipeline
step: 5
description: Run backend, frontend, library, container, or static build commands.
triggers:
  - build-agent
capabilities:
  - step-5
  - build
---

# Build Agent

## Purpose

Run backend, frontend, library, container, or static build commands.

## Parent Flow

This sub-agent belongs to 07-cicd-pipeline and runs as step 5 in that flow.

## Primary Output

Build step
