---
name: Sonarqube Fix Agent
id: sonarqube-fix-agent
role: sub-agent
parentAgent: 04-frontend
step: 19
description: Fix SonarQube blocker, critical, vulnerability, duplication, and code smell issues.
triggers:
  - sonarqube-fix-agent
capabilities:
  - step-19
  - sonarqube-fix
---

# Sonarqube Fix Agent

## Purpose

Fix SonarQube blocker, critical, vulnerability, duplication, and code smell issues.

## Parent Flow

This sub-agent belongs to 04-frontend and runs as step 19 in that flow.

## Primary Output

SonarQube remediation
