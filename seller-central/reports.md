# Reports you should run weekly

🟡 **Intermediate.** Amazon's Reports section is data-rich but UI-poor. Most sellers ignore it. The ones who don't get pattern recognition that beats algorithmic sourcing.

## The 7 reports that matter

Most BoxedUp resellers should run these regularly:

### 1. Inventory Performance Report
**Path:** Inventory → Inventory Performance → Inventory Performance Index

**Why:** shows your IPI score + sub-metrics. The single most important page for capacity planning.

**Cadence:** weekly (Monday)

**What to act on:**
- IPI dropping → see [IPI deep dive](../fba/ipi.md) for recovery
- Excess inventory list → drop prices or remove
- Stranded inventory → fix listings or remove
- Sell-through rate → identify slow movers

### 2. Aged Inventory Report
**Path:** Reports → Fulfillment → Aged Inventory Surcharge

**Why:** shows inventory age brackets. Catches items entering the 271-day surcharge zone before LTSF hits.

**Cadence:** weekly (Monday)

**What to act on:**
- 181–270 days: drop price 15%
- 271–365 days: drop price 30% or remove
- 365+ days: dispose immediately (LTSF compounds)

### 3. Inventory Reconciliation Report
**Path:** Reports → Fulfillment → Reconciliation → Inventory Adjustments

**Why:** shows units lost, damaged, miscounted by Amazon. **Source of reimbursement claims.**

**Cadence:** weekly (Friday with reimbursement claims)

**What to act on:**
- "Damaged - Warehouse" entries → file reimbursement
- Negative adjustments without reason → investigate, file claim
- Pattern of issues at one warehouse → escalate

### 4. Sales Report (Detail Page Sales and Traffic)
**Path:** Reports → Business Reports → Detail Page Sales and Traffic

**Why:** sales velocity + Buy Box win rate per ASIN. Identifies which SKUs are working.

**Cadence:** weekly (Sunday review for upcoming week planning)

**What to act on:**
- Buy Box <70% on any SKU → investigate competition + pricing
- Sessions but no sales → conversion problem (price? listing?)
- Top SKUs by units: focus replen orders here

### 5. Returns Report
**Path:** Reports → Fulfillment → Returns

**Why:** which SKUs return at high rates? Why?

**Cadence:** monthly

**What to act on:**
- High-return SKUs (>10%): evaluate listing accuracy or stop sourcing
- Customer-cited reasons: pattern signals (sizing, quality, descriptions)
- Returns marked "Customer Damaged - Refund" — sometimes reimbursable

### 6. Reimbursement Report
**Path:** Reports → Payments → Reimbursements

**Why:** track money Amazon owed you and paid back.

**Cadence:** weekly (Friday with reconciliation)

**What to act on:**
- Reimbursement % of revenue: should be 0.5–2%
- If trending down: you're missing claims
- If specific issues recur: address process

### 7. Performance Notifications
**Path:** Performance → Notifications

**Why:** Amazon's direct flags about issues — IP claims, warnings, restrictions.

**Cadence:** check daily; address within 24 hours

**What to act on:**
- IP complaints: file POA
- Performance warnings: corrective action
- Listing suppressions: investigate + fix

## Underused but powerful reports

### Search Term Report (for sellers with own listings)
**Path:** Reports → Advertising Reports → Search Term Report (or similar)

**Why:** see what customers search for to find your listings.

