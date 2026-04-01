# agents

Personal configuration and command definitions for AI coding agents.

This repo is the source of truth. Agent tools (OpenCode, etc.) symlink into it rather than maintaining their own copies.

## Structure

```
opencode/
  AGENTS.md          # Global rules injected into every OpenCode session
  commands/          # Slash command definitions
    explain.md       # /explain <file or topic>
    fix.md           # /fix <error or test name>
    pr.md            # /pr — draft a pull request description
    refactor.md      # /refactor <file> [instructions]
    review.md        # /review — review staged or recent changes
    search.md        # /search <query> — find where something is implemented
    standup.md       # /standup — summarize recent activity
```

## Setup

Symlink the commands directory to where OpenCode expects it:

```sh
ln -s ~/dev/agents/opencode/commands ~/.config/opencode/commands
```
