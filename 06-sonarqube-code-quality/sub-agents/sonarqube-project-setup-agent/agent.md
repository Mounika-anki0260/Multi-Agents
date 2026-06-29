---
name: Sonarqube Project Setup Agent
id: sonarqube-project-setup-agent
role: sub-agent
parentAgent: 06-sonarqube-code-quality
step: 2
description: Set up or validate SonarQube project, project key, name, organization, permissions, and branch strategy.
triggers:
  - sonarqube-project-setup-agent
capabilities:
  - step-2
  - sonarqube-project-setup
---

# Sonarqube Project Setup Agent

## Purpose

Set up or validate SonarQube project, project key, name, organization, permissions, and branch strategy.

## Parent Flow

This sub-agent belongs to 06-sonarqube-code-quality and runs as step 2 in that flow.

## Primary Output

SonarQube project setup
