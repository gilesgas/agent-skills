---
name: buildkite
description: "Interacts with Buildkite pipelines, builds, agents, and CI/CD workflows via the MCP server. Use when asked to manage builds, view logs, check pipeline status, or work with Buildkite."
---

# Buildkite MCP Server Skill

This skill provides integration with Buildkite through the Model Context Protocol (MCP).

## What this skill does

The Buildkite MCP server enables you to:

- **Pipeline Management**: List and view pipeline configurations, create and update pipelines
- **Build Operations**: Trigger builds, view build details, logs, and artifacts
- **Job Management**: Monitor job execution, read and search logs, unblock jobs
- **Test Engine**: Access test suite data, view test runs and failed executions
- **Cluster and Queue Management**: List and inspect clusters and queues
- **Annotations**: List build annotations for debugging and context

## How to use it

Once configured, you can ask for help with Buildkite tasks like:

- "Show me the status of recent builds for the docs pipeline"
- "List all failed builds from today"
- "View the logs for the failed job in build #123"
- "Show me the test results for the latest build"
- "Trigger a new build on the feature branch"
- "What annotations are on the latest build?"

## Authentication

The Buildkite MCP server uses OAuth. When you first use the skill, you'll be prompted to authorize in your browser. No manual API token configuration is required.

## Configuration

This server is configured in the skill's `mcp.json` file at `~/.config/agents/skills/buildkite/mcp.json`, using the remote Buildkite MCP server at `https://mcp.buildkite.com/mcp`.
