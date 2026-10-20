# Hey Nabu

The connector and the discipline for using it, in one plugin.

- `skills/hey-nabu/SKILL.md` — tells Claude to call `read_guide` and follow it. The
  connector serves the full skill there, as it has it today, so a change to it reaches
  you without a new version of this plugin. It also keeps four rules for when the call
  fails: search wide, cite what was found, say plainly what the sources do not cover,
  and never invent an organisation.
- `.mcp.json` — the server at `https://heynabu.ai/api/mcp`. It runs its own
  OAuth, so Claude sends you there to sign in and approve at first use and is given a
  token of its own. Nothing to paste.

The skill here is generated from `public/skill/plugin.md` in the app's repository. Do not
edit it here; edit it there and republish.

Installation, what the sources cover, and how to take a connection back:
[heynabu.ai/connect](https://heynabu.ai/connect).
