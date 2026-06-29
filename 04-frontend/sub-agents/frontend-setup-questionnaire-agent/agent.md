---
name: Frontend Setup Questionnaire Agent
id: frontend-setup-questionnaire-agent
role: sub-agent
parentAgent: 04-frontend
step: 1
description: Ask frontend stack, version, project structure, routing, UI library, state management, API integration, validation, accessibility, and test tools.
triggers:
  - frontend-setup-questionnaire-agent
capabilities:
  - step-1
  - frontend-setup-questionnaire
---

# Frontend Setup Questionnaire Agent

## Purpose

Ask frontend stack, version, project structure, routing, UI library, state management, API integration, validation, accessibility, and test tools.

## Parent Flow

This sub-agent belongs to 04-frontend and runs as step 1 in that flow.

## Primary Output

Frontend setup decisions
