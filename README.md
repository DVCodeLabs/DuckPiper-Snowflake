# DuckPiper Snowflake Connector

Optional Snowflake connector extension for DuckPiper.

## Requirements

- DuckPiper core extension (`duckpiper.duckpiper`)

## What it adds

- Registers a Snowflake provider form schema into DuckPiper.
- Registers a Snowflake runtime adapter for test/query/introspection.
- Adds Snowflake connection import flow:
  - `Import Connection Settings`
  - `Parse & Fill`
  - Supports JDBC/ODBC strings and Snowflake TOML snippets.
- Restores the Snowflake setup guide file in `DP/system/connection.snowflake.instructions.md`.
- Adds command: `DP: Snowflake Setup Guide`.

## Setup Guide Behavior

- The extension creates `DP/system/connection.snowflake.instructions.md` only when `DP/system` already exists.
- If your project is not initialized yet, run DuckPiper project initialization first.
