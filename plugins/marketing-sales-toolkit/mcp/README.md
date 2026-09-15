# MCP Server Templates

These are example MCP server configurations for connecting marketing/sales tools (CRM, email, analytics) to Claude Code. They are templates only — no credentials are included. Copy the one you need into your project's `.mcp.json`, fill in the placeholder values (or reference environment variables), and restart Claude Code.

None of these servers are bundled or auto-installed by this plugin. They point at third-party MCP server packages; verify each package's source and publisher before adding it to your `.mcp.json`, since MCP servers run with your tool permissions.

| File | Connects to | Typical use |
|---|---|---|
| `hubspot.mcp.json` | HubSpot CRM | Pull/update contacts, deals, and pipeline stages for sales skills |
| `google-analytics.mcp.json` | Google Analytics (GA4) | Pull traffic/conversion data for campaign measurement plans |
| `sendgrid.mcp.json` | SendGrid | Send/inspect transactional or campaign email |

## Usage

1. Copy the relevant JSON block into your project's `.mcp.json` under `"mcpServers"`.
2. Replace every `<...>` placeholder with your own value or an environment variable reference.
3. Never commit real API keys — use `${ENV_VAR}` substitution or your OS keychain where your MCP client supports it.
