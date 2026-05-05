# SellerAmp SAS deep dive

🟢 → 🟡 — SellerAmp SAS is the most-used scanning tool in the BoxedUp community. This page goes beyond the setup basics into the specific features that separate beginner-grade scanning from pro-level sourcing.

## What SAS shows you (full breakdown)

When you scan a product, SAS pulls live data and displays:

### The header
- ✅ **Eligibility status** — "You can sell" / "Approval required" / "Restricted"
- 🚨 **Brand IP risk indicator** — green / yellow / red
- 📊 **Sales rank** — current + 30/90/180 day averages
- 💵 **Buy Box price** — current

### The fees breakdown
- **Referral fee** — %, calculated from category
- **FBA fee** — pick/pack based on size + weight tier
- **Storage fee estimate** — pro-rated monthly
- **Inbound placement fee** — varies by your shipping plan
- **Returns reserve** — 5% default

### The ROI calculator
- Input your **Buy Cost** (with cashback adjustments)
- Input **Prep Cost** (default \$0.30–\$0.75)
- Input **Inbound Shipping** (default \$0.30–\$0.50/lb)
- See **Net profit per unit**, **ROI%**, **Margin%**

### The Keepa chart
- 90-day default view
- Switch to 1-year, 2-year, all-time
- Toggle: Buy Box, Amazon, New, Used, FBA, FBM, Sales rank

### Offer details
- **FBA seller count** — how many FBA-fulfilled offers
- **FBM seller count** — how many merchant-fulfilled
- **Amazon presence** — is Amazon currently selling?
- **Lowest FBA / FBM** — minimum prices

### Variation handling
- If the listing has variations (sizes, colors), SAS shows:
  - Which variation matches your scanned UPC
  - That specific variation's BSR + Buy Box
  - All variations on the listing for context

## Configuring SAS for your strategy

The default settings work for general arbitrage. For specialized strategies, tune:

### For RA (high-volume scanning)
- **ROI threshold:** 30%
- **Profit floor:** \$3
- **Max FBA sellers:** 5
- **Show only:** "Eligible" items
- **Fast-scan mode** ON (less data per scan, more scans per minute)

### For OA (online research)
- **ROI threshold:** 20%
- **Profit floor:** \$3
- **Max FBA sellers:** 5
- **Detailed Keepa chart:** ON
- **Show variations panel:** ON

### For Restock/Monitor strategy
- **AMAZON_OOS:** ON as a key metric
- **Brand exclusion list:** loaded with your Tier 1 + Tier 2 brands to avoid
- **Show offer count history chart:** ON

### For wholesale scouting
- **ROI threshold:** 15%
- **Profit floor:** \$5
- **Max FBA sellers:** 8
- **Stable Buy Box requirement** flag enabled

## The Buy Cost field — getting it right

The single most-misused field. If you input wrong, ROI math is wrong.

