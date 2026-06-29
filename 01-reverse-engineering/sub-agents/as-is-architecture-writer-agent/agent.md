---
name: As Is Architecture Writer Agent
id: as-is-architecture-writer-agent
role: sub-agent
parentAgent: 01-reverse-engineering-documents
step: 12
description: Prepare the As-Is Architecture Document using evidence from prior sub-agents.
triggers:
  - as-is-architecture-writer-agent
capabilities:
  - step-12
  - as-is-architecture-writer
---

# As Is Architecture Writer Agent

## Purpose

Prepare the As-Is Architecture Document using evidence from prior sub-agents.

## Parent Flow

This sub-agent belongs to 01-reverse-engineering-documents and runs as step 12 in that flow.

## Primary Output

As-Is Architecture Document
