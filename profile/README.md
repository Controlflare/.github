# Controlflare

**A hard monthly billing cap for Cloudflare Workers.** Set a spend limit; when your
estimated month-to-date Workers spend crosses it, Controlflare pauses your Workers —
before the invoice does the talking. You resume things yourself, when you're ready.

- 🌐 **Website:** [controlflare.whirlwin.io](https://controlflare.whirlwin.io)
- 📊 **Dashboard:** [app.controlflare.whirlwin.io](https://app.controlflare.whirlwin.io)
- 🛡️ **[controlflare-cost-agent](https://github.com/Controlflare/controlflare-cost-agent)** —
  an open-source Worker you deploy into *your own* Cloudflare account so your API token
  never leaves it. Controlflare talks to the agent; the agent talks to Cloudflare.
  Small enough to read before you deploy it.

> Controlflare is an independent tool, not affiliated with Cloudflare.
