---
name: Security Dependency Scan Agent
id: security-dependency-scan-agent
role: sub-agent
parentAgent: 07-cicd-pipeline
step: 9
description: Run dependency, secret, SAST, container, and IaC scans as required.
triggers:
  - security-dependency-scan-agent
capabilities:
  - step-9
  - security-dependency-scan
---

# Security Dependency Scan Agent

## Purpose

Run dependency, secret, SAST, container, and IaC scans as required.

## Parent Flow

This sub-agent belongs to 07-cicd-pipeline and runs as step 9 in that flow.

## Primary Output

Security scan step
