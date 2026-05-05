# The reseller's mental model

Before you scan a single product, internalize this. It's the difference between people who quit in 90 days and people who run six-figure businesses.

## You are not a "seller." You are an arbitrageur.

Amazon resellers don't *make* products — we move them from where they're underpriced to where they're overpriced, and we get paid for the friction we remove. Your job has three parts:

1. **Find mispriced inventory** (sourcing)
2. **Move it through Amazon's pipes** (FBA prep + shipping)
3. **Survive the platform's rules** (account health, IP, gating)

Everything in this guide maps to one of those three.

## The core belief — the data does not lie

> **Keepa discovers. The news confirms. Speed is the edge.**

The BoxedUp methodology is built on a single belief: **the Keepa chart tells the full story.** Social media, news, and industry reports are useful for confirming the *why* behind a signal — but the *discovery* of the opportunity always starts in the data.

The order is always the same:

1. **Spot the signal in Keepa** (offer count patterns, OOS trends, price behavior)
2. **Confirm the *why* through external research** (Twitter, Reddit, industry news)
3. **Act before the broader market catches up**
4. **Never use emotion. Never guess. Only data and logic.**

This is not a feelings business. It's a data business. By the time it's news, the margin is gone.

## The two strategies

Every profitable BoxedUp flip is one of two distinct plays. **Never confuse them — different sourcing logic, different buying timing, completely different risk profile.**

### A2A — Amazon-to-Amazon (pricing anomaly)

You buy an item **from Amazon** at a price that's temporarily lower than its historical norm, then **resell it on Amazon** when the price corrects back up.

- The key word is **anomaly**
- You're not buying because it's cheap — you're buying because the current price is a **statistically unusual deviation** from what the market considers normal
- Surfaced via **Keepa Deals** (real-time)
- Window: hours to a day or two
- The bet: mean reversion

### Restock/Monitor (availability scarcity)

You identify items that Amazon **historically stocked** but is **currently OOS on**, then set up monitors to catch the moment Amazon restocks. You buy the second supply appears and sell at the elevated 3P market price.

- The key word is **scarcity**
- You're not buying because the price is low — you're buying because the item is **hard to get** and demand exceeds supply
- Surfaced via **KPF (Keepa Product Finder)** + monitor infrastructure (Tempo, Blaze)
- Window: weeks to months
- The bet: when Amazon restocks at historical retail, you ride 3P pricing back up

### The test to know which one applies

Ask: *"Is this item profitable because the **price is lower than normal**, or because it's **hard to get**?"*

- Lower than normal → **A2A**
- Hard to get → **Restock/Monitor**

A2A requires the item to be readily available. Restock requires the item to be scarce. The sourcing logic, buying timing, and risk profile are completely different. **Never conflate them.**

## The four levers of profit

Whichever strategy you're running, every flip lives or dies on these four numbers.

| Lever | What it controls | Where you find it |
|---|---|---|
| **Buy cost** | What you pay (Amazon for A2A, retailer for Restock) | Receipt / order confirmation |
| **Sell price** | The 3P Buy Box on Amazon | Keepa, SAS |
| **Amazon fees** | Referral % + FBA pick/pack + storage | SAS, FBA Revenue Calculator |
| **Velocity** | How fast it sells (units/month) | Keepa BSR drops, monthly sold |

The first three give you **profit per unit**. The fourth gives you **profit per month.**

## ROI vs Margin vs Cash velocity

Three different ways to measure "is this a good flip." Not the same.

```
ROI    = profit / cost           (return on invested cash)
Margin = profit / sell_price     (% of revenue you keep)
Velocity = units sold / month    (how fast cash recycles)
```

