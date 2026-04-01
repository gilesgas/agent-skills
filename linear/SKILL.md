---
name: linear
description: "Interacts with Linear for issue tracking, project management, and team workflows via the MCP server. Use when asked to create, update, or search Linear issues, projects, or cycles."
---

# Linear MCP Server Skill

This skill provides integration with Linear through the Model Context Protocol (MCP).

## What this skill does

The Linear MCP server enables you to:

- **Issue Management**: Create, read, update, and manage Linear issues
- **Project Management**: Access and manage Linear projects, teams, and workflows
- **Team Operations**: Work with Linear teams, members, and assignments
- **Status Tracking**: Monitor issue states, priorities, and progress
- **Search and Filtering**: Query issues and projects with various filters
- **Comments and Updates**: Add comments and updates to Linear issues
- **Labels and Tags**: Manage issue labels and project tags

## How to use it

Once configured, you can ask for help with Linear tasks like:

- "Create a new issue in Linear for the bug fix"
- "Show me all high-priority issues in the frontend team"
- "Update the status of issue LIN-123 to In Progress"
- "Add a comment to issue LIN-456 about the deployment"
- "List all issues assigned to me in the current cycle"
- "Search for issues related to authentication"

## Authentication

The Linear MCP server uses OAuth. When you first use the skill, you'll be prompted to authorize in your browser. No manual API token configuration is required.

## Configuration

This server is configured in the skill's `mcp.json` file at `~/.config/agents/skills/linear/mcp.json`, using the remote Linear MCP server at `https://mcp.linear.app/sse`.
