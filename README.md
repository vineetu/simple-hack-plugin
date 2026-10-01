# Simple Hack for Claude

Run a hackathon on [simple-hack.app](https://simple-hack.app/). The bundled `run-hackathon` skill guides hosted event setup, team sites, judging, results, and an optional private instance. The `.mcp.json` connector points to the hosted Simple Hack MCP server. Sign in through Claude's connection flow and choose **Manage my events** for organiser work; a participant connects to their team separately for site publishing.

The organiser connection exposes ten tools to list events, check a name, create and read a draft, update page settings and stages, read or replace a rubric, and export judging scores or results. The connector sends tool arguments to `simple-hack.app`; event, team, judge and site data is returned only within the account and role's permissions. A team connection can publish only its selected team's site. Self-hosted setup in the skill may call the chosen cloud provider and DNS provider using the organiser's credentials.

The package contains no credentials. Support is [support@simple-host.app](mailto:support@simple-host.app). The new P1 workflows are prepared in this skill and await platform deployment verification. This public source is a Claude Code marketplace, not an Anthropic directory listing; no directory submission or approval is claimed.

## Install from a public source

Add the public source as a Claude Code marketplace, then install the plugin:

```text
/plugin marketplace add vineetu/simple-hack-plugin
/plugin install simple-hack@simple-hack-marketplace
```

The connection requires sign-in to Simple Hack; choose **Manage my events** for organiser work. P1 browser and API workflows in the skill require the matching platform release. The marketplace source is [vineetu/simple-hack-plugin](https://github.com/vineetu/simple-hack-plugin); it has not been submitted to or approved by the Anthropic directory.

Source: the maintained `simple-host-website/skills/run-hackathon/` skill and `hack-toolkit/metadata/` in the Simple Host repository. Regenerate from those files for each release. The ten organiser MCP tools are unchanged.
