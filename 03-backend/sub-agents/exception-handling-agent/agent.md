---
name: Exception Handling Agent
id: exception-handling-agent
role: sub-agent
parentAgent: 03-backend
step: 13
description: Add global exception handling, error contracts, domain exceptions, validation errors, and audit-safe error messages.
triggers:
  - exception-handling-agent
capabilities:
  - step-13
  - exception-handling
---

# Exception Handling Agent

## Purpose

Add global exception handling, error contracts, domain exceptions, validation errors, and audit-safe error messages.

## Parent Flow

This sub-agent belongs to 03-backend and runs as step 13 in that flow.

## Primary Output

Error handling layer
