---
name: Integration Analysis Agent
id: integration-analysis-agent
role: sub-agent
parentAgent: 01-reverse-engineering-documents
step: 8
description: Identify third-party systems, API calls, queues, files, events, protocols, retries, and failure handling.
triggers:
  - integration-analysis-agent
capabilities:
  - step-8
  - integration-analysis
---

# Integration Analysis Agent

## Purpose

Identify third-party systems, API calls, queues, files, events, protocols, retries, and failure handling.

## Parent Flow

This sub-agent belongs to 01-reverse-engineering-documents and runs as step 8 in that flow.

## Primary Output

Integration inventory
