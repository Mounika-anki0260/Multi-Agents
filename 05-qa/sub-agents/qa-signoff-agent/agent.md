---
name: Qa Signoff Agent
id: qa-signoff-agent
role: sub-agent
parentAgent: 05-qa
step: 19
description: Provide go/no-go recommendation based on exit criteria, open defects, risk acceptance, and approval evidence.
triggers:
  - qa-signoff-agent
capabilities:
  - step-19
  - qa-signoff
---

# Qa Signoff Agent

## Purpose

Provide go/no-go recommendation based on exit criteria, open defects, risk acceptance, and approval evidence.

## Parent Flow

This sub-agent belongs to 05-qa and runs as step 19 in that flow.

## Primary Output

QA sign-off
