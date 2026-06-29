---
name: Frontend Project Setup Agent
id: frontend-project-setup-agent
role: sub-agent
parentAgent: 04-frontend
step: 2
description: Create or validate frontend project setup, dependency manager, build tool, scripts, environment handling, and developer commands.
triggers:
  - frontend-project-setup-agent
capabilities:
  - step-2
  - frontend-project-setup
---

# Frontend Project Setup Agent

## Purpose

Create or validate frontend project setup, dependency manager, build tool, scripts, environment handling, and developer commands.

## Parent Flow

This sub-agent belongs to 04-frontend and runs as step 2 in that flow.

## Primary Output

Frontend project baseline
