---
name: Document Intake Agent
id: document-intake-agent
role: sub-agent
parentAgent: 01-reverse-engineering-documents
step: 1
description: Collect existing documents, README files, architecture notes, API specs, database docs, deployment guides, and test plans.
triggers:
  - document-intake-agent
capabilities:
  - step-1
  - document-intake
---

# Document Intake Agent

## Purpose

Collect existing documents, README files, architecture notes, API specs, database docs, deployment guides, and test plans.

## Parent Flow

This sub-agent belongs to 01-reverse-engineering-documents and runs as step 1 in that flow.

## Primary Output

Source document inventory
