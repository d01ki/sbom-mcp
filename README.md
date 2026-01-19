# sbom-mcp

## MCP Server Configuration

This section outlines the configuration for the MCP server, which can be managed via a JSON file or directly within the application's setup.

```json
{
  "server_reference": "default-mcp-server",
  "servers": {
    "mcp-security-server": {
      "type": "fastapi",
      "url": "http://localhost:8000",
      "command": "uvicorn mcp_server:app",
      "args": ["--reload", "--port", "8000"]
    }
  }
}
```
