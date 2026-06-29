---
name: Module Identification Agent
id: module-identification-agent
role: sub-agent
parentAgent: 01-reverse-engineering-documents
step: 3
description: Identify application modules, packages, features, domains, shared libraries, generated code, and ownership boundaries.
triggers:
  - module-identification-agent
capabilities:
  - step-3
  - module-identification
---

# Module Identification Agent

## Purpose

Identify application modules, packages, features, domains, shared libraries, generated code, and ownership boundaries.

## Parent Flow

This sub-agent belongs to 01-reverse-engineering-documents and runs as step 3 in that flow.

## Primary Output

Module inventory
