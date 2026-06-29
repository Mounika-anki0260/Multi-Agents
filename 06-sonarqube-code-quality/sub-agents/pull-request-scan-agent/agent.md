---
name: Pull Request Scan Agent
id: pull-request-scan-agent
role: sub-agent
parentAgent: 06-sonarqube-code-quality
step: 10
description: Run or define pull request scan behavior, decoration, branch comparison, and failure conditions.
triggers:
  - pull-request-scan-agent
capabilities:
  - step-10
  - pull-request-scan
---

# Pull Request Scan Agent

## Purpose

Run or define pull request scan behavior, decoration, branch comparison, and failure conditions.

## Parent Flow

This sub-agent belongs to 06-sonarqube-code-quality and runs as step 10 in that flow.

## Primary Output

Pull request scan setup
