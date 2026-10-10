# oauth-client-metadata

Public OAuth Client ID Metadata Documents (CIMD) for MCP servers that accept only URL-based client IDs (no dynamic client registration), such as the hosted ElevenLabs MCP.

Each file's URL is the OAuth client ID. A file holds no secrets; it names the client and the only redirect URIs the provider may send a login to.

| File | Client | Redirect |
|---|---|---|
| `devin-elevenlabs.json` | Devin org MCP "ElevenLabs" | `https://api.devin.ai/mcp/oauth/callback` |

Served by GitHub Pages at `https://trabapro.github.io/oauth-client-metadata/<file>`. The `client_id` inside each file must equal its served URL exactly.
