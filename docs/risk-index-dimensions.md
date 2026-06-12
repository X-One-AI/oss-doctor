# Risk Index Dimensions

These dimensions are allowed only when they support an MCP server catalog entry.

| Dimension | Meaning | Evidence Source | Destination |
|---|---|---|---|
| `repository` | Source repository URL | GitHub repository URL | `mcp-risk-index.maintenance.repository` |
| `source_checked_at` | Date maintainer checked public source metadata | maintainer review timestamp | `mcp-risk-index.maintenance.source_checked_at` |
| `archived` | Whether repository is archived | GitHub repository metadata | future maintenance note |
| `pushed_at` | Latest public push date | GitHub repository metadata | release or activity signal |
| `security_policy` | Whether maintainers document security reporting | `SECURITY.md` URL | future limitation/evidence note |
| `license` | License file or package metadata | repository file/package metadata | future limitation/evidence note |
| `install_command` | Documented startup command | README/package docs | launch evidence |

## Rules

- Do not convert these dimensions into a score.
- Do not call a project safe, unsafe, trusted, or abandoned from these dimensions alone.
- Add limitations when metadata is stale, missing, or ambiguous.
- Prefer deleting a dimension over publishing a noisy proxy.
