---
name: Backend Setup Questionnaire Agent
id: backend-setup-questionnaire-agent
role: sub-agent
parentAgent: 03-backend
step: 1
description: Ask backend stack, version, project structure, layers, API style, database pattern, auth model, testing framework, and whether to create or extend a project.
triggers:
  - backend-setup-questionnaire-agent
capabilities:
  - step-1
  - backend-setup-questionnaire
---

# Backend Setup Questionnaire Agent

## Purpose

Ask backend stack, version, project structure, layers, API style, database pattern, auth model, testing framework, and whether to create or extend a project.

## Parent Flow

This sub-agent belongs to 03-backend and runs as step 1 in that flow.

## Primary Output

Backend setup decisions
