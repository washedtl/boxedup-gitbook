# SellerBoard — profit dashboard & reimbursements

🟡 **Intermediate.** SellerBoard is the answer to "how much did I actually make?" — a real-time profit dashboard that pulls from Seller Central and tells you the truth your gut can't.

## What SellerBoard does

Three things, exceptionally well:

1. **Real-time P&L** — every order, every fee, every refund, accurately attributed to the SKU that produced it. Live, not month-end.
2. **Per-SKU profitability** — finally see which SKUs make money and which ones bleed it. Most resellers are shocked by what they find.
3. **Automatic reimbursement detection** — finds lost / damaged / overcharged units that Amazon owes you for, and helps you file claims.

## Why it matters

Most resellers run on vibes. They look at deposits and feel rich. SellerBoard surfaces the inconvenient truths:

- That replen you love? It's actually losing \$1.50/unit after long-term storage.
- That "winner" SKU? It's a 4% margin, not the 20% you thought.
- That brand you ramped into? You're owed \$340 in lost-unit reimbursements right now.

Without SellerBoard (or InventoryLab — overlapping but different), you're flying blind past ~\$5K/mo revenue.

## The core dashboard

When you open SellerBoard, the top widgets show:

| Widget | What it tells you |
|---|---|
| **Today's profit** | Live P&L for orders that shipped today |
| **This month** | MTD revenue, fees, COGS, profit, ROI |
| **Best-selling products** | Top SKUs by profit, not revenue |
| **Worst products** | The ones bleeding cash — kill these |
| **Cash flow** | How much capital is tied up in inventory |
| **Reimbursements** | New cases SellerBoard found |

The "worst products" widget is the single most valuable view. Every month, look at the bottom 5 and decide: keep them (with a price increase), or remove and stop replenning.

## Setting up SellerBoard

The 30-minute setup that pays for itself:

1. **Sign up** at sellerboard.com — they offer a 1-month free trial
2. **Connect your Amazon MWS / SP-API** — read-only access, takes 2–3 minutes
3. **Wait 24 hours** — they need to ingest your historical data
4. **Enter your COGS** for each SKU — this is the painful part for old accounts. Use bulk CSV upload.
5. **Set your prep cost** — usually \$0.30–\$0.75/unit baseline
6. **Set your shipping-to-FBA cost** — average \$0.30–\$0.50/lb
7. **Verify the first few orders' profit math** matches your gut — if not, adjust costs

> **Tip:** if you already use **InventoryLab**, you can export COGS from IL and bulk-upload to SellerBoard. Saves hours.

## The reimbursement automation

This alone often pays for SellerBoard 5× over.

Amazon "loses" inventory all the time:
- Units lost in the warehouse
- Units damaged by Amazon (their fault, not yours)
- Customer returns Amazon never received but credited
- Weight/dimension miscalculations on FBA fees
- Orders refunded without the unit being returned

You're entitled to reimbursement for all of these. SellerBoard scans your reports and flags every case. You then submit through Seller Central's case manager (or use SellerBoard's filing helper).

**Typical recovery for a \$10K/mo seller: \$300–\$800/quarter.** For a \$50K/mo seller: \$1,500–\$5,000/quarter.

⚠️ **Window:** Amazon limits reimbursement claims to **18 months** from the event. Old issues you never filed are lost forever. Set up SellerBoard *before* you have a backlog.

## SellerBoard vs InventoryLab

They overlap. Many sellers use both. The honest comparison:

| Feature | SellerBoard | InventoryLab |
|---|---|---|
| Real-time P&L dashboard | ✅ Best-in-class | OK |
| Per-SKU profitability | ✅ Best-in-class | OK |
| Reimbursement automation | ✅ Excellent | Limited |
| Listing creation tool | ❌ No | ✅ Yes |
| Shipment building | ❌ No | ✅ Yes (Stratify) |
| Bookkeeping export | ✅ Good | ✅ Good |
| Price | \$15–\$50/mo | \$69/mo |

**The BoxedUp default setup:** InventoryLab for listing & shipment building, SellerBoard for P&L + reimbursements. The combo runs \$80/mo and replaces 3 hours/week of spreadsheet work.

## Daily / weekly / monthly cadence

Once it's set up, the discipline:

### Daily (60 seconds)
- Glance at "today's profit" — is it on track?
- Check for new reimbursement cases — file the easy ones (lost units, weight overcharges)

### Weekly (15 minutes)
- Open "worst products" widget — flag any SKU losing money for 2 weeks straight
- Review cash flow — are you over-leveraged in slow inventory?
- File any reimbursement cases that need supporting docs

### Monthly (45 minutes)
- Export P&L to your bookkeeping software
- Review per-brand profitability — any brand consistently bleeding? Drop it.
- Reconcile reimbursements actually paid vs filed
- Update COGS for any SKUs where supplier prices changed

## What SellerBoard won't tell you

Be clear-eyed about its blind spots:

- ❌ It can't tell you *which deal to source next* — that's [Keepa](keepa.md) + [SAS](sellerAmp.md)
- ❌ It doesn't account for **time spent sourcing** — the most valuable resource you have
- ❌ It uses *your* COGS — if you mis-enter, the math is wrong
- ❌ It doesn't predict price tanks — for that, watch Keepa

## When SellerBoard pays for itself

| Your monthly Amazon revenue | Will SellerBoard pay for itself? |
|---|---|
| < \$1K | No — too small to matter |
| \$1K–\$5K | Probably — reimbursements alone usually cover it |
| \$5K–\$25K | Definitely — P&L visibility is invaluable |
| \$25K+ | You should already have it |

If you're scaling and don't have it, **today is the day**.

***

Next: [Part 5 — Deal analysis →](../deal-analysis/profit-equation.md)

*Last updated: 2026-05-05*
