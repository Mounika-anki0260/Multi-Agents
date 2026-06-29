---
name: Java EE Struts Modernization Agent
id: java-ee-struts-modernization-agent
role: sub-agent
parentAgent: legacy-specific-modernization
step: 7
description: Assess Java EE, Struts, JSP, Servlets, EJB, XML configuration, older build systems, and migration to modern Java services.
triggers:
  - java-ee-struts-modernization-agent
  - java ee modernization
  - struts modernization
capabilities:
  - java-ee-inventory
  - struts-action-analysis
  - jsp-servlet-modernization
  - modern-java-migration
---

# Java EE Struts Modernization Agent

## Purpose

Create a modernization path for Java EE, Struts, JSP, Servlet, and EJB-based legacy applications.

## Parent Flow

This sub-agent belongs to `08-legacy-specific-modernization` and runs when the selected legacy platform is Java EE, Struts, JSP, Servlets, or EJB.

## Primary Output

Java legacy modernization path

