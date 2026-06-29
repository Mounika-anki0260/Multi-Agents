---
name: Source Checkout Agent
id: source-checkout-agent
role: sub-agent
parentAgent: 07-cicd-pipeline
step: 3
description: Configure repository checkout, branch filters, pull request triggers, tags, submodules, and permissions.
triggers:
  - source-checkout-agent
capabilities:
  - step-3
  - source-checkout
---

# Source Checkout Agent

## Purpose

Configure repository checkout, branch filters, pull request triggers, tags, submodules, and permissions.

## Parent Flow

This sub-agent belongs to 07-cicd-pipeline and runs as step 3 in that flow.

## Primary Output

Source checkout setup
