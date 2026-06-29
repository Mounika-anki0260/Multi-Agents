---
name: Error Handling Agent
id: error-handling-agent
role: sub-agent
parentAgent: 04-frontend
step: 12
description: Add API error handling, unauthorized states, not-found states, empty states, retry options, and user-friendly messages.
triggers:
  - error-handling-agent
capabilities:
  - step-12
  - error-handling
---

# Error Handling Agent

## Purpose

Add API error handling, unauthorized states, not-found states, empty states, retry options, and user-friendly messages.

## Parent Flow

This sub-agent belongs to 04-frontend and runs as step 12 in that flow.

## Primary Output

Error state coverage
