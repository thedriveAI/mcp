# Installing The Drive AI MCP

This is a hosted remote server. There is nothing to clone, build or run.

1. Add this server to the client's MCP config:

```json
{
  "mcpServers": {
    "thedriveai": {
      "type": "streamableHttp",
      "url": "https://mcp.thedrive.ai/mcp"
    }
  }
}
```

2. On first use, the client opens a browser for OAuth sign-in to The Drive AI. The person signs in with Google, Microsoft, GitHub or email. No API key is needed.

3. Check it works by calling `get_current_user`, which returns the person's workspaces.

Docs: https://docs.thedrive.ai/integrations/mcp-server
