# Using deal-feed channels effectively

🟡 **Intermediate.** Deal feeds are where the BoxedUp Discord earns its membership fee. But raw deal pings are noisy — filtering, reacting, and acting fast separates members who profit from members who get ratio'd by FOMO.

## The deal-feed mental model

Deal channels are **firehoses**, not curated lists. In an active server you might see:
- 5–30 A2A pings per hour during weekday business hours
- 2–10 restock pings per day
- 1–5 wholesale leads per week
- Occasional category-wide alerts (RAM shortage, new restriction, etc.)

You can't act on all of them. Discipline = "pick what fits MY operation, ignore the rest."

## The 60-second triage

For each ping, run through these in <60 seconds:

### 1. Is it in my categories / price band?
If you only sell Toys & Games, an Electronics deal is noise. Filter mentally.

### 2. Is the link still alive?
- Click the link → does the deal still exist? If sold out, scroll past.
- If price has already corrected, scroll past.

### 3. Does it scan profitable for me?
Open SAS / your scanner → run the numbers with **your costs** (your prep tier, your shipping, your ROI floor). What's profitable for someone with wholesale invoices may not be for you.

### 4. Can I actually buy it?
- Quantity limit? (Amazon often caps at 1, 2, 5)
- Gated? (See [gating](../anti-patterns/gating.md))
- Restricted to your account?

### 5. Is the listing safe?
- Check the brand's IP-claim history
- Check the offer-count trend (don't pile into a deal that's about to be cooked)
- Sanity-check the chart with [Keepa rules](../tools/keepa.md)

If all 5 pass, **act.** If not, scroll.

## Speed matters (sometimes)

For different deal types:

| Channel | Window | Action speed required |
|---|---|---|
| A2A pings | Hours, sometimes minutes | Buy within 5–15 min |
| Restock pings | Minutes to hours | Buy within 60–90 sec |
| Walmart in-store | Days (until store inventory clears) | Buy within 12–24 hrs |
| Wholesale leads | Days to weeks | Apply within a week |
| KPF queries | No urgency | Run on your schedule |

For restock pings, you're competing against bots and other members hitting refresh. Speed = winning.

For A2A and Walmart leads, deliberation > speed within reason. Better to do due diligence and pass than panic-buy a tank.

## The pile-on problem

When too many members hit the same deal, three things happen:
1. **Inventory runs out** before you can buy
2. **Listing offer-count spikes** (15 sellers within hours)
3. **Price tanks** as everyone undercuts each other to clear inventory

This is "the deal got cooked." Even if you bought, the math gets ugly.

How to avoid getting cooked:
- **Don't pile in 2 hours after the post** — by then it's already cooked
- **Watch the offer count in Keepa before buying**, not after
- **If 5+ FBA sellers added since the post, walk** — there's no Buy Box share for you
- **If price has already dropped 15% from when posted, walk**

## Reacting matters

When a member surfaces a deal that converts for you:

✅ React with the ✅ or 💰 emoji on the original post

This:
- Shows the source their lead worked
- Motivates them to post more
- Helps mods see which leads have high signal
- Builds your reputation as a contributor (not a leecher)

The best deal posters are responding to social signal. If their deals never get reactions, they stop posting. The whole feed gets worse.

## When to surface your own deals

Threshold for posting your own A2A or sourcing find:

- ✅ **You verified the math** (don't post a "deal" you didn't profit-test)
- ✅ **You bought your fill first** (don't post then race to buy more — selfish)
- ✅ **The deal has enough quantity** for others to act (no "I bought the last unit" posts)
- ✅ **Not from a paid group** (don't share leads from other paid services without permission)

When you post:
- ASIN + retailer + buy URL
- Your cost basis (RA receipt? OA + cashback?)
- Buy Box at time of posting
- Estimated ROI / margin
- Any caveats (gating, hazmat, oversize)

A high-signal post:
```
ASIN: B0XXXXX
Walmart: walmart.com/ip/...
$11.99 in store (also online)
Sell: $34.99 BB, 4 FBA sellers
ROI ~80%
Note: gated for some accounts, scan first
Got mine — go!
```

A low-signal post:
```
walmart deal lol $34
```

Don't be the second guy.

## The quiet days

Active members notice deal flow varies:
- **Mondays**: high (Amazon restock, weekend store-floor leads)
- **Tue–Thu**: steady
- **Friday afternoon**: drops (everyone exits early)
- **Saturday**: low (deal posters touching grass)
- **Sunday**: rebuilds (people prepping for the week)

Don't expect Monday-density on Saturday. The lull is normal.

## The signal-vs-noise rule

After 30 days in deal feeds, calibrate:

- **High-signal members**: their leads convert often → enable mobile push for their posts
- **Low-signal members**: their "deals" miss often → mute or filter
- **Bot-pings (Tempo, Blaze)**: enable push for the channels but **disable global notifications** (you'll burn out)

A common Discord configuration:
- 🔔 **Mention-only** for general channels
- 🔔 **All messages** for `#a2a-feed`, `#restock-monitors` (active hours only)
- 🔕 **Muted** for status channels and `#general` (check on your own time)

Set notifications by channel, not server-wide. Otherwise you'll be a slave to the buzz.

## Dispelling FOMO

If you've been here a month and feel like you're missing every deal, you're not. The reality:

- Most deals **don't end up profitable for most members**
- The people screenshotting big wins also took losses you didn't see
- Pile-ons are real — being late is often safer than being first
- The **best returns come from your own KPF queries + replens**, not chasing pings

Treat the deal feed as **opportunity surface area**, not the main game. The main game is your own discipline.

***

Next: [Bots & commands cheat sheet →](bots.md)

*Last updated: 2026-05-05*
