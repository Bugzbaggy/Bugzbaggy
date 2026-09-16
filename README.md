# Hi, I'm Renz 👋

SQL Server DBA working on high-volume messaging infrastructure — Always On
availability groups across AWS and GCP, distributed AGs spanning four regions,
and the CI/CD and observability that keeps them honest.

Most of what I publish here started as something I needed at 3am.

---

### 🛠 Operations & HADR

| Project | What it does |
|---|---|
| [**mssql-hadr-ops**](https://github.com/Bugzbaggy/mssql-hadr-ops) | PowerShell for safe Always On failover and rolling patching — pre-flight validation, prepare/resume across reboots, AWS/GCP/Azure driver updates |

### 🤖 AI + databases

| Project | What it does |
|---|---|
| [**mssql-dba-mcp**](https://github.com/Bugzbaggy/mssql-dba-mcp) | Read-only MCP server giving an AI agent real diagnostics across a SQL Server fleet — structurally incapable of writing |
| [**mssql-data-api**](https://github.com/Bugzbaggy/mssql-data-api) | Governed read-only REST/GraphQL/MCP API over curated stored procedures, built on Data API Builder |

### 🚦 Database CI/CD & quality

| Project | What it does |
|---|---|
| [**mssql-dacpac-cicd**](https://github.com/Bugzbaggy/mssql-dacpac-cicd) | DACPAC build, Flyway migrations, policy gates, staged promotion with approvals |
| [**tsqlt-integration-pipeline**](https://github.com/Bugzbaggy/tsqlt-integration-pipeline) | Every PR gets a disposable SQL Server 2022 — publish, integrity-check, tSQLt tests, coverage, PR comment |
| [**nitsql**](https://github.com/Bugzbaggy/nitsql) | Multi-dialect SQL analyzer: 52 rules across SQL Server, PostgreSQL, Oracle, MySQL, SQLite |
| [**schemalore**](https://github.com/Bugzbaggy/schemalore) | Documents SSDT objects and gates commits on documentation coverage |

### ✍️ Writing

[**Presentations**](https://github.com/Bugzbaggy/Presentations) — field notes
from real incidents:

- [In-place upgrading an Always On cluster to Windows Server 2025](https://github.com/Bugzbaggy/Presentations/blob/main/posts/upgrading-always-on-to-windows-server-2025.md)
- [A read-only SQL MCP, powered by dbatools](https://github.com/Bugzbaggy/Presentations/blob/main/posts/sql-server-mcp-server-for-dbas.md)
- [Every pull request gets its own SQL Server](https://github.com/Bugzbaggy/Presentations/blob/main/posts/per-pr-database-integration-testing.md)

---

### A recurring theme

Most of these share one idea: **make the dangerous thing structurally
impossible rather than forbidden by policy.**

A read-only MCP that cannot write. A data API whose read-only status is
asserted by a CI gate, not a convention. A test pipeline where only one
unambiguous check can block you. Guardrails you can't forget to follow beat
guardrails you're supposed to remember.

📫 Issues and PRs welcome on any of these.
