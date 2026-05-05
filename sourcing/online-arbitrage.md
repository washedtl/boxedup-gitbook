# OA — Online Arbitrage

🟡 **Intermediate.** Online arbitrage = sourcing inventory from online retailers (instead of physical stores) and reselling on Amazon. Most BoxedUp members graduate from RA to OA around month 3–6.

## Why OA wins over RA at scale

The math:

- **RA** = drive 90 min, scan 90 min in store, drive 30 min back. 4-hour day, find 5–10 winners. Cost: gas + time.
- **OA** = sit at desk, run KPF query, scan 200 ASINs in 60 min, find 10–20 winners. Cost: subscription tools + cashback rewards.

OA scales because:
- ✅ **No travel time** — your "store" is every retailer that ships
- ✅ **Cashback stacking** — 1–10% off purchases via Rakuten, TopCashback, Honey
- ✅ **Coupon stacking** — promo codes layer on cashback
- ✅ **Volume per hour** — 10× more SKUs analyzed per hour vs RA
- ✅ **Replenishability** — online retailers restock predictably; same SKU 10 weeks in a row

## Where to source OA

The retailers that actually produce profit:

### Tier S — high frequency winners
- **Walmart.com** — biggest source by volume; clearance + rollbacks daily
- **Target.com** — smaller volume but consistent clearance
- **Kohl's** — Kohl's Cash + sales create deep discounts
- **JCPenney** — frequent storewide promotions
- **Macy's** — sales + cashback can stack 30%+ off

### Tier A — niche but reliable
- **Home Depot, Lowes** — tools, seasonal, hardware
- **Best Buy** — open-box, daily deals
- **Ulta, Sephora** — beauty (gated category — verify ungating first)
- **Bath & Body Works** — Semi-Annual Sale = OA goldmine
- **The Children's Place, Old Navy, Gap** — apparel-arb
- **Wayfair** — furniture, home goods (oversize FBA risk)
- **Newegg** — electronics, components

### Tier B — opportunistic
- **Crate & Barrel, West Elm** — high-end, occasional clearance
- **Costco.com** — bulk-only (member-only, math rarely works)
- **Bed Bath & Beyond** (when alive) — closeouts
- **Hot Topic, BoxLunch** — niche pop culture

### Tier F — skip
- **Amazon itself** — that's A2A, different game (see [A2A page](a2a.md))
- **Most marketplaces** (eBay, Etsy) — no cashback, sketchy authenticity
- **Liquidation directly** (Liquidation.com) — pallet-only, see [liquidation](liquidation.md)

## The cashback stack

OA's secret weapon. On any retailer you source from:

### Step 1: Cashback portal
- **Rakuten** — most retailers, 1–10% back, payouts every 3 months
- **TopCashback** — sometimes higher rates than Rakuten, similar coverage
- **MrRebates / Swagbucks** — backup options

Compare rates before each purchase — they fluctuate.

### Step 2: Credit card rewards
- Amex Blue Business Cash: 2% back on everything
- Chase Ink Cash: 5% on office supplies, 2% on gas
- Co-branded cards (Target RedCard for Target, Kohl's Card for Kohl's) — often 5%
- Stack with cashback portal for ~7–12% combined back

### Step 3: Coupon codes
- **Honey** browser extension — auto-applies known codes at checkout
- **Capital One Shopping** — similar
- **Slickdeals** — manual search for niche codes
- Add to portal + card stack for 15%+ effective discount on some retailers

### Step 4: Retailer-specific
- **Walmart Wallet** — connect Walmart Pay for occasional bonus offers
- **Target Circle** — earn 1% in store credit
- **Kohl's Cash** — earned at checkout, redeemable on next purchase
- **Macy's Star Rewards** — points → coupons

A "good" OA buy is profitable BEFORE any of these stacks. Treat them as bonus margin, not the primary play.

## OA workflow

### Step 1: Surface candidates
Three sources:

**Source A: KPF Restock queries**
Run weekly (see [KPF deep dive](../tools/keepa-product-finder.md)) — outputs 100–500 ASIN candidates. Then check if they're available at any of the OA retailers above.

**Source B: Keepa Deals stream**
For A2A specifically — see [A2A page](a2a.md). Real-time mispricings.

**Source C: Discord deal-feed pings**
Members surface OA leads in real time. Act fast (see [deal feeds](../discord/deal-feeds.md)).

### Step 2: Validate

