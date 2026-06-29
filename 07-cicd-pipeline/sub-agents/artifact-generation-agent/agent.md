---
name: Artifact Generation Agent
id: artifact-generation-agent
role: sub-agent
parentAgent: 07-cicd-pipeline
step: 10
description: Package build outputs, version artifacts, attach metadata, and publish artifacts.
triggers:
  - artifact-generation-agent
capabilities:
  - step-10
  - artifact-generation
---

# Artifact Generation Agent

## Purpose

Package build outputs, version artifacts, attach metadata, and publish artifacts.

## Parent Flow

This sub-agent belongs to 07-cicd-pipeline and runs as step 10 in that flow.

## Primary Output

Build artifact