For arbitrage sellers, less useful (you don't control listings). For PL sellers, essential.

### Order Reports
**Path:** Reports → Fulfillment → Order Reports

**Why:** export all orders + customer info + ship-to addresses. Useful for:
- Bulk customer messaging
- Geographic sales analysis
- Deep historical analysis

### Inbound Performance Report
**Path:** Reports → Fulfillment → Inbound Performance Dashboard

**Why:** how reliable are your shipments? Errors per shipment. Quality grade by warehouse.

For sellers with high inbound volume, this catches systemic issues.

### Buy Box Percentage Report
**Path:** Reports → Business Reports → Detail Page Sales and Traffic → Filter by ASIN

**Why:** which SKUs win Buy Box; which lose.

For each SKU below 70% Buy Box: investigate why, fix.

## Setting up reporting habits

### Monday morning (15 min)
- IPI dashboard
- Aged Inventory
- Sales + Buy Box review

### Friday afternoon (20 min)
- Inventory Reconciliation → file reimbursements
- Reimbursement Report → confirm prior week's payouts
- Performance Notifications → address any new issues

### Monthly (45 min)
- Returns Report → identify problem SKUs
- Order Reports → quarterly review of sales patterns
- P&L from SellerBoard or InventoryLab

### Quarterly (90 min)
- Cross-channel analysis (RA vs OA vs Wholesale profitability)
- Brand-level analysis (which brands are working)
- Category-level analysis (where to expand or contract)
- Competitor analysis (storefront tracking results)

## Connecting reports to action

The point of reporting isn't to "have the data" — it's to drive decisions.

### Sample decision tree from data

```
This week's reports show:
├─ IPI: 620 (was 680 last week)
├─ Aged inventory: 12 SKUs entering 271-day bracket
├─ Top 10 SKUs: still selling well
├─ Returns: 1 SKU at 18% return rate
└─ Reimbursement: $340 found this week

Actions this week:
1. Drop price 15% on 12 aged SKUs (rescue from surcharge)
2. Stop replen on 18%-return SKU (kill the bleeding)
3. File 3 reimbursement cases (claim the $340)
4. Reorder top 5 SKUs (proven winners, ride the velocity)
```

Without reports → you'd miss IPI decline, miss the surcharge cliff, replen a bad SKU, leave reimbursements unclaimed.

## Tools that aggregate reports

For deeper analysis than native Amazon UI:

### SellerBoard
- Imports all data
- Cleaner P&L visualization
- Auto-flags reimbursement opportunities
- ~\$15–\$50/month

### InventoryLab
- Same data + listing/shipping integration
- ~\$69/month

### Scout / Helium 10 / Jungle Scout
- Sales-tracking on competitors (storefront stalking)
- Useful for sourcing intelligence
- ~\$50–\$200/month

### Custom dashboards
- Some sellers export Amazon reports → Google Sheets / Power BI
- Free (your time)
- Best for advanced analytics

For most BoxedUp members: SellerBoard + Amazon native reports cover 95% of needs.

## Pattern recognition from reports

After 6 months of weekly review, patterns emerge:

### Sales pattern observation 1: Day-of-week
Sales by day are NOT uniform. Common patterns:
- Monday: highest (post-weekend cart-abandonment fulfillment)
- Sunday: low (people cooking instead of buying)
- Friday afternoon: dip
- Black Friday-week: 5–10× normal

Plan inventory + cash flow accordingly.

### Sales pattern observation 2: Seasonal
- Q4 spike: 1.5–3× normal
- Post-Christmas dip: 2 weeks of slow
- January spike (gift cards being spent): real
- Spring + summer ramp depending on category

### Sales pattern observation 3: Buy Box seasonality
Some SKUs have stable Buy Box year-round; others have constant churn.

For replens: prefer stable Buy Box patterns. For one-time A2A: timing matters less.

### Sales pattern observation 4: Competition cycles
Some SKUs see new sellers enter every 60–90 days as deal-feed groups discover them. Plan inventory commitments around expected dilution.

## What doesn't belong in reports

Things you won't find on Amazon's reports:

### True cost basis
Amazon doesn't know your buy cost. You enter it via Inventory Lab / SellerBoard. Without that, "profit" reports are garbage.

### Cashback/rebate adjustments
Net cost = retail - cashback - coupons. Amazon doesn't know any of that. Manual or via your tracking tool.

### Time investment
Hours you spent sourcing, prepping, shipping. Track separately to compute true hourly rate.

### External revenue
Sales on eBay, Mercari, Walmart Marketplace. Not in Amazon's reports.

For the full picture, blend Amazon reports + SellerBoard + your own tracking.

***

This concludes Part 6 — Seller Central operations. Next: [Part 7 — Business & tax setup →](../business-setup/entity.md)

*Last updated: 2026-05-05*
