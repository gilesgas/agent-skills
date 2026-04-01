---
name: github
description: "Interacts with GitHub repositories, issues, and pull requests via the MCP server. Use when asked to create PRs, review code, manage issues, search repos, or work with GitHub."
---

# GitHub MCP Server Skill

This skill provides integration with GitHub through the Model Context Protocol (MCP) using the `@modelcontextprotocol/server-github` package.

## What this skill does

The GitHub MCP server enables you to:

- **Repository Management**: Browse repos, get file contents, create branches, push files
- **Pull Requests**: Create, review, list, merge PRs and manage PR reviews
- **Issues**: Create, update, list, search, and comment on issues
- **Code Search**: Search code, repositories, issues, and users across GitHub
- **Commits**: List and inspect commits on branches

## How to use it

Once configured, you can ask for help with GitHub tasks like:

- "Create a new branch and PR for this change"
- "List open PRs assigned to me in buildkite/docs-private"
- "Search for issues related to authentication"
- "Review the files changed in PR #123"
- "Merge PR #456 with a squash merge"
- "Get the contents of README.md from the main branch"
- "Push these changes to my feature branch"

## Authentication

The GitHub MCP server uses a Personal Access Token (PAT). The token needs:

- **Classic PAT**: `repo` scope for full private repository access
- **Fine-grained PAT**: `Contents`, `Pull requests`, `Issues` read/write permissions on target repos

## Configuration

This server is configured in the skill's `mcp.json` file at `~/.config/agents/skills/github/mcp.json`. The PAT is stored directly in that file.

To create a PAT, visit: https://github.com/settings/tokens
