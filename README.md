# Hey Nabu

Ask Claude about the field of impact and get an answer you can check.

Each expert has read one field — regenerative wealth, systems change, ocean
regeneration, bioregions, AI innovation. It knows the organisations doing the work,
who funds them, and what the research says. It keeps reading as new work appears.
Every answer links back to where it came from.

This repository is a Claude plugin marketplace holding one plugin. It carries two
things: the connector to [heynabu.ai](https://heynabu.ai), and a skill that teaches
Claude how to read the experts — search every one before narrowing, cite what it
found, name what the sources do not cover, and never invent an organisation. The
skill is short: it tells Claude to fetch the full version from the connector, so
what Claude is taught stays current between versions of this plugin.

## Install

**In claude.ai or the desktop app.** Add the connector first, from
[heynabu.ai/connect](https://heynabu.ai/connect). Its button opens Claude with the
connector filled in. Then go to Customize → Plugins → Add → Add marketplace, give it
`heynabu/hey-nabu-plugin`, and add **Hey Nabu**. A plugin never adds its own
connector, so this order matters: added first, the connector shows as Connected on
the plugin's page. Plugins are on Pro, Max, Team and Enterprise.

**On a Team or Enterprise plan.** Most members cannot add a connector or a plugin
themselves. The Owner adds both for everyone from
[heynabu.ai/team](https://heynabu.ai/team): the connector, then the plugin as a zip,
set to *Installed by default*. An organisation cannot add this repository itself,
because Claude syncs only private ones. Each member then connects Hey Nabu under
Customize → Connectors.

**In Claude Code.**

```bash
claude plugin marketplace add heynabu/hey-nabu-plugin
claude plugin install hey-nabu@hey-nabu
```

Either way, Claude sends you to sign in at Hey Nabu and approve. It is then given a
token of its own that reads exactly what you read, for an hour at a time, renewing
itself until you take it back on the site's **Add Nabu to your AI** page. Nothing to paste.

The connector works without the plugin. The plugin adds the skill, which is the only
way to get it into a chat.

You need an account. Each expert is built for the organisation it was commissioned by,
and some are open to everyone.

## What it can do

Ask it about the field and it searches every expert you can read, not the one you
named. An expert knows the organisations working in its field, who funds them, and what
the research says. It also reads what those organisations publish, so it can tell you
what changed this week. Every story has a summary written for it and a link to the
publication.

It reads. It cannot publish, delete or edit anything. It writes only notes to the
editors: a gap it found in the sources, or a change you asked for. A note changes
nothing anyone can read until an editor acts on it. It does not give financial, legal or tax advice, and it will route you to named
organisations and documents rather than answering thinly from the nearest source.

## What is in it

| | |
|---|---|
| `hey-nabu/skills/hey-nabu/SKILL.md` | Tells Claude to read the current skill from the connector |
| `hey-nabu/.mcp.json` | The connector — one HTTP server, OAuth at first use |

The full skill is served two ways: by the connector's `read_guide` tool, which is what
this plugin's skill calls, and at [heynabu.ai/skill/SKILL.md](https://heynabu.ai/skill/SKILL.md),
open without signing in so anybody can read it first. Both are the one copy the app
keeps, and a test holds it to the server's actual tools: it names every one and invents
none. So a change to the skill reaches every Claude that reads it from the connector the day it ships, with
no new version of this plugin. The plugin's own short skill changes rarely; refresh it
with `claude plugin marketplace update hey-nabu`.

## Support

[heynabu.ai/connect](https://heynabu.ai/connect) is where tokens are
made and revoked, and where a connection is taken back.
