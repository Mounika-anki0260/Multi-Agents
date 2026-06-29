---
name: Quality Setup Questionnaire Agent
id: quality-setup-questionnaire-agent
role: sub-agent
parentAgent: 06-sonarqube-code-quality
step: 1
description: Ask SonarQube/SonarCloud choice, project key, organization, languages, scanner, thresholds, coverage reports, branches, ownership, and exclusions.
triggers:
  - quality-setup-questionnaire-agent
capabilities:
  - step-1
  - quality-setup-questionnaire
---

# Quality Setup Questionnaire Agent

## Purpose

Ask SonarQube/SonarCloud choice, project key, organization, languages, scanner, thresholds, coverage reports, branches, ownership, and exclusions.

## Parent Flow

This sub-agent belongs to 06-sonarqube-code-quality and runs as step 1 in that flow.

## Primary Output

Quality setup decisions
