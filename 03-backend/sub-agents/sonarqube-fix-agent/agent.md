---
name: Sonarqube Fix Agent
id: sonarqube-fix-agent
role: sub-agent
parentAgent: 03-backend
step: 18
description: Fix SonarQube blocker, critical, vulnerability, duplication, and code smell issues.
triggers:
  - sonarqube-fix-agent
capabilities:
  - step-18
  - sonarqube-fix
---

# Sonarqube Fix Agent

## Purpose

Fix SonarQube blocker, critical, vulnerability, duplication, and code smell issues.

## Parent Flow

This sub-agent belongs to 03-backend and runs as step 18 in that flow.

## Primary Output

SonarQube remediation
