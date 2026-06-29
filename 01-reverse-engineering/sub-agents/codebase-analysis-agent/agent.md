---
name: Codebase Analysis Agent
id: codebase-analysis-agent
role: sub-agent
parentAgent: 01-reverse-engineering-documents
step: 2
description: Analyze current source structure, languages, frameworks, build tools, dependencies, configuration, and entry points.
triggers:
  - codebase-analysis-agent
capabilities:
  - step-2
  - codebase-analysis
---

# Codebase Analysis Agent

## Purpose

Analyze current source structure, languages, frameworks, build tools, dependencies, configuration, and entry points.

## Parent Flow

This sub-agent belongs to 01-reverse-engineering-documents and runs as step 2 in that flow.

## Primary Output

Codebase analysis summary
