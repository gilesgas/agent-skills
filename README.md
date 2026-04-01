# Agent skills

MCP server skills for AI coding agents. These skills are optimized for [Sourcegraph Amp](https://ampcode.com), but should be usable by other AI tools that support MCP servers and skill/instruction files.

## Installation

Copy the skill directories into your Amp skills directory:

```bash
cp -r buildkite github linear notion ~/.config/agents/skills/
```

`~/.config/agents/skills/` is the default user-wide skills directory for Amp. Skills installed here are available across all projects.

## Configuration

For the GitHub skill, you need to configure your classic GitHub personal access token in `github/mcp.json` before use. Replace the placeholder value in the `GITHUB_PERSONAL_ACCESS_TOKEN` field with your token.