> **The BoxedUp rule of thumb (when there's no special signal):**
> - **ROI ≥ 30%** for RA, ≥ 20% for OA, ≥ 15% for wholesale
> - **Sales rank** in the top 1% of category (or velocity ≥ 5/mo)
> - **No more than 3 FBA sellers** on the listing besides you
>
> **The exception:** during a confirmed shortage / Restock play, these floors can move dramatically. A 5% margin per unit on a 1000-unit-per-month-restocking SKU with 0 FBA sellers can be the best play of the year.

## What "no rank ≠ no sales" means

**Counterintuitive but critical.** Items without a current BSR can be among the fastest-selling items on Amazon. When a SKU goes deeply OOS across all sellers simultaneously, Amazon's ranking algorithm has no current sales data to work with — so the rank disappears. **The buyers haven't disappeared. The supply has.**

Five signals that work when BSR is absent or suppressed:

1. **Offer count drops** — each drop = a seller ran out, which means buyers were buying
2. **Offer count fluctuation patterns** — rapid up-and-down cycling = high turnover
3. **Subcategory rank** — top-level may be suppressed but subcategory often visible
4. **Monthly Sold data** (yellow-gold line) — Amazon's own demand estimate
5. **"Bought in past month" badge** on the product page

What NOT to use: **review count growth.** OOS items can't accumulate reviews when there's no inventory to sell. Absence of review growth on a scarce item tells you nothing.

Full framework: [Reading a Keepa chart like a pro](../tools/keepa.md#reading-velocity-without-a-bsr).

## The five things that will kill your account

This is the survival list. Memorize it.

1. **Inauthentic complaints** — selling something Amazon thinks is fake
2. **IP / trademark complaints** — brand owner files against you
3. **Used sold as new** — opened, damaged, or returned items relisted
4. **Late shipment / cancellation rate** (only matters for FBM)
5. **Counterfeit traps** — sourcing from sketchy liquidation lots

[Anti-patterns](../anti-patterns/ip-complaints.md) is built around avoiding these. Read it before you scale.

## What this business actually feels like

Honest things, so you know what you're signing up for:

- **The first 90 days are mostly losing money** while you learn what's gated, what's a trap, and how to read Keepa.
- **Most products are not profitable.** You'll scan 100 items and find 2 worth buying. That's normal.
- **Fees eat 30–40% of revenue.** Plan for it.
- **Cash flow is the boss.** You can be "profitable" and still go broke if your cash is locked in slow-moving inventory. Velocity matters more than ROI past a certain scale.
- **Amazon will randomly suspend you for things you didn't do.** It happens to everyone eventually.
- **The discovery happens during routine work.** The biggest wins (like the [RAM shortage call](../tools/the-ram-shortage-case-study.md)) come from doing the reps every week, not from special hunts.

## Core principles

The rules the methodology lives by:

### On data
- The chart does not lie. Learn to read it and trust it.
- Social media confirms. Keepa discovers. Always in that order.
- Don't use emotion. Don't guess. Use supply-and-demand logic.
- Don't hound on metrics that don't apply to your item type. Match your signals to what you're evaluating.

### On sourcing
- **You make money when you buy** — sourcing discipline matters more than selling tactics.
- If you stick too strictly to the book (must have BSR, must have reviews, etc.) you miss the most profitable items.
- A no-rank item selling 500 units a month is more profitable than a ranked item selling 10.
- The infrastructure has to be in place BEFORE the window opens.

### On competition
- **Low offer count when you catch a restock = you own the listing.**
- Being the only FBA seller on a 200/month item is more valuable than being one of 50 sellers on a 5000/month item.
- Offer count collapse is your opportunity signal.

### On the business
- Community fast-tracks success. BoxedUp exists because everyone finds more together.
- Build a Found Profit List — track every profitable item you ever identify. Patterns emerge.
- Profit, not revenue. Always.
- When you want to quit, don't.

## What this guide will not do

- It won't make you rich in 30 days.
- It won't replace experience — you have to do reps.
- It won't cover dropshipping (we don't), FBM exclusively (we mostly don't), or selling on other marketplaces.

What it *will* do is compress the 18 months of expensive mistakes most resellers make into a few weeks of reading.

***

Next: [Glossary →](glossary.md)
