# Controlflare

**A hard monthly billing cap for Cloudflare Workers.** Set a spend limit; when your
estimated month-to-date spend crosses it, Controlflare pauses your Workers, before
the invoice does the talking. You resume things yourself, when you are ready.

The estimate covers Workers, D1, R2, KV and Durable Object requests, priced at
Cloudflare's published rates.

- 🌐 **Website:** [controlflare.com](https://controlflare.com)
- 📊 **Dashboard:** [app.controlflare.com](https://app.controlflare.com)
- 🤖 **For AI agents:** [controlflare.com/agents](https://controlflare.com/agents/), a remote
  MCP server over Streamable HTTP with twelve tools. Four of them stop production
  traffic, so read that part first.

## Repositories

**[controlflare-cost-agent](https://github.com/Controlflare/controlflare-cost-agent)**
is an open-source Worker you deploy into *your own* Cloudflare account, so your API
token never leaves it. Controlflare talks to the agent; the agent talks to Cloudflare.
Small enough to read before you deploy it.

**[claude-marketplace](https://github.com/Controlflare/claude-marketplace)** is the
Claude Code plugin. It contains no code: three JSON files pointing at the hosted MCP
server, so there is nothing to run locally and no key to paste.

```
/plugin marketplace add Controlflare/claude-marketplace
/plugin install controlflare@controlflare
```

> Controlflare is an independent tool, not affiliated with Cloudflare. Spend is an
> **estimate** from Cloudflare's usage analytics and published prices, not your
> invoice. See the [disclaimer](https://controlflare.com/disclaimer/).
