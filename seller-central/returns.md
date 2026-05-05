# Returns & FBA inbound problems

🟡 **Intermediate.** Returns happen — the questions are how you minimize them, how Amazon handles them, and how to recover the value when they happen. Inbound problems are different beasts but share the "small stuff that drains margin" pattern.

## How returns work for FBA

When a customer returns an FBA order, Amazon handles it:

1. Customer initiates return via "Your Orders"
2. Amazon emails return label
3. Customer ships back to FBA warehouse
4. Amazon receives + grades the unit:
   - **Sellable** — back to your inventory
   - **Customer damaged** — usually back to your inventory at "Used" condition (varies by category)
   - **Carrier damaged** — Amazon usually pays you (reimbursement)
   - **Defective from new** — varies; sometimes back, sometimes you eat
   - **Lost in return shipping** — Amazon refunded customer; you may be reimbursed

Most returns: 7–14 days from customer initiating to inventory updated.

## Return rates by category

Approximate return rates BoxedUp members typically see:

| Category | Return rate |
|---|---|
| Books | 1–3% |
| Toys | 3–8% |
| Home goods | 4–10% |
| Beauty | 5–15% |
| Apparel | 15–30% |
| Electronics | 8–15% |
| Health/personal care | 8–18% |

**Apparel is the killer** — high return rates eat margin. Most BoxedUp members avoid apparel for this reason.

## What Amazon does with returns

Three outcomes:

### Outcome 1: Returned to your inventory as "New"
The unit was barely opened or unopened. Amazon adds it back to your sellable inventory.

**Reality:** Amazon's grading is sometimes generous. A "new" return might actually be lightly used. Customer of your future sale may complain.

### Outcome 2: Returned to your inventory as "Used - Like New" (or other Used grade)
Amazon grades down. The unit goes back as a different SKU, sells at lower price.

**Reality:** lower margin per unit. Sometimes worth selling, sometimes worth disposal/removal.

### Outcome 3: Disposed by Amazon
Unit deemed unsellable. Amazon disposes; you eat the loss.

**Reality:** sometimes you're owed reimbursement (carrier damage, Amazon damage). File case if applicable.

## Return-related reimbursements

You're entitled to reimbursement when:

### Customer return refunded but never received
Customer initiated return, got refunded, but Amazon never received the return shipment. After 60 days, you can claim.

### Return processed but unit not added back to inventory
Tracking shows the package arrived at FBA, but your inventory count didn't update. After 30 days, you can claim.

### Return damaged in carrier transit (not customer fault)
Amazon's tracking shows damage from FedEx/UPS. You're owed value of the unit.

### Return processed under wrong SKU
Amazon mis-categorized the return. Inventory adjustment required.

For all of these: see [Reimbursements](reimbursements.md). Tools like SellerBoard auto-flag eligible cases.

## Reducing return rates

Five tactics:

### Tactic 1: Accurate listings
- Listing photos match unit
- Description includes specific dimensions, materials
- "What's in the box" listed clearly

For arbitrage: don't change listings (the brand owns them) but be aware which listings have inflated promises.

### Tactic 2: Quality prep
- Verify each unit pre-shipping
- Reject damaged units
- Don't ship "looks fine, probably works"

