---
name: Ui Component Test Agent
id: ui-component-test-agent
role: sub-agent
parentAgent: 04-frontend
step: 16
description: Add component and UI tests for rendering, interaction, validation, loading, error, and permission states.
triggers:
  - ui-component-test-agent
capabilities:
  - step-16
  - ui-component-test
---

# Ui Component Test Agent

## Purpose

Add component and UI tests for rendering, interaction, validation, loading, error, and permission states.

## Parent Flow

This sub-agent belongs to 04-frontend and runs as step 16 in that flow.

## Primary Output

UI/component test coverage
