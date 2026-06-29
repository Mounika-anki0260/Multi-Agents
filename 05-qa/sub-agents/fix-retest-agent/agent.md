---
name: Fix Retest Agent
id: fix-retest-agent
role: sub-agent
parentAgent: 05-qa
step: 17
description: Retest fixed defects, verify regression impact, and update defect status.
triggers:
  - fix-retest-agent
capabilities:
  - step-17
  - fix-retest
---

# Fix Retest Agent

## Purpose

Retest fixed defects, verify regression impact, and update defect status.

## Parent Flow

This sub-agent belongs to 05-qa and runs as step 17 in that flow.

## Primary Output

Retest report
