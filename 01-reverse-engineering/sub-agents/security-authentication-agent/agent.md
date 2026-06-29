---
name: Security Authentication Agent
id: security-authentication-agent
role: sub-agent
parentAgent: 01-reverse-engineering-documents
step: 10
description: Capture identity provider, login/logout, sessions, tokens, roles, permissions, policies, secrets, and certificates.
triggers:
  - security-authentication-agent
capabilities:
  - step-10
  - security-authentication
---

# Security Authentication Agent

## Purpose

Capture identity provider, login/logout, sessions, tokens, roles, permissions, policies, secrets, and certificates.

## Parent Flow

This sub-agent belongs to 01-reverse-engineering-documents and runs as step 10 in that flow.

## Primary Output

Security and auth flow