### What to include
- ✅ Retail price you'll pay
- ✅ Sales tax (if you don't have a reseller cert)
- ✅ Subtract cashback from portals (Rakuten, etc.)
- ✅ Subtract coupon discounts

### What NOT to include
- ❌ Shipping to your home (that's separate; SAS includes inbound shipping)
- ❌ Time spent shopping (that's labor, separate concern)
- ❌ Returns reserve (SAS adds this automatically)

A worked example for OA on a \$30 retail item:
```
Retail price:           $30.00
Sales tax (skip if cert): $0.00
Coupon (10%):           -$3.00
Cashback (5% Rakuten):  -$1.35
Net Buy Cost:            $25.65
```

Input **\$25.65** in SAS, not \$30.

## Multi-pack / variation gotchas

Common mistake: scanning a multi-pack but SAS shows single-pack data.

How to avoid:
1. Always scan the actual UPC on your specific unit
2. Verify SAS's "matched ASIN" matches the listing you intend to sell on
3. Check the variation panel — confirm the BSR / Buy Box match

If SAS picks the wrong variation:
- Tap "View on Amazon" to manually navigate to the right variation
- Re-scan from that listing

## The brand IP risk feature

SAS's brand IP risk indicator pulls from databases of:
- Recent IP complaints
- Brand Registry status
- Hijacker frequency

| Color | Meaning |
|---|---|
| 🟢 Green | Low risk — no recent complaints, not Brand Registered |
| 🟡 Yellow | Moderate — Brand Registered, occasional complaints |
| 🔴 Red | High — frequent complaints + active enforcement |

**Red flags = walk.** Even if the math works, the suspension risk isn't worth it.

## SAS + Keepa integration

SAS pulls Keepa data via your API key. To configure:

1. Keepa.com → Account → API Access → Generate API key
2. SAS Settings → Keepa → paste API key
3. Refresh — Keepa charts now appear inline

Without Keepa connection, SAS shows limited data. With Keepa connected:
- Full price history
- BSR drops counter
- Offer count history
- Sales velocity estimate (Keepa's monthly sold)

## Storefront tracking

SAS lets you "track" specific sellers — when they list new ASINs, you get notified.

How to use:
1. Open a listing of a competing FBA seller you respect
2. Click their seller name → SAS shows their storefront
3. Click "Track Storefront" — adds them to your watchlist
4. Daily / weekly digest of their new ASINs appears in SAS

This is the "follow the money" technique — successful sellers source good SKUs, you piggyback on their research.

⚠️ **Don't blindly copy.** Verify each ASIN with your own analysis. Just because they're listing doesn't mean it's profitable for you.

## Notes feature

SAS lets you add notes to ASINs:
- "Walmart in-store \$8.99 — receipt 4/15"
- "Replenishable from Target — restocks Mondays"
- "Don't reorder — price tanked May 2025"

Notes save context across multiple scans. After 200+ ASINs, you'll thank yourself for taking notes.

## Bulk export

SAS allows CSV export of scanned ASINs:
- Date scanned
- ASIN, UPC, title
- Buy Box, BSR, ROI calc
- Your input cost
- Decision (bought / passed)

Export weekly to a master spreadsheet. Cross-reference with sales data later to identify patterns.

## Mobile vs desktop

SAS works on both, with different strengths:

### Mobile (in-store / on-the-go)
- Camera scan UPC barcode
- Full data display
- One-tap decisions
- Best for RA + quick OA checks

### Desktop (deep research)
- Click into Keepa charts
- Multi-tab comparisons
- Storefront analysis
- CSV exports

Use both as needed. Many BoxedUp members keep desktop SAS open during sourcing sessions while phone scans new finds.

## Common SAS errors and fixes

### Error: "Could not find a match"

The UPC you scanned isn't on Amazon. Either:
- The product isn't sold on Amazon (skip)
- The UPC encoding is wrong (try scanning a different barcode on the package)
- Amazon's catalog is missing this UPC (rare; not your problem)

### Error: "Not eligible to sell"

Either:
- Brand is gated for you (apply for ungating)
- Category is restricted (apply for category)
- Account has a temporary restriction (check Account Health)

### Error: "Buy Box: $0.00"

Means there's no current Buy Box offer. Reasons:
- All sellers are out of stock
- Listing has been suppressed
- Pricing rules conflicted

In any case: don't source. Wait for normal Buy Box to return.

### Error: "Could not load Keepa data"

API rate limit hit, or Keepa is down. Retry in 5 minutes.

## Tips for power users

### Batch scanning workflow
For sourcing 50 SKUs from a CSV:
1. Open SAS desktop
2. Paste UPC list into "Bulk lookup" feature
3. Set auto-fetch all data
4. Wait 60–90 seconds for SAS to scan all
5. Review filtered results sorted by ROI

### Pricing alerts
Save ASINs you sourced. SAS can alert you when:
- Buy Box drops below your floor
- Offer count spikes (potential pile-on)
- Amazon comes back in stock

Set alerts on your top 50 SKUs. React when triggered.

### Replen confirmation
For replens, scan the source store's UPC weekly:
- Is the store price still the same?
- Is Amazon's Buy Box still the same?
- Do margins still hold?

If any drift: investigate. If math still works: reorder.

## SAS alternatives

For comparison:

| Tool | Pros | Cons |
|---|---|---|
| **BuyBotPro** | Auto-evaluates "buy/skip" | Less manual control |
| **ScanPower** | Older, established | Less polished UI |
| **AMZ Analyzer** | Free | Fewer features |
| **Native Amazon Seller App** | Free | Only basic data |

SAS strikes the best balance for most BoxedUp members. Stick with it unless you have a specific reason to switch.

***

Next: [InventoryLab for accounting & prep →](inventory-lab.md)

*Last updated: 2026-05-05*
