---
name: Dependency Install Agent
id: dependency-install-agent
role: sub-agent
parentAgent: 07-cicd-pipeline
step: 4
description: Install backend, frontend, infrastructure, test, and scanner dependencies with caching where appropriate.
triggers:
  - dependency-install-agent
capabilities:
  - step-4
  - dependency-install
---

# Dependency Install Agent

## Purpose

Install backend, frontend, infrastructure, test, and scanner dependencies with caching where appropriate.

## Parent Flow

This sub-agent belongs to 07-cicd-pipeline and runs as step 4 in that flow.

## Primary Output

Dependency install step
