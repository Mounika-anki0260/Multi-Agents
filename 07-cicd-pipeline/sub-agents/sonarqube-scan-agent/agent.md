---
name: Sonarqube Scan Agent
id: sonarqube-scan-agent
role: sub-agent
parentAgent: 07-cicd-pipeline
step: 8
description: Run SonarQube scan, publish quality gate status, and fail pipeline when required.
triggers:
  - sonarqube-scan-agent
capabilities:
  - step-8
  - sonarqube-scan
---

# Sonarqube Scan Agent

## Purpose

Run SonarQube scan, publish quality gate status, and fail pipeline when required.

## Parent Flow

This sub-agent belongs to 07-cicd-pipeline and runs as step 8 in that flow.

## Primary Output

SonarQube scan step
