# CLAUDE.md

This file provides guidance for AI assistants working in this repository.

## Project Overview

**Name:** IoTs
**Purpose:** General Research Trends and Current Status on IoT Facets
**Status:** Early-stage research/documentation repository for Internet of Things topics

This repository is intended to collect, organize, and present research on IoT trends, technologies, and current developments across various IoT domains.

## Repository State

As of the initial commit (2026-03-03), this repository contains only a README. There is no source code, no build system, and no configured dependencies yet. The project is in its setup/planning phase.

## Git Workflow

### Branches

- `master` — stable, reviewed content
- `claude/<session-id>` — AI-assisted development branches (e.g., `claude/claude-md-mmbbjj9mpffwwxif-eLgNK`)

### Commit Conventions

Write clear, descriptive commit messages in imperative mood:

```
Add section on MQTT protocol security
Update edge computing trends with 2026 data
Fix broken references in networking overview
```

### Push Instructions

Always push using:

```bash
git push -u origin <branch-name>
```

Branch names for AI sessions must start with `claude/` and end with the session ID.

## Development Guidelines

### Adding Content

Since this is a research/documentation repository, contributions will primarily be Markdown documents. Follow these conventions:

- Place topic documents in organized subdirectories (e.g., `docs/`, `research/`, `protocols/`)
- Use `README.md` in each subdirectory to describe its contents
- Prefer `.md` (Markdown) for all documentation
- Use relative links between documents

### File Naming

- Use lowercase with hyphens for filenames: `edge-computing.md`, `mqtt-security.md`
- Group related documents in appropriately named directories

### Markdown Style

- Use ATX-style headings (`#`, `##`, `###`)
- Include a top-level `# Title` in every document
- Use fenced code blocks with language identifiers when showing code or configs
- Keep line length reasonable (80–120 characters for prose)

### If Source Code Is Added

When this project grows to include code (scripts, tools, data processing, etc.), document the chosen language, toolchain, and conventions here. Likely candidates for an IoT research project:

- **Python** — data analysis, scripts, simulations
- **JavaScript/Node.js** — dashboards, REST APIs, MQTT clients
- **Shell scripts** — automation, environment setup

For any language added, ensure a corresponding dependency file is committed (`requirements.txt`, `package.json`, etc.) along with a `.gitignore` suited to that ecosystem.

## Remote Configuration

The git remote (`origin`) is configured to a local proxy server. No authentication tokens or secrets should be committed to this repository.

## Key Conventions for AI Assistants

1. **Do not invent project structure** — only add files consistent with the stated purpose (IoT research documentation)
2. **Ask before adding a build system or language runtime** — the project has no toolchain yet; confirm with the user before introducing one
3. **Keep changes focused** — match the scope of what was requested; do not add unrequested files or refactoring
4. **Commit and push** completed work to the designated `claude/` branch
5. **No secrets** — never commit API keys, credentials, or tokens
