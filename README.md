<img src="assets/geistra-icon-512.png" alt="Geistra" width="96" />

# Geistra MCP server

Geistra is shared memory for your AI apps: Spaces of records, files and plans that Claude, ChatGPT, Gemini, Cursor or any app that supports MCP can read and update, under your own permissions, and that you can share with the people you invite. Every change is kept, with who made it and through which AI.

**This repository holds only connection settings and documentation.** Geistra is a hosted service; its source code is not here.

- Website: https://geistra.com
- Server address: `https://mcp.geistra.com/mcp` (Streamable HTTP, OAuth sign-in)
- Official MCP Registry: `com.geistra/geistra`

## Connect

Add a remote MCP server with the address above. Your app opens Geistra's sign-in page; sign in (or create a free account) and click **Allow**. No API key is needed.

| App | How |
|---|---|
| Claude | Settings → Connectors → add a custom connector with the address. Guide: https://geistra.com/docs/claude |
| Claude Code | `claude mcp add --transport http geistra https://mcp.geistra.com/mcp`, then `/mcp` → geistra → Authenticate |
| ChatGPT | Apps, or a custom MCP server at `https://mcp.geistra.com/mcp/chatgpt`. Guide: https://geistra.com/docs/chatgpt |
| Cursor | Use [`.mcp.json`](.mcp.json) from this repo, or add the address in Settings → MCP |
| Gemini CLI | `gemini extensions install https://github.com/LittlejohnPartners/geistra-mcp` |
| Cline | See [llms-install.md](llms-install.md) |
| VS Code, Zed, Goose, Windsurf and others | Add a remote (HTTP) MCP server with the address above |

## What your AI can do with it

Find and update records, read and show files, follow plans, hand work to another person or AI app, catch up on what changed since it last looked, and set up apps, reminders and scheduled tasks. Sensitive actions wait for your approval in Geistra itself, whatever the AI asks: sharing outside a Space, inviting people or changing their access, publishing a public link, running a saved action (such as sending a text) and applying a draft. Full list: https://geistra.com/features

To make your AI use Geistra without being asked, add these instructions to it: https://geistra.com/docs/ai-instructions

## Privacy

Your data is stored in the U.S., encrypted, never used to train AI, and can be deleted at any time. Each AI app connects with its own permissions, which you can change or revoke in Geistra's web app. Privacy policy: https://geistra.com/privacy

Operated by Littlejohn Partners LLC. For businesses: [Geistra Pro](https://geistra.pro).

## License

The files in this repository (connection settings and documentation) are under the [MIT License](LICENSE). It covers only these files: it grants no rights to the hosted Geistra service, its source code, or the Geistra name and logo.
