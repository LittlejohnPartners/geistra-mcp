# Installing Geistra in Cline

Geistra is a hosted MCP server. There is nothing to download, build or run locally.

1. In Cline, open **MCP Servers → Remote Servers**.
2. Server name: `geistra`. Server URL: `https://mcp.geistra.com/mcp`. Add it.
3. Cline opens Geistra's sign-in page in the browser. Sign in (or create a free account at https://geistra.com) and click **Allow**.

Equivalent entry in `cline_mcp_settings.json`:

```json
{
  "mcpServers": {
    "geistra": {
      "type": "streamableHttp",
      "url": "https://mcp.geistra.com/mcp"
    }
  }
}
```

No API key is needed: sign-in uses OAuth, and the connection acts with the person's own permissions.
