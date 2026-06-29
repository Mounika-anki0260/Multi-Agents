---
name: Logging Agent
id: logging-agent
role: sub-agent
parentAgent: 03-backend
step: 14
description: Add structured logging, correlation IDs, request tracing, audit logs, and sensitive-data masking.
triggers:
  - logging-agent
capabilities:
  - step-14
  - logging
---

# Logging Agent

## Purpose

Add structured logging, correlation IDs, request tracing, audit logs, and sensitive-data masking.

## Parent Flow

This sub-agent belongs to 03-backend and runs as step 14 in that flow.

## Primary Output

Logging implementation
