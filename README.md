# Ratio by Levr

<img src="icon.svg" width="72" alt="Ratio, the Levr owl">

**Ratio** is the trading companion of [Levr](https://levr.fi), the platform that runs crypto trading signals on your
own exchange accounts: it sizes each trade to your risk, places the stop on the exchange and takes profit at the
targets. Ratio brings that into Claude.

Ask it:

- *"Is this signal worth taking?"* (paste the call) — reward to each target from the planned entry and from the
  price now, how far price already ran, what past setups like it did, the chart checked against the trade, the
  economic calendar and the news.
- *"How are my trades?"* — your running Levr trades, live: R and USD now, distance to the stop and the next target.
- *"How did my week go?"* — win rate, average R, what worked and what didn't, by source, coin and setup.
- *"What's RSI?"* — trading words explained in plain language, with an example from your own trade.

Ratio **only reads**: it never places, changes or closes a trade, and it never sees your exchange keys.

## What's inside

- **The Ratio connector** (MCP, `https://app.levr.fi/mcp`): eleven read-only tools — check a signal, open and closed
  trades, performance, Ratio's brain (lessons from research and Levr users' closed trades, anonymous), technical
  analysis (on the plans that include it), the economic calendar and news, the market situation, a glossary.
- **The Ratio skill** (`skills/levr-ratio`): how Claude should use those tools — check a signal before any view,
  verdict first, the data over the textbook, never judge the analyst, news sets the size of a move, not its
  direction.

## Install

**Claude (web, desktop, mobile):** add it from the Claude directory, or go to
[app.levr.fi/ratio](https://app.levr.fi/ratio) and follow "Connect to Claude".

**Claude Code:**

```
/plugin marketplace add heyheyheyhe999/levr-ratio
/plugin install levr-ratio@levr
```

Then run `/mcp`, choose **ratio** and sign in.

You need a Levr account: [sign up at levr.fi](https://levr.fi). The first time, you sign in to Levr and approve
Ratio with your 2FA code.

## Privacy and terms

Ratio reads your Levr data only after you approve it, and only to answer you. See Levr's
[privacy policy](https://levr.fi/privacy.html) and [terms](https://levr.fi/terms.html).

Information, not financial advice. Trading crypto with leverage can lose more than you put in.

## License

The skill and these files: MIT. Levr and Ratio's service: © Levr.
