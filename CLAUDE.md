# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Mintlify documentation site for Hermes. MDX files with YAML frontmatter, configured via `docs.json`.

## Development Commands

```bash
# Install Mintlify CLI (requires Node LTS, not v25+)
npm i -g mint

# Start dev server at http://localhost:3000
mint dev

# Update CLI if issues occur
mint update
```

## Architecture

- `docs.json` - Navigation structure, theme, colors, fonts, and site settings
- `*.mdx` files - Documentation pages with YAML frontmatter
- `snippets/` - Reusable content snippets
- `images/` and `logo/` - Static assets

## Working Relationship

- Push back on ideas when warranted - cite sources and explain reasoning
- ALWAYS ask for clarification rather than making assumptions
- NEVER lie, guess, or make up information

## Content Strategy

- Document just enough for user success - not too much, not too little
- Make content evergreen when possible
- Search for existing information before adding new content to avoid duplication
- Check existing patterns for consistency
- Start by making the smallest reasonable changes

## Frontmatter Requirements

Every MDX file must have:
```yaml
---
title: "Clear, descriptive page title"
description: "Concise summary for SEO/navigation"
---
```

## Writing Standards

- Second-person voice ("you")
- Prerequisites at start of procedural content
- Test all code examples before publishing
- Match style and formatting of existing pages
- Include both basic and advanced use cases
- Language tags on all code blocks
- Alt text on all images
- Relative paths for internal links (e.g., `/quickstart`, not absolute URLs)

## Git Workflow

- NEVER use `--no-verify` when committing
- Ask how to handle uncommitted changes before starting
- Create a new branch when no clear branch exists for changes
- Commit frequently throughout development

## Do Not

- Skip frontmatter on any MDX file
- Use absolute URLs for internal links
- Include untested code examples
- Make assumptions - always ask for clarification
