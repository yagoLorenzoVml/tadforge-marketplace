# WPP ESMAP Marketplace

Claude Code marketplace containing `manolo-agent`, an Adobe Experience Platform delivery agent for the IKEA account.

## Install from GitHub

Add the marketplace using its GitHub `owner/repository` name:

```text
/plugin marketplace add <owner>/<repository>
/plugin install manolo-agent@wppesmap
```

Run `/reload-plugins` if installing in an existing session. The plugin connects automatically to the bundled remote AEP MCP server. Use `/mcp` to review its connection or complete authentication if the server requests it.

## Test locally

From a Claude Code session, add this repository by absolute path:

```text
/plugin marketplace add <absolute-path-to-this-repository>
/plugin install manolo-agent@wppesmap
```

The installed subagent appears as `manolo-agent:manolo-agent`. Its skills are namespaced under `manolo-agent`, for example:

```text
/manolo-agent:aep-sandbox-audit
/manolo-agent:aep-schema-design
/manolo-agent:aep-client-context
```

## Capabilities

- AEP use-case definition and architecture.
- XDM schema and dataset design.
- Identity, Profile, and merge-policy reviews.
- Audience and activation design.
- Sandbox audits and housekeeping.
- Dataflow health and launch hypercare.
- Governance and consent reviews.

Live AEP resources are resolved through the bundled MCP server. IKEA-specific resources and rules are never assumed when they cannot be verified.
