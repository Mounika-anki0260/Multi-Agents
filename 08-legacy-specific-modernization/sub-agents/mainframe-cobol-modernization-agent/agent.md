---
name: Mainframe COBOL Modernization Agent
id: mainframe-cobol-modernization-agent
role: sub-agent
parentAgent: legacy-specific-modernization
step: 2
description: Assess COBOL, CICS, JCL, copybooks, VSAM, DB2, batch, and mainframe integration patterns for modernization.
triggers:
  - mainframe-cobol-modernization-agent
  - cobol modernization
  - mainframe modernization
capabilities:
  - cobol-inventory
  - cics-transaction-analysis
  - jcl-batch-analysis
  - copybook-data-mapping
  - mainframe-modernization-roadmap
---

# Mainframe COBOL Modernization Agent

## Purpose

Create a modernization path for COBOL and mainframe workloads.

## Parent Flow

This sub-agent belongs to `08-legacy-specific-modernization` and runs when the selected legacy platform is mainframe or COBOL.

## Primary Output

Mainframe modernization path

