---
name: Batch Scheduled Task Agent
id: batch-scheduled-task-agent
role: sub-agent
parentAgent: 01-reverse-engineering-documents
step: 9
description: Identify cron jobs, schedulers, background workers, ETL jobs, reports, and operational scripts.
triggers:
  - batch-scheduled-task-agent
capabilities:
  - step-9
  - batch-scheduled-task
---

# Batch Scheduled Task Agent

## Purpose

Identify cron jobs, schedulers, background workers, ETL jobs, reports, and operational scripts.

## Parent Flow

This sub-agent belongs to 01-reverse-engineering-documents and runs as step 9 in that flow.

## Primary Output

Batch and scheduled task catalog
