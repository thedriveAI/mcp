# The Drive AI MCP

[The Drive AI](https://thedrive.ai) lets your AI agent work on your company files. Find files by what's in them, read PDFs and sheets, and reorganize folders across Google Drive, OneDrive, SharePoint and Dropbox. Every change is previewed first and can be undone.

```
https://mcp.thedrive.ai/mcp
```

Remote server, streamable HTTP, OAuth sign-in. Nothing to install or host.

## Connect

**Claude (web, desktop, mobile)**
Settings > Connectors > Add custom connector, paste the URL above, sign in.

**ChatGPT**
Settings > Connectors > Create, paste the URL above, sign in.

**Claude Code**
```bash
claude mcp add --transport http thedriveai https://mcp.thedrive.ai/mcp
```

**Codex CLI**
```bash
codex mcp add --url https://mcp.thedrive.ai/mcp thedriveai
```

**Gemini CLI**
```bash
gemini extensions install https://github.com/thedriveAI/mcp
```

**VS Code**
```bash
code --add-mcp '{"name":"thedriveai","type":"http","url":"https://mcp.thedrive.ai/mcp"}'
```

**Cursor, Windsurf and anything else**
```json
{
  "mcpServers": {
    "thedriveai": {
      "url": "https://mcp.thedrive.ai/mcp"
    }
  }
}
```

The first call opens a browser to sign in to The Drive AI (Google, Microsoft, GitHub or email).

## What your agent can do

- **Find:** browse folders, search by meaning, grep inside documents, find duplicates
- **Read:** PDFs, docs, sheets and scans, page by page
- **Change:** create, move, rename and update files as a changeset you preview, apply and undo
- **Save:** turn attachments, uploads and URLs into files in your workspace
- **Share:** check and change who has access
- **Verify:** sign documents your agent made and check them later

## Try it

- "Sort my Inbox folder by client and year"
- "Find every contract that renews in Q1 and list the renewal dates"
- "Rename these scans by vendor and invoice date, show me first"

## Also here

- `gemini-extension.json` for Gemini CLI
- `.claude-plugin/` for Claude Code plugins
- `.cursor-plugin/` and `mcp.json` for Cursor
- `llms-install.md` for agents installing this server
- Skills for agents: [thedriveAI/skills](https://github.com/thedriveAI/skills)

## Links

[Docs](https://docs.thedrive.ai/integrations/mcp-server) · [thedrive.ai/mcp](https://thedrive.ai/mcp) · Official MCP Registry: `ai.thedrive/thedriveai` · contact@thedrive.ai