### Tactic 3: Avoid high-return categories
- Apparel (sizing, fit, fabric texture)
- High-cost electronics (buyer's remorse)
- Hyper-specific niche items (functional disappointment)

### Tactic 4: Source from quality channels
- Retail returns + liquidation = higher return rates downstream
- Wholesale + new = lower return rates

### Tactic 5: Customer expectation management
- For listings you control, write descriptions that prevent surprises
- Conservative claims + over-delivery > inflated claims + under-delivery

## Returns processing optimization

When returns hit your inventory:

### Returned as "New" — sellable
- Inventory automatically rejoins sale flow
- No action required
- BUT: monitor for customer complaints on subsequent sales (they may complain about "used as new")

### Returned as "Used - Like New"
- Different SKU, lower price
- Decide: sell as Used or remove?
- Selling as Used: typical 50–70% of New price
- Removing: \$0.97 cost (small std), recover unit for resale elsewhere

### Returned but never shipped back
- Customer never returned the package
- Amazon may eventually reimburse you (after 60 days)
- File reimbursement case

### Returned damaged
- Inspect via photos in Manage Inventory → Returns
- Submit reimbursement claim if Amazon's responsibility
- If your responsibility (e.g., you sold a damaged unit), accept the loss

## FBA inbound problems

Different beast: problems that arise during shipping inventory IN to FBA.

### Inbound problem 1: Lost in receiving
You shipped 100 units; Amazon received 87. Where are the other 13?

**Action:**
- Wait 10–14 days for receiving to complete
- Check Reports → Reconcile (Inventory Reconciliation)
- Submit shipment-level reimbursement claim with shipment ID + actual count

### Inbound problem 2: Carrier damage
UPS damaged a box in transit. Some units inside are unusable.

**Action:**
- File claim with the carrier (UPS, FedEx) for the damaged units
- Amazon Partnered Carrier shipments: Amazon often handles claim for you
- Manual carrier shipments: file directly with carrier

### Inbound problem 3: Stuck shipment
Shipment status "Receiving" for >10 days with no progress.

**Action:**
- Open case: Help → Inbound Shipment Problem
- Provide tracking number, shipment ID
- Often gets manual escalation, expedites within 3–5 days

### Inbound problem 4: Wrong contents counted
Amazon checked in 50 units of SKU A, but you actually shipped 50 units of SKU B (mis-labeled).

**Action:**
- Check FNSKU labels first — your fault?
- If mis-labeled, request relabeling (Amazon charges \$0.30/unit)
- If Amazon's mis-count, submit claim

### Inbound problem 5: Mixed up boxes
Two of your shipments collide; contents mixed.

**Action:**
- Submit help case with both shipment IDs
- Provide expected vs actual contents per box
- Amazon's reconciliation team manually fixes (slow, 2–4 weeks)

## Removal orders for returns / inventory cleanup

Returned-as-Used inventory you don't want to sell as Used:

1. Inventory → Manage Inventory
2. Filter "Condition: Used" or filter by SKU
3. Action → Create Removal Order
4. Choose:
   - **Return to address** (~\$0.97 std) — get unit back
   - **Disposal** (~\$0.30 std) — Amazon destroys

For aggressive IPI cleanup: dispose. For value recovery on valuable items: return.

## Removal-as-flip strategy

Some BoxedUp members use returns to recover hot inventory during stockout periods.

The play:
- Hot SKU is often OOS
- You have stranded "Used" returns for that SKU
- Remove → photograph as "open box" → resell elsewhere (eBay, Facebook, your own site)

Margins can be 50%+ of new price for "open box" items. Disclose condition honestly.

## What prevents inbound problems

Discipline at shipping:

### Discipline 1: Photograph every box before sealing
Protects you on damage claims, quantity disputes.

### Discipline 2: Weigh + measure boxes accurately
Prevents oversize charges, wrong-bin assignments.

### Discipline 3: Use Amazon Partnered Carrier
Amazon's UPS rates are 30–50% cheaper, and Amazon handles damage claims for you.

### Discipline 4: Print 2D barcode labels
Faster receiving, fewer mis-counts. See [Third-party tools](../seller-account/third-party-tools.md).

### Discipline 5: Submit shipping plans accurately
Don't lie about contents to test ASINs. Amazon detects inconsistencies and flags accounts.

## When to escalate

Most inbound problems resolve via case-filing within 2–4 weeks. Escalate if:

- 30+ days without resolution
- High dollar value (>\$1,000 of disputed inventory)
- Pattern of issues with same warehouse (rare; can flag systemic problem)

Escalation paths:
1. Reply to existing case requesting "tier 2 escalation"
2. New case to "Account Health" referencing the original
3. Last resort: Twitter/X public post tagging Amazon's seller-support handle (sometimes faster than tickets)

## Tracking returns + inbound

Make a habit of monthly review:

### Monthly inventory audit
- Compare your shipped quantity vs Amazon's received
- Identify any unreconciled gaps
- File claims on gaps >5 units

### Monthly return analysis
- Which SKUs return at high rates?
- Which SKUs come back damaged most?
- Adjust sourcing to avoid problem SKUs

### Quarterly process audit
- Are damage rates trending up?
- Are inbound problems concentrated in one carrier?
- Adjust shipping practices accordingly

***

Next: [Pricing automations & rules →](pricing.md)

*Last updated: 2026-05-05*
