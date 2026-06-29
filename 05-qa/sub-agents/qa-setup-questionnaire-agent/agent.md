---
name: Qa Setup Questionnaire Agent
id: qa-setup-questionnaire-agent
role: sub-agent
parentAgent: 05-qa
step: 1
description: Ask testing scope, tools, script structure, environments, test data, entry/exit criteria, devices, defect process, performance targets, and sign-off evidence.
triggers:
  - qa-setup-questionnaire-agent
capabilities:
  - step-1
  - qa-setup-questionnaire
---

# Qa Setup Questionnaire Agent

## Purpose

Ask testing scope, tools, script structure, environments, test data, entry/exit criteria, devices, defect process, performance targets, and sign-off evidence.

## Parent Flow

This sub-agent belongs to 05-qa and runs as step 1 in that flow.

## Primary Output

QA setup decisions
