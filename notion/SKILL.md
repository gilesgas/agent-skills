---
name: notion
description: "Interacts with Notion workspaces via the remote MCP server. Use when asked to read, create, update, or search Notion pages, databases, comments, or blocks."
---

# Notion MCP Server Skill

This skill provides integration with Notion through the Model Context Protocol (MCP) using Notion's hosted remote server.

## What this skill does

The Notion MCP server enables you to:

- **Pages**: Create, retrieve, update, and move pages
- **Blocks**: Read and append block children, delete blocks
- **Data sources (databases)**: Query, create, update, and retrieve data sources and their templates
- **Search**: Search across all connected Notion content
- **Comments**: Create and retrieve comments on pages
- **Users**: List workspace users

## How to use it

Once configured, you can ask for help with Notion tasks like:

- "Find the page titled 'Customer Private S3 Bucket' in Notion"
- "Create a new page under the Engineering wiki"
- "Search Notion for documentation about job log archiving"
- "Add a comment to a Notion page"
- "Query a database for all items with status 'In Progress'"
- "Get the contents of a specific Notion page"

## Authentication

The Notion MCP server uses OAuth. When you first use the skill, you'll be prompted to authorize in your browser. No manual API token configuration is required.

## Configuration

This server is configured in the skill's `mcp.json` file at `~/.config/agents/skills/notion/mcp.json`, using the remote Notion MCP server at `https://mcp.notion.com/sse`.
