# DashTask.ai MCP Server

Connect your AI assistant (Cursor, Claude, Grok, ChatGPT) to [DashTask.ai](https://dashtask.ai) — task management, approvals and CRM for small teams.

![DashTask.ai](assets/logo.png)

## Server URL

```
https://dashtask-mcp.stevie-c03.workers.dev/mcp
```

Remote MCP over HTTP with OAuth 2.1 sign-in. No API key needed.

## Install in Cursor

Add to `~/.cursor/mcp.json` (or `.cursor/mcp.json` in a project):

```json
{
  "mcpServers": {
    "dashtask": { "url": "https://dashtask-mcp.stevie-c03.workers.dev/mcp" }
  }
}
```

Cursor opens a DashTask.ai sign-in window. Choose **Connect as Me** or **Connect as AI Agent** and pick your bot.

## What it can do

- List, create and update tasks and subtasks; add comments
- Join open tasks, move work to In progress or Awaiting approval
- Manage tags, projects and dimensions
- Create and update CRM contacts and leads (when CRM access is granted)

## Safety rules

- Agents never mark tasks Done — the human owner approves.
- Agents never take over someone else's in-progress task without confirmation.
- Every action runs under the signed-in account's permissions.

## Requirements

A DashTask.ai account (7-day free trial). Sign up at https://dashtask.ai.

## Support

support@dashtask.ai · [Privacy](https://dashtask.ai/privacy) · [Terms](https://dashtask.ai/terms)

## License

MIT
