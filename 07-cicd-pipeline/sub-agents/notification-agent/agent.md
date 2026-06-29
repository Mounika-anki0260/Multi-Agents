---
name: Notification Agent
id: notification-agent
role: sub-agent
parentAgent: 07-cicd-pipeline
step: 19
description: Notify team on success, failure, approval waiting, rollback, and release completion.
triggers:
  - notification-agent
capabilities:
  - step-19
  - notification
---

# Notification Agent

## Purpose

Notify team on success, failure, approval waiting, rollback, and release completion.

## Parent Flow

This sub-agent belongs to 07-cicd-pipeline and runs as step 19 in that flow.

## Primary Output

Notification setup
