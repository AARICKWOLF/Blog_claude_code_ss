# Getting Started with Claude Code — Internal Team Guide

Claude Code is Anthropic's agentic coding tool. It reads your codebase, edits files, runs commands, and integrates with your terminal, IDE, browser, and apps.

---

## Overview

Claude Code operates in an **agentic loop**:

1. Gather context
2. Take action
3. Verify results

### Why Our Team Uses Claude Code

- ⚡ Ship faster
- 🔁 Automate Git workflows
- 🧪 Generate and fix tests
- 🐛 Debug automatically
- 📝 Generate documentation
- 🤝 Enforce team standards via `CLAUDE.md`

---

## What You Can Do

- Ask questions about your codebase  
- Edit code across multiple files  
- Run and fix tests  
- Search and navigate your project  
- Perform Git operations  
- Automate CI workflows  
- Connect external tools (Slack, Jira, Supabase)

---

## Platforms

| Platform | Best For | Features |
|--------|----------|----------|
| Terminal CLI | Full control | All features |
| VS Code | IDE workflow | Inline diffs |
| JetBrains | IntelliJ users | Interactive diffs |
| Desktop App | Visual workflows | Parallel sessions |
| Web | No setup | Cloud execution |
| GitHub Actions | CI/CD | Automated review |

---

## Quickstart

### Install

#### macOS / Linux

```bash
curl -fsSL https://claude.ai/install.sh | bash
```

#### Windows

```powershell
winget install Anthropic.ClaudeCode
```

---

### Run Claude Code

```bash
cd your-project
claude
```

---

### Example Commands

```bash
# Understand codebase
claude "summarize this codebase"

# Fix bugs
claude "fix login validation"

# Run tests
claude "run tests and fix failures"
```

---

## Agent Loop Architecture

```text
User Request
   ↓
Gather Context
   ↓
Take Action
   ↓
Verify Results
   ↓
Repeat Until Complete
```

---

## Available Tools

| Tool | Function |
|-----|----------|
| Read | Read files |
| Write | Edit files |
| Bash | Run commands |
| Grep | Search |
| Glob | File matching |
| MCP | External integrations |

---

## Common Workflow

### Explore

```bash
claude "explain auth system"
```

### Plan

```bash
claude "create plan to add OAuth"
```

### Implement

```bash
claude "implement plan"
```

### Commit

```bash
claude "commit changes"
```

---

## CLAUDE.md Example

```md
# CLAUDE.md

## Stack
- TypeScript
- Next.js
- Supabase

## Commands
pnpm build
pnpm test
pnpm lint

## Rules
Use functional components
Follow conventional commits
```

---

## CLI Reference

### Start session

```bash
claude
```

### One-shot query

```bash
claude -p "explain architecture"
```

### Resume session

```bash
claude -c
```

---

## Supabase Integration

Install templates:

```bash
npx claude-code-templates@latest --mcp supabase
```

Capabilities:

- Schema management
- Migration generation
- Security auditing
- Type generation
- Query optimization

---

## Best Practices

- Use `/clear` between tasks
- Use version control
- Always review generated code
- Keep CLAUDE.md concise

---

## FAQ

<details>
<summary>What subscription is required?</summary>

Claude Code requires Pro, Max, Team, or Enterprise plan.

</details>

<details>
<summary>Does Claude modify files automatically?</summary>

Claude asks permission unless auto-accept mode is enabled.

</details>

---

## Resources

Official Docs  
https://code.claude.com/docs

GitHub  
https://github.com/anthropics/claude-code

---

## Internal Notes

Maintained by Closefuture Team
