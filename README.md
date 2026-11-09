# Time Trakkr plugin

Connect your [Time Trakkr](https://timetrakkr.com) workspace to an AI client.
Ask about tracked time, budgets and profitability, log time, run timers, and
draft invoices, all under your own role in Time Trakkr.

This repository is the connector packaged in the open
[Agent Plugins](https://agent-plugins.org) format: `plugin.json` describes it
and `mcp.json` points at the Time Trakkr MCP server,
`https://timetrakkr.com/api/mcp`. It holds no code and no credentials.

## Install in Perplexity

Custom plugins need a paid Perplexity plan.

1. In Perplexity, open **Plugins → Add custom → Import plugin from GitHub**.
2. Paste `https://github.com/Time-Trakkr/time-trakkr-plugin`.
3. Open the Time Trakkr connector the plugin adds and sign in with your Time
   Trakkr account. Choose read-only, or read and write if you want to log time
   and draft invoices.

## What it will and will not do

- It reads and acts with your own permissions. Members never see rates or
  other money, and only owners and admins can draft invoices.
- Invoices are only ever drafted. Nothing is sent to a client; you review and
  send drafts yourself in Time Trakkr.
- It cannot delete time entries or change rates.

Disconnect at any time under **Integrations** in Time Trakkr.

## Other clients

Claude, ChatGPT, Gemini CLI, Cursor and others connect to the same server
directly. Setup for each is in the
[help article](https://timetrakkr.com/help/integrations/mcp-and-ai-clients).

For logging AI coding-agent sessions as time, see
[Time-Trakkr/agent-plugins](https://github.com/Time-Trakkr/agent-plugins).

## Support

https://timetrakkr.com/contact · hello@timetrakkr.com
