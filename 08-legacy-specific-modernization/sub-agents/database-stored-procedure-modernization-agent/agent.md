---
name: Database Stored Procedure Modernization Agent
id: database-stored-procedure-modernization-agent
role: sub-agent
parentAgent: legacy-specific-modernization
step: 8
description: Assess database-heavy applications where stored procedures, packages, triggers, jobs, and views contain major business logic.
triggers:
  - database-stored-procedure-modernization-agent
  - stored procedure modernization
  - database modernization
capabilities:
  - stored-procedure-inventory
  - trigger-business-rule-analysis
  - database-job-analysis
  - data-logic-modernization
---

# Database Stored Procedure Modernization Agent

## Purpose

Create a modernization path for database-heavy applications with business logic in stored procedures, packages, triggers, jobs, views, or reports.

## Parent Flow

This sub-agent belongs to `08-legacy-specific-modernization` and runs when the selected legacy platform is primarily database logic.

## Primary Output

Database logic modernization path

