---
name: Database Schema Agent
id: database-schema-agent
role: sub-agent
parentAgent: 01-reverse-engineering-documents
step: 7
description: Analyze tables, views, collections, relationships, constraints, indexes, migrations, stored logic, and data ownership.
triggers:
  - database-schema-agent
capabilities:
  - step-7
  - database-schema
---

# Database Schema Agent

## Purpose

Analyze tables, views, collections, relationships, constraints, indexes, migrations, stored logic, and data ownership.

## Parent Flow

This sub-agent belongs to 01-reverse-engineering-documents and runs as step 7 in that flow.

## Primary Output

Database schema documentation
