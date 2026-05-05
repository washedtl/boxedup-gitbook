# Bots & commands cheat sheet

🟡 **Intermediate.** The BoxedUp Discord runs several bots that automate sourcing, monitoring, and community functions. Quick reference for the commands you'll use most.

> **Note:** The exact bots and command syntax can drift. If a command in this cheat sheet doesn't work, check `#bot-status` or `!help` in `#bot-commands`.

## Tempo (restock monitor)

The primary restock monitor across multiple retailers.

### Add monitors

```
!m add [retailer] sku1 sku2 sku3 ...
```

All SKUs go on **one line**. Whitespace separates them.

### Examples

```
!m add amazonus B081XWLQKS B0C79S2CHW B07ZPLM1R1
!m add walmart 12345678 87654321
!m add bestbuy 6483193 6543210
!m add target A-89473123
```

### Remove monitors

```
!m remove [retailer] sku
```

### List your monitors

```
!m list
```

### Supported retailers (typical list)
- `amazonus` — Amazon US
- `amazonca` — Amazon Canada
- `walmart` — Walmart.com
- `bestbuy` — Best Buy
- `target` — Target
- `newegg` — Newegg
- `bhphoto` — B&H Photo
- `homedepot` — Home Depot
- `lowes` — Lowes

For a current list, run `!m help`.

### Tips
- **Don't dump 200 ASINs in one command** — break into batches of 20–50
- **Prune dead monitors weekly** to avoid notification fatigue
- **Set channel-specific notification levels** so you only get pinged for high-priority retailers

For full Tempo workflow, see [Restock monitoring](../sourcing/restock-monitoring.md).

## Blaze (secondary monitor)

Different scraping engine, useful for redundancy. Setup is API-driven, not command-line.

To enroll an ASIN in Blaze:
1. Open `#bot-commands`
2. Use the Blaze setup form (linked from server's pinned messages)
3. Submit your monitor list
4. Receive pings in the channel where you submitted

Blaze typically wakes up faster than Tempo for some retailers but slower for others. Running both = best coverage.

## Server utility bots

### MEE6 / Carl-bot (moderation)

Standard Discord moderation bot. Handles:
- Auto-roles based on reactions in `#welcome`
- Tier upgrades when payments process
- Anti-spam, anti-link enforcement

You generally interact with this bot via reactions, not commands.

### YAGPDB / similar

Sometimes used for:
- Self-assignable roles (notification preferences, region, sourcing focus)
- Polls and voting
- Scheduled messages

Check `#welcome` for the role-assignment instructions.

## Custom BoxedUp bots

Servers often have custom bots for specific functions:

### Deal-feed bot
Some servers parse external deal sources and pipe them into channels automatically. You don't command it — it auto-posts.

### Wholesale-lead bot
Curated, gated content distribution. Often locked to higher-tier roles. You can't trigger; the bot pushes leads when verified.

### Webhook bot (Discord webhooks)
Most BoxedUp tooling (BoxedUp CC, FlipAlert, custom scripts) post to Discord via webhooks. You don't see the webhook URL — but mods do.

If you write your own tooling and want to post to a Discord channel, ask mods for a webhook URL. They typically provision a private channel for your personal feed (e.g., `#my-leads-yourname`).

## Self-help via bots

### Server search
Discord's native search is your first stop. `Ctrl+F` (Discord) → search keywords like "ungating" or "Tempo" before asking. Most beginner questions have been asked.

### `?help` / `!help` / `/help`
Prefix varies by bot. Try each — one will surface a help message with available commands.

### `?ping` / `!ping`
Test if a bot is alive. If it doesn't respond, the bot is down — check `#bot-status` before assuming you typed wrong.

## Bot etiquette

### Don't spam commands in public channels
Always run bot commands in `#bot-commands` (or whatever your server's bot channel is). Running `!m add` in `#general` clutters everyone's view.

### Don't trigger every bot to test
"Let me see what each bot does" floods channels. Read the channel pins, then test in `#bot-commands` only.

### Report bot issues, don't argue with them
If Tempo missed a restock, post in `#tool-bug-reports` with:
- Date/time of expected ping
- ASIN
- Retailer
- Whether you saw the restock yourself

Don't DM the bot maintainer demanding fixes. They're a volunteer or paid staff who's already aware.

## When bots break

Bots go down. Common causes:
- **Retailer site changes** — Walmart updates their HTML, scrapers break
- **API rate limits** — too many users hitting the bot at once
- **Discord outage** — sometimes the issue is Discord, not the bot
- **Hosting issues** — VPS reboots, SSL cert expirations

When a bot is down:
1. Check `#bot-status` for known outages
2. If no announcement, post in `#tool-bug-reports`
3. Have a fallback: manually monitor your top SKUs while bots recover

For high-stakes monitors (top replens, hot restocks), don't rely on a single bot. Run Tempo + Blaze + your own watching. Redundancy = uptime.

## Pinging the right bot for the right thing

Quick reference:

| Need | Bot |
|---|---|
| Add restock monitor | Tempo (`!m add`) |
| Backup restock monitor | Blaze |
| Get role / upgrade access | MEE6 / Carl-bot reaction |
| Find an old message | Discord native search |
| Test if a bot is alive | `?ping` / `!ping` |
| Set up custom webhook for personal tooling | DM mods |

## What's not a bot but feels like one

A few server features that look bot-like:

- **Pinned posts** — manually maintained by mods. Read them; they have the canonical guides for the server.
- **Channel descriptions** — also mod-set. Quick reference for what the channel is for.
- **Stickied messages** — auto-posted templates in onboarding channels.

Treat these as documentation, not bot output. They're maintained, just not via commands.

***

Next: [Discord etiquette →](etiquette.md)

*Last updated: 2026-05-05*
