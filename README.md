# Simple Hack for Claude

Run, join, or judge a hackathon on [simple-hack.app](https://simple-hack.app/) from Claude. Participants describe their idea, and Claude builds and publishes their team's website, so the people competing do not need to write code. Organisers set up the event, judges score against the organiser's rubric, and results go out from the same place.

This plugin bundles five skills and the Simple Hack connector (`https://simple-hack.app/mcp`). The first time Claude needs the connector, a Simple Hack sign-in window opens: sign in with Google or an emailed code, then choose Allow. The plugin asks for no API keys, team keys, or passwords, and it reads nothing from your computer. Each call runs with the signed-in person's own role in each event.

## Skills

- `run-hackathon`: for organisers. Create an event, set registration questions and tracks, publish the public page, manage teams and judging, post announcements, and publish results.
- `join-hackathon`: for participants. Join an event, form or join a team, pick a track, fill in the entry, vote, and see results.
- `judge-hackathon`: for judges. Read the rubric and the queue, score entries, comment, and flag conflicts.
- `website-deploy-builder`: plans a team site or a custom event website, including what it stores and who can read it.
- `website-deploy`: builds and publishes that site with the team's or organiser's scoped access.

## What people use it for

- A university society runs a weekend hackathon for 120 students. The organiser asks Claude to create the event, add an AI track and a social impact track, and open registration on Friday.
- A product team runs an internal innovation day. A product manager on one team says "build our site: an app that matches volunteers to shifts", and Claude publishes it at the team's address before entries close.
- A panel of three judges each work through their assigned entries in Claude, scoring against the rubric and leaving comments the organiser reviews before publishing results.

## Install in Claude Code

```
/plugin marketplace add vineetu/simple-hack-plugin
/plugin install simple-hack@simple-hack-marketplace
```

In the Claude apps without plugins, add the connector instead: open [Claude connectors](https://claude.ai/new?modal=add-custom-connector#customize/connectors/yours), name it Simple Hack, paste `https://simple-hack.app/mcp`, and choose Add.

## Privacy and support

The connector sends tool arguments to simple-hack.app and returns event, team, judging, and site data only within the signed-in person's permissions. Privacy policy: https://simple-hack.app/privacy.html. Terms: https://simple-hack.app/terms.html. Support: support@simple-host.app.

## Source

Generated from [github.com/vineetu/simple-host](https://github.com/vineetu/simple-host) (`hack-toolkit/`). Please open issues there.

MIT licensed. Website: https://simple-hack.app/
