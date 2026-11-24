# SocialMCP skill

An agent skill for [SocialMCP](https://getsocialmcp.com): schedule and publish posts to X and LinkedIn from your AI agent, with one social media calendar.

The skill teaches your agent how to connect SocialMCP's hosted MCP server (`https://getsocialmcp.com/mcp`, OAuth sign-in) and how to use it well: check posts before they go out, write X threads and LinkedIn posts, use posting slots, and confirm the text and time with you before anything is published.

Works with OpenClaw, Hermes Agent and any agent that reads [Agent Skills](https://agentskills.io).

## Install

**Any agent** (with the open `skills` CLI):

<!-- commands:any_agent.skill -->
```bash
npx skills add mshahbazm/socialmcp-skill
```
<!-- /commands -->

**OpenClaw**

<!-- commands:openclaw.skill -->
```bash
openclaw skills install @mshahbazm/socialmcp --global
```
<!-- /commands -->

**Hermes Agent**

<!-- commands:hermes.skill -->
```bash
hermes skills install mshahbazm/socialmcp-skill/skills/socialmcp
```
<!-- /commands -->

## Connect SocialMCP

The skill walks your agent through this, but you can also do it yourself.

**OpenClaw**

<!-- commands:openclaw.connect -->
```bash
openclaw mcp add socialmcp --url https://getsocialmcp.com/mcp --transport streamable-http --auth oauth
openclaw mcp login socialmcp
```
<!-- /commands -->

**Hermes Agent**

<!-- commands:hermes.connect -->
```bash
hermes mcp add socialmcp --url https://getsocialmcp.com/mcp --auth oauth
hermes mcp login socialmcp
```
<!-- /commands -->

Your browser opens SocialMCP's sign-in page. Sign in and click **Allow**. You need a SocialMCP account ([start free](https://getsocialmcp.com/signup)) with your X account or LinkedIn profile connected. SocialMCP posts through the official X and LinkedIn APIs and never sees your passwords.

## What's inside

[`skills/socialmcp/SKILL.md`](skills/socialmcp/SKILL.md): connection steps for each agent, and how to post, schedule, edit and cancel with SocialMCP's tools.

## Support

- Docs: [getsocialmcp.com/docs/mcp](https://getsocialmcp.com/docs/mcp)
- Email: [hello@getsocialmcp.com](mailto:hello@getsocialmcp.com)

## License

[MIT](LICENSE)
