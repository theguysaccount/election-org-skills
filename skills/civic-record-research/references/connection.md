# Connect Election.org

The skill needs Election.org's read-only MCP server. It does not itself install a connector, grant permissions or contain an API key. The full Claude plugin includes this connection configuration.

## Claude Code

If the plugin is not installed, the user can add the public server:

```sh
claude mcp add --transport http election-org https://election.org/api/mcp
```

Review the connection permissions in Claude. No OAuth or API key is required. Do not enable unrelated tools or bypass approval prompts. Tool names may have an `mcp__election-org__` prefix.

## Claude web / Cowork

Use the approved Election.org directory plugin when available, or add `https://election.org/api/mcp` as a custom connector if the account supports it. Directory publication is separate from this downloadable skill. Ask the user to complete any required account or access approval. Do not imply the connector exists when it does not.

## Without the connection

Explain that live figures have not been checked. You may offer the public API documentation at https://election.org/data/api or the relevant public site page; never fabricate a tool result or request a private API credential for this anonymous server.
