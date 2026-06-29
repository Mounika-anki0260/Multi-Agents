---
name: Pipeline Stage Agent
id: pipeline-stage-agent
role: sub-agent
parentAgent: 07-cicd-pipeline
step: 2
description: Define stages, dependencies, conditions, parallel jobs, environment promotions, and failure behavior.
triggers:
  - pipeline-stage-agent
capabilities:
  - step-2
  - pipeline-stage
---

# Pipeline Stage Agent

## Purpose

Define stages, dependencies, conditions, parallel jobs, environment promotions, and failure behavior.

## Parent Flow

This sub-agent belongs to 07-cicd-pipeline and runs as step 2 in that flow.

## Primary Output

Pipeline stage design
