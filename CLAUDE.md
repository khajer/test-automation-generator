# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Claude Code plugin called "test-automation-generator" that generates automation tests, specifically focusing on Playwright project initialization.

## Architecture

### Plugin Structure

This follows the standard Claude Code plugin architecture:

- **.claude-plugin/plugin.json**: Plugin manifest defining name, description, version, and author
- **commands/**: Custom slash commands that users can invoke
  - `init.md`: Initializes a new Playwright project
- **agents/**: Directory for specialized agent definitions (currently empty)
- **skills/**: Directory for reusable skill definitions (currently empty)
- **hooks/**: Directory for event-driven hooks (currently empty)

### Plugin Manifest

The plugin is registered in `.claude-plugin/plugin.json`:
- Name: test-automation-generator
- Version: 0.1.0
- Description: Generate automation test

### Command Structure

Commands are defined as markdown files in the `commands/` directory with YAML frontmatter:
- Frontmatter includes `description` field for command documentation
- Command body contains the prompt/instructions that get expanded when invoked

## Development

### Git Workflow

- Main branch: `main`
- Development branch: `develop`
- Feature branches should be created from and merged back to `develop`

### Adding New Commands

Create a new `.md` file in the `commands/` directory with:
```markdown
---
description: Brief description of the command
---

# Command Name

Command instructions and prompt that will be executed when invoked.
```

### Adding New Skills

Create skill definitions in the `skills/` directory following Claude Code skill conventions.

### Adding New Agents

Create agent definitions in the `agents/` directory following Claude Code agent conventions.

### Adding New Hooks

Create hook scripts in the `hooks/` directory to respond to events like tool calls or user interactions.
