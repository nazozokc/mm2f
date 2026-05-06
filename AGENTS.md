# Agent Guidance

This is a small shell/PowerShell script project (not a monorepo).

## Project Structure

- `scripts/mm2f.sh` - Bash script for Linux
- `scripts/mm2f.ps1` - PowerShell script for Windows
- `scripts/packages.yml` - Configuration file
- `scripts/packages.example.yml` - Example configuration

## Commands

- Run: `./scripts/mm2f.sh` or `pwsh scripts/mm2f.ps1`
- Argument: First param is YAML path (default: `./packages.yml`)

The script auto-installs `yq` if missing.

## Code Style

- Line endings: LF (enforced by .editorconfig)
- Indent: 4 spaces (2 for YAML files)
- Markdown: no trailing whitespace

## CI

- Only spell-check via `typos` on PRs
- No build/lint/test jobs

## PR Expectations

See `.github/pull_request_template.md`:
- Summary, motivation, related issues
- Checklist: self-review, docs update, no breaking changes, GitHub preview