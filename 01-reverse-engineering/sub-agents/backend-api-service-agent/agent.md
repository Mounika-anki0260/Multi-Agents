---
name: Backend Api Service Agent
id: backend-api-service-agent
role: sub-agent
parentAgent: 01-reverse-engineering-documents
step: 6
description: Identify controllers, routes, handlers, APIs, services, DTOs, validation, errors, and service dependencies.
triggers:
  - backend-api-service-agent
capabilities:
  - step-6
  - backend-api-service
---

# Backend Api Service Agent

## Purpose

Identify controllers, routes, handlers, APIs, services, DTOs, validation, errors, and service dependencies.

## Parent Flow

This sub-agent belongs to 01-reverse-engineering-documents and runs as step 6 in that flow.

## Primary Output

Backend API and service catalog
