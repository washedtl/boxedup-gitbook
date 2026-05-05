# Reimbursements: lost, damaged, weight

🔴 **Highest dollar leverage in the entire guide.** Most BoxedUp resellers leave \$500–\$5,000 per quarter on the table by not actively chasing reimbursements. This page shows you what's owed and how to claim it.

## The premise

Amazon's FBA system makes mistakes:

- They lose units in transit between warehouses
- They damage units during storage
- They credit customer returns the unit never came back for
- They miscalculate weight/dimensions and overcharge fees
- They fulfill orders from your stock and never reconcile the inventory

By Amazon's own policy, **you're entitled to be reimbursed for all of this.** But Amazon doesn't proactively pay — they wait for you to ask.

## How much is at stake

Quick math from BoxedUp Discord's averages:

| Monthly revenue | Typical reimbursement claim per quarter |
|---|---|
| \$2K–\$5K | \$80–\$200 |
| \$5K–\$15K | \$200–\$700 |
| \$15K–\$50K | \$700–\$3,000 |
| \$50K+ | \$3,000–\$15,000 |

This is **money you're already owed** — not new sales. Pure margin recovery.

## The 8 reimbursement categories

### 1. Lost in warehouse / lost in transit

Inventory that was checked into FBA, then disappeared. Amazon's tracking system flags it. You file → they reimburse at your average sale price (or replacement cost).

**Where to find:** Reports → Fulfillment → Inventory Adjustments → filter for negative adjustments.

### 2. Damaged in warehouse

Items damaged by Amazon staff or in storage. Amazon flags as "Customer Damage" or "Warehouse Damage." Warehouse damage = you're owed.

**Where to find:** Reports → Fulfillment → Inventory Ledger → filter "Damaged - Warehouse."

### 3. Customer return never received

Customer returns refunded by Amazon, but the return package never arrived back at FBA. After 60 days, you can claim.

**Where to find:** Reports → Fulfillment → Returns → filter "Refund issued, no return."

### 4. Customer return damaged beyond resale

Customer returned the item, Amazon couldn't resell it (graded "Defective" or "Customer Damaged"). Sometimes you're owed reimbursement for these.

**Where to find:** Returns dashboard → "Sellable status: Unsellable."

### 5. Order fulfilled but never deducted from inventory

Amazon shipped a unit to a customer but never marked it as shipped in your inventory. Tricky to find — usually surfaces via discrepancies between sales reports and inventory ledger.

### 6. Weight/dimension overcharges

Amazon's measurement system misclassifies your unit's size or weight, charging you a higher FBA tier than warranted. Common with:
- Newly listed ASINs (never re-measured)
- Listings where Amazon's measurements differ from yours
- Oversize units near the std/oversize threshold

**Where to find:** Reports → Payments → Transaction view → filter for unusually high FBA fees on a specific ASIN.

### 7. Inbound shipment discrepancies

You shipped 100 units; Amazon received 98. The 2-unit discrepancy can be:
- Lost in receiving (you're owed reimbursement)
- Mis-counted (no reimbursement, just inventory adjustment)
- Stolen (you're owed reimbursement)

**Where to find:** Reports → Fulfillment → Reconcile → ship plan reconciliation reports.

### 8. Return reimbursement reversal

Customer returned an item, you got reimbursed, then 30 days later Amazon reversed the reimbursement and reclaimed the credit. This is a known Amazon bug — file a case and they often re-reimburse.

## How to claim

Two paths:

### Manual case-by-case (good for small sellers)

1. Identify the discrepancy in a report
2. Open Help → Get support → Selling on Amazon → Fulfillment by Amazon
3. Provide:
   - Order ID or shipment ID
   - SKU + ASIN
   - Quantity affected
   - Date of incident
   - Specific request: "Please reimburse me for [N] units of [SKU] [reason]"
4. Wait 24–72 hours for Amazon to investigate
5. Receive reimbursement (or denial — you can re-file if denied)

Time per claim: 5–15 minutes. Worth it if you're filing fewer than ~30/month.

### Reimbursement automation tools (essential at scale)

Above ~\$5K/month revenue, manual case-filing isn't tractable. Use a tool:

- **SellerBoard** — best all-around, ~\$15–\$50/mo, includes reimbursement automation. See [SellerBoard page](../tools/sellerboard.md).
- **Refunds Manager** — specialized in reimbursements, ~\$50–\$200/mo
- **Helium 10 Refund Genie** — bundled with Helium 10
- **GETIDA** — performance-based pricing (you only pay if they recover), often best for low-volume sellers

The tools work by:
1. Pulling your full Amazon report data via API
2. Identifying every potential reimbursement case
3. Auto-filing claims (or queueing them for your one-click approval)
4. Tracking which got paid and which got denied

Time saved: 90%+. Recovery rate: typically 1.5–3× higher than manual filing.

## The 18-month window

⚠️ **Critical**: Amazon's policy limits reimbursement claims to **18 months** from the event. Older issues are lost forever.

If you've been selling for 6+ months without filing claims:
- Sign up for SellerBoard or GETIDA today
- They'll backfile every eligible historical case
- Expect a 4-figure recovery in the first 30 days

This is found money. Don't skip it.

## What Amazon will deny

Not every claim wins. Common denial reasons:

- **Customer-fault damage** — if Amazon flags damage as customer-caused, you're not owed
- **Stickerless / commingled inventory** — Amazon won't reimburse for inventory you can't identify as yours
- **Outside the 18-month window**
- **Insufficient evidence** — no order ID, no SKU specifics
- **Already reimbursed** — Amazon proactively reimbursed and you're double-claiming

When denied, you can:
1. **Re-file** — sometimes a different rep approves what the first one denied
2. **Escalate** — request a higher-tier rep
3. **Walk** — if it's small dollars, accept and move on

## Reimbursement income statement line

For tax purposes, treat reimbursement income as **other income** (not gross sales). It's not a refund, not a sale — it's compensation from Amazon for losses.

In your bookkeeping (InventoryLab, SellerBoard, QuickBooks), categorize as:
- **Account:** "FBA Reimbursements" or similar
- **Category:** Other Operating Income

Total it monthly and compare to total revenue. Healthy reseller ratios:
- Reimbursements as % of revenue: 0.5%–2%
- If <0.3%, you're under-claiming
- If >3%, something's wrong (high damage rate, inventory accounting issue)

## Cadence

A workflow that scales:

### Weekly (15 min)
- Open reimbursement-tool dashboard
- Approve auto-filed cases
- Submit any "needs evidence" cases (look up order IDs)

### Monthly (60 min)
- Reconcile reimbursements paid vs claimed
- Identify denied claims worth re-filing
- Review category-level inventory loss rates (is one warehouse worse than another?)

### Quarterly (2 hours)
- Audit historical reports for claims missed
- Review reimbursement % of revenue trend
- Submit any backfile cases for SKUs that need extra documentation

## A note on ethics

Reimbursements aren't a "scam" — Amazon's policy promises reimbursement and you're holding them to their word. There's no shadiness to claiming what you're owed.

Some sellers feel weird about asking. Don't. Amazon's automation is designed to under-pay unless you ask. **Asking is the system working as intended.**

***

Next: [Customer messages & A-to-Z claims →](customer-messages.md)

*Last updated: 2026-05-05*
