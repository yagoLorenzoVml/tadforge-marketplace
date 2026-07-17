# Tadforge Marketplace

Claude Code marketplace containing `tadforge`, a collection of Adobe Experience Platform skills for the IKEA account with a bundled remote MCP server.

## Install from GitHub

Add the marketplace using its GitHub `owner/repository` name:

```text
/plugin marketplace add <owner>/<repository>
/plugin install tadforge@tadforge
```

Run `/reload-plugins` if installing in an existing session. The plugin connects automatically to the bundled remote AEP MCP server. Use `/mcp` to review its connection or complete authentication if the server requests it.

## Test locally

From a Claude Code session, add this repository by absolute path:

```text
/plugin marketplace add <absolute-path-to-this-repository>
/plugin install tadforge@tadforge
```

The skills are namespaced under `tadforge`, for example:

```text
/tadforge:wppes-sandbox-audit
/tadforge:wppes-schema-design
/tadforge:wppes-client-context
```

## Migrate from the previous names

Remove the previous plugin and marketplace before installing Tadforge:

```text
/plugin uninstall manolo-agent@wppesmap
/plugin marketplace remove wppesmap
/plugin marketplace add <owner>/<repository>
/plugin install tadforge@tadforge
/reload-plugins
```

Open `/mcp` after reloading. The bundled server appears as `plugin:tadforge:aep`.

## Capabilities

- AEP use-case definition and architecture.
- XDM schema and dataset design.
- Identity, Profile, and merge-policy reviews.
- Audience and activation design.
- Sandbox audits and housekeeping.
- Dataflow health and launch hypercare.
- Governance and consent reviews.

Live AEP resources are resolved through the bundled MCP server. IKEA-specific resources and rules are never assumed when they cannot be verified.
