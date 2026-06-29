---
name: Legacy Modernization Questionnaire Agent
id: legacy-modernization-questionnaire-agent
role: sub-agent
parentAgent: legacy-specific-modernization
step: 1
description: Ask the legacy platform, modernization goal, artifact availability, compatibility constraints, target constraints, and delivery expectations.
triggers:
  - legacy-modernization-questionnaire-agent
capabilities:
  - legacy-modernization-intake
  - modernization-goal-capture
  - compatibility-constraint-capture
---

# Legacy Modernization Questionnaire Agent

## Purpose

Collect the minimum decisions required before selecting a technology-specific modernization path.

## Parent Flow

This sub-agent belongs to `08-legacy-specific-modernization` and runs as step 1 in that flow.

## Primary Output

Legacy modernization intake decisions

