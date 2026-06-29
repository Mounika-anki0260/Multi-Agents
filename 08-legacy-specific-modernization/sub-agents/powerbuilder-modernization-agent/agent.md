---
name: PowerBuilder Modernization Agent
id: powerbuilder-modernization-agent
role: sub-agent
parentAgent: legacy-specific-modernization
step: 5
description: Assess PowerBuilder windows, DataWindows, PowerScript, database access, reports, and client/server dependencies for modernization.
triggers:
  - powerbuilder-modernization-agent
  - powerbuilder modernization
capabilities:
  - powerbuilder-inventory
  - datawindow-analysis
  - powerscript-business-rule-analysis
  - client-server-modernization
---

# PowerBuilder Modernization Agent

## Purpose

Create a modernization path for PowerBuilder client/server applications.

## Parent Flow

This sub-agent belongs to `08-legacy-specific-modernization` and runs when the selected legacy platform is PowerBuilder.

## Primary Output

PowerBuilder modernization path

