# Legacy-Specific Modernization Sub-Agents

These sub-agents create focused modernization guidance for a particular legacy platform or workload type.

## Step-by-Step Sub-Agent Flow

| Step | Sub-Agent | Purpose | Primary Output |
|---|---|---|---|
| 1 | `legacy-modernization-questionnaire-agent` | Ask the legacy technology, modernization goal, artifact availability, compatibility constraints, and target constraints. | Legacy modernization intake |
| 2 | `mainframe-cobol-modernization-agent` | Assess COBOL, CICS, JCL, copybooks, VSAM, DB2, and mainframe integration patterns. | Mainframe modernization path |
| 3 | `vb6-com-modernization-agent` | Assess VB6, COM, Classic ASP, ActiveX, Windows dependencies, and desktop-to-web/API migration concerns. | VB6 modernization path |
| 4 | `oracle-forms-reports-modernization-agent` | Assess Oracle Forms, Reports, PL/SQL packages, triggers, and UI-to-web migration concerns. | Oracle Forms modernization path |
| 5 | `powerbuilder-modernization-agent` | Assess PowerBuilder windows, DataWindows, PowerScript, database access, and reporting patterns. | PowerBuilder modernization path |
| 6 | `dotnet-framework-modernization-agent` | Assess .NET Framework, WebForms, MVC, WCF, Windows Services, and migration to modern .NET. | .NET Framework modernization path |
| 7 | `java-ee-struts-modernization-agent` | Assess Java EE, Struts, JSP, Servlets, EJB, XML configuration, and migration to modern Java services. | Java legacy modernization path |
| 8 | `database-stored-procedure-modernization-agent` | Assess database-heavy logic in stored procedures, packages, triggers, jobs, and views. | Database logic modernization path |
| 9 | `legacy-batch-reporting-modernization-agent` | Assess batch jobs, schedulers, file exchanges, reports, ETL, and operational windows. | Batch/reporting modernization path |
| 10 | `modernization-roadmap-handoff-agent` | Consolidate findings into a roadmap and handoff checklist for architecture and delivery agents. | Modernization roadmap and handoff |

## Mandatory Question Gate

The `legacy-modernization-questionnaire-agent` must ask:

- Which legacy technology family is in scope?
- What modernization outcome is expected?
- Which artifacts are available for analysis?
- Which interfaces, files, data structures, screens, or reports must remain compatible?
- What target platform, language, database, security, and delivery constraints exist?

## Handoff Rules

- Always record assumptions before selecting a migration path.
- Each platform-specific sub-agent must identify automation candidates and manual review items.
- The roadmap handoff must include follow-up work for reverse engineering, target architecture, backend, frontend, QA, quality gates, and CI/CD.

