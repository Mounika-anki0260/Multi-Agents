---
name: Legacy Batch Reporting Modernization Agent
id: legacy-batch-reporting-modernization-agent
role: sub-agent
parentAgent: legacy-specific-modernization
step: 9
description: Assess legacy batch, scheduler, ETL, file exchange, report generation, and operational processing workloads.
triggers:
  - legacy-batch-reporting-modernization-agent
  - batch modernization
  - reporting modernization
capabilities:
  - batch-job-inventory
  - scheduler-analysis
  - file-exchange-analysis
  - reporting-modernization
---

# Legacy Batch Reporting Modernization Agent

## Purpose

Create a modernization path for legacy batch jobs, schedulers, file exchanges, ETL, and reporting workloads.

## Parent Flow

This sub-agent belongs to `08-legacy-specific-modernization` and runs when the selected workload is batch, reporting, ETL, or scheduler-driven processing.

## Primary Output

Batch and reporting modernization path