For each candidate ASIN:
1. Open SAS / scanner → get current Buy Box, fees, ROI at the retailer's price
2. Check Keepa chart — stable Buy Box? Few FBA sellers? Amazon out?
3. Check IP risk — Brand Registered? Aggressive enforcement?
4. Check gating — eligible for your account?

### Step 3: Source

Click through the retailer link and:
1. Apply coupon codes (Honey)
2. Activate cashback portal (Rakuten / TopCashback)
3. Use the right credit card (Amex Blue Business or co-branded card)
4. Submit reseller cert if you have tax-exempt status with the retailer
5. Place order

### Step 4: Receive + prep

Online orders arrive in 2–5 days. When they do:
1. Inspect for damage
2. FNSKU label per unit
3. Prep per category requirements
4. Build into next FBA shipment

### Step 5: List + sell

Inventory hits FBA, listing goes live, sells through.

## Cashback management

Cashback portals pay out 30–90 days after purchase. To track:

| Tool | What it tracks |
|---|---|
| Rakuten dashboard | Pending / earned cashback |
| TopCashback dashboard | Same |
| Spreadsheet | Cross-reference cashback vs orders |
| Tax software | Cashback is **not taxable income** in the US — it's purchase price reduction |

For tax purposes, treat cashback as:
- **NOT income** (you didn't earn it, you paid less for inventory)
- **Reduce COGS** by the cashback amount when calculating profit

## OA-specific risks

### Risk 1: Stockouts during transit
You ordered 50 units. By the time they ship, the deal expires and Amazon's price drops 20%. Your math no longer works.

**Mitigation:**
- Buy in smaller batches (10–20 units initially)
- Verify the listing is healthy before scaling buys
- Don't assume short-term price holds

### Risk 2: Counterfeit / wrong item
Online retailer ships the wrong item, or a non-authentic version. You ship to FBA and Amazon flags it.

**Mitigation:**
- Inspect every unit before shipping to FBA
- If something looks off, return to retailer
- Save invoice + product photos for IP defense

### Risk 3: Dropshipping detection
You order and ship-to-FBA without inspecting. Amazon detects "dropship" patterns (return labels showing the original retailer).

**Mitigation:**
- Always ship to YOUR address first, then to FBA
- Repackage if necessary (remove retailer-branded packaging)

### Risk 4: Account multi-buy detection
Some retailers limit "1 per customer" on hot SKUs. Sourcers create multiple accounts to bypass.

**Mitigation:**
- Stick to one account per retailer
- Use legitimate household members for "one more order" (with their consent)
- Don't stack 5+ accounts; retailers cancel the orders

## Hot OA categories

Categories that consistently produce OA wins:

### Toys
- Easter / Christmas / Halloween clearance (Tier 2 brands only — avoid Disney)
- LEGO with LEGO ungating (otherwise risky)
- Mid-tier toys at 30%+ off retail

### Beauty
- Drugstore brand clearance (Maybelline, L'Oreal lines)
- Specialty beauty closeouts (limited editions, discontinued shades)
- Requires Beauty category ungating

### Apparel
- End-of-season clearance from major retailers
- Style-specific inventory (out of trend)
- Avoid hot brands (Nike, Adidas) without invoices

### Home goods
- Kitchen utensils, small appliances, organizing
- Less brand-protected, easier source

### Books / Media
- Used book arbitrage (different game; specialized)
- Gaming / Pop Vinyl / collectibles (volatile)

### Avoid for OA
- Electronics (high-IP-risk, low-margin)
- Hazmat (shipping complications)
- Oversize (FBA fees eat OA margins)

## OA scaling pattern

By month-over-month volume:

| Month | OA orders/month | Tools you need |
|---|---|---|
| Month 1–3 | 5–20 | SAS only |
| Month 4–6 | 20–50 | SAS + Inventory Lab |
| Month 7–12 | 50–200 | + KPF + SellerBoard + Tempo |
| Year 2+ | 200–500 | + VA support, custom tools |

## When OA stops scaling

Above ~200 OA orders/month, you'll hit:
- Cashback caps (Rakuten limits per retailer per quarter)
- Per-retailer order limits (1 per customer)
- Inventory storage at home (boxes pile up)
- Time bottleneck on prep + shipping

Solutions:
- **Multiple retailers** — diversify sourcing across 10+ retailers, not 3
- **Prep service** — outsource prep + shipping (frees ~10 hrs/week)
- **Wholesale** — start replacing OA winners with wholesale equivalents (lower margin, infinite scale)

***

Next: [Wholesale →](wholesale.md)

*Last updated: 2026-05-05*
