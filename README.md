# VS Code Setups

A collection of `.vscode` configuration folders for different development tasks.
Each subdirectory is self-contained — open it as a VS Code workspace root and it
will apply the correct extensions, settings, launch configurations, and tasks.

## Environments

| Directory | Focus | Key Extensions |
|---|---|---|
| `dotnet-console/` | C# .NET console apps (not web) | C# Dev Kit, .NET Test Explorer, DocComment |
| `rust/` | Rust development | rust-analyzer, CodeLLDB, Crates, Even Better TOML |
| `nushell/` | Nushell script authoring | Nushell language server |
| `sqlserver/` | SQL Server database queries | MSSQL (official), SQLTools + MSSQL driver |
| `duckdb/` | DuckDB analytical queries | SQLTools + DuckDB driver, DuckDB shell, Parquet viewer |
| `python-datawrangler/` | Python data science + DataWrangler | Python, Pylance, Ruff, Jupyter, DataWrangler |

## Usage

1. Open any subdirectory as the root folder in VS Code.
   ```bash
   code dotnet-console
   code rust
   code duckdb
   ```
2. When prompted, install the recommended extensions.
3. Start coding — the `.vscode` folder will configure the editor automatically.

## Scope

These configurations are intentionally focused on **non-web** development:
console apps, scripts, databases, and data analysis. No web framework
extensions, no live-server, no browser debuggers.

## Shared .gitignore

The root `.gitignore` covers common OS files, build artifacts (`bin/`, `obj/`,
`target/`), and IDE clutter. Each subfolder is designed to be independent, so
you can copy it out into a real project when ready.
