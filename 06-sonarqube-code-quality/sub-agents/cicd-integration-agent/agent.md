---
name: Cicd Integration Agent
id: cicd-integration-agent
role: sub-agent
parentAgent: 06-sonarqube-code-quality
step: 9
description: Integrate scans into CI/CD build, pull request validation, branch analysis, and release gates.
triggers:
  - cicd-integration-agent
capabilities:
  - step-9
  - cicd-integration
---

# Cicd Integration Agent

## Purpose

Integrate scans into CI/CD build, pull request validation, branch analysis, and release gates.

## Parent Flow

This sub-agent belongs to 06-sonarqube-code-quality and runs as step 9 in that flow.

## Primary Output

CI/CD quality integration
