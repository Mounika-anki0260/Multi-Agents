---
name: Database Connection Agent
id: database-connection-agent
role: sub-agent
parentAgent: 03-backend
step: 5
description: Set up database connection, pooling, migrations, ORM/SQL mapper/direct SQL, and local database configuration.
triggers:
  - database-connection-agent
capabilities:
  - step-5
  - database-connection
---

# Database Connection Agent

## Purpose

Set up database connection, pooling, migrations, ORM/SQL mapper/direct SQL, and local database configuration.

## Parent Flow

This sub-agent belongs to 03-backend and runs as step 5 in that flow.

## Primary Output

Database connectivity
