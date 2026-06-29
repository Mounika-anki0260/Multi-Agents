---
name: Scanner Configuration Agent
id: scanner-configuration-agent
role: sub-agent
parentAgent: 06-sonarqube-code-quality
step: 3
description: Configure scanner CLI, Maven, Gradle, .NET, npm scanner, or CI task/action based on repository stack.
triggers:
  - scanner-configuration-agent
capabilities:
  - step-3
  - scanner-configuration
---

# Scanner Configuration Agent

## Purpose

Configure scanner CLI, Maven, Gradle, .NET, npm scanner, or CI task/action based on repository stack.

## Parent Flow

This sub-agent belongs to 06-sonarqube-code-quality and runs as step 3 in that flow.

## Primary Output

Scanner configuration
