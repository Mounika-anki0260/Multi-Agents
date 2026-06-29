---
name: Backend Project Setup Agent
id: backend-project-setup-agent
role: sub-agent
parentAgent: 03-backend
step: 2
description: Create or validate backend project setup, dependencies, build tool, runtime configuration, and developer commands.
triggers:
  - backend-project-setup-agent
capabilities:
  - step-2
  - backend-project-setup
---

# Backend Project Setup Agent

## Purpose

Create or validate backend project setup, dependencies, build tool, runtime configuration, and developer commands.

## Parent Flow

This sub-agent belongs to 03-backend and runs as step 2 in that flow.

## Primary Output

Backend project baseline
