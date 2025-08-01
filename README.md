Install this MCP server by adding the following JSON code to jour config file

```json

{
  "mcpServers": {
    "server": {
      "command": "uvx",
      "args": [
        "--from",
        "git+https://github.com/Nikola-Vukasinovic/mcp-server-chess-build.git",
        "chess"
      ]
    }
  }
}
```