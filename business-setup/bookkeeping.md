# Bookkeeping & inventory accounting (FIFO)

🟡 **Intermediate.** Bookkeeping isn't optional. It's how you know if you're actually making money. Most BoxedUp resellers think they're profitable; their books reveal otherwise. This page shows the system that actually works.

## Why bookkeeping matters

Five reasons:

### Reason 1: Tax compliance
You need accurate records for tax filing. Sloppy books = audit risk + back taxes.

### Reason 2: Real profit visibility
Your gut feel of profit is wrong. Almost always. Books tell the truth.

### Reason 3: Decision-making
Should you reorder? Source more category X? Drop SKU Y? Books answer these.

### Reason 4: Loan / financing capability
Want a line of credit at 5% to scale inventory? Need 12 months of clean books.

### Reason 5: Selling the business
Some resellers exit by selling their Amazon account (allowed by Amazon under specific conditions). Buyer wants 12+ months of audited books.

## The system stack

For most BoxedUp resellers:

```
Layer 1: Bank account (Mercury or similar)
   ↓
Layer 2: Sourcing tracker (InventoryLab) — per-SKU COGS
   ↓
Layer 3: P&L tool (SellerBoard) — sales + reimbursements
   ↓
Layer 4: General ledger (QuickBooks Online or similar) — combined view
   ↓
Layer 5: CPA — annual review + filing
```

You don't need all layers from day 1. Add as you scale.

## Day 1 setup

If you're just starting:

### Step 1: Separate bank account (Mercury)
All business income → here. All business expenses → here. NEVER personal use.

### Step 2: InventoryLab (or 2D Workflow + spreadsheet)
Track per-SKU costs as you ship to FBA.

### Step 3: SellerBoard
Pull sales data + auto-flag reimbursement opportunities.

### Step 4: Spreadsheet for general expenses
For non-COGS operating expenses (software, mileage, supplies). Keep simple.

Total cost: ~\$80/month. Total time: 30 min/week to maintain.

## Inventory accounting (FIFO)

Critical for tax compliance.

### What FIFO means
"First In, First Out" — sold inventory uses cost of oldest acquired inventory.

### Why FIFO over alternatives
- **Standard** — IRS-accepted, most common for ecommerce
- **Predictable** — easy to calculate
- **Software-supported** — InventoryLab and similar tools default to FIFO

Alternatives (LIFO, Specific Identification, Weighted Average) have niche use cases but aren't worth complexity for typical resellers.

### FIFO worked example

You bought:
- 100 units at \$5 each in January (\$500 total)
- 100 units at \$7 each in March (\$700 total)
- 100 units at \$9 each in May (\$900 total)

Total inventory: 300 units, \$2,100 invested

In June, you sold 250 units at \$15 each.

FIFO COGS calculation:
```
First 100 sold: cost = $5 each = $500 (Jan inventory)
Next 100 sold:  cost = $7 each = $700 (Mar inventory)
Next 50 sold:   cost = $9 each = $450 (50 of May inventory)
Total COGS:     $1,650 for 250 units sold
```

Remaining inventory: 50 units × \$9 = \$450 still on books.

Revenue from sale: 250 × \$15 = \$3,750
Gross profit: \$3,750 - \$1,650 = \$2,100

After fees + operating expenses, that becomes your net profit for tax purposes.

## What InventoryLab does for you

Manual FIFO tracking gets painful >50 SKUs. InventoryLab (IL):

- Tracks every unit's cost basis
- Allocates to sales using FIFO automatically
- Adds inbound shipping + prep costs to landed cost
- Reports per-SKU profit using accurate COGS

Once set up, you don't think about FIFO — IL does the math.

## Per-unit landed cost calculation

Your true cost of goods isn't just the retail price. It includes:

```
Buy cost (retail price minus cashback - coupons) ......... $10.00
+ Inbound shipping (your cost to FBA, prorated per unit) .. $0.40
+ Prep cost (per-unit allocation of supplies + time) ...... $0.50
+ Misc per-unit (returns reserve, etc.) ................... $0.20
─────
Total landed cost per unit ................................ $11.10
```

This is your TRUE cost basis for tax + profit purposes. Beginners forget the second three lines and overestimate profit by 5–10%.

## Categorizing transactions

Standard categories for a reseller's chart of accounts:

### Revenue
- Amazon Sales — Marketplace
- Amazon Sales — Shipping
- Amazon Sales — Promotional Rebates
- eBay Sales (if applicable)
- Other Marketplace Sales
- FBA Reimbursements (separate income line)
- Other Income (interest, etc.)

### Cost of Goods Sold (COGS)
- Inventory Purchases
- Inbound Freight
- Prep Supplies
- Returns Adjustments

### Operating Expenses
- Software Subscriptions (Inventory Lab, Keepa, etc.)
- Office Supplies
- Internet & Phone (business %)
- Travel & Mileage (sourcing)
- Bank Fees
- Credit Card Processing Fees
- Professional Fees (CPA, lawyer)
- Education
- Marketing & Advertising
- Insurance

### Owner Distributions / Draw
- Funds you take out for personal use

### Tax Payments
- Federal estimated tax
- State estimated tax
- Sales tax remitted (if applicable)

## Weekly bookkeeping discipline

A rhythm that works:

### Monday morning (10 min)
- Review last week's bank transactions
- Categorize new transactions in your bookkeeping tool
- Flag any "unsure" transactions for review with CPA

### Friday afternoon (15 min)
- Reconcile bank balance vs bookkeeping balance
- Mismatch >\$10? Investigate before week ends.
- Update mileage log (if applicable)

### Monthly close (30–60 min)
- Run P&L for the month
- Compare to target (e.g., 25% net margin)
- Identify variance drivers
- Send P&L to CPA (if monthly basis) or save for quarterly

### Quarterly (60–90 min)
- Estimated tax payment (if profitable)
- Per-SKU profit deep-dive
- Per-channel ROI analysis (RA vs OA vs wholesale)
- Adjust pricing / sourcing strategy based on data

## Reading a P&L

Sample monthly P&L for a \$15K/month reseller:

```
Revenue:                            
  Amazon Sales                       $14,200
  Reimbursements                       $300
  Other                                $500
  Total Revenue                     $15,000

Cost of Goods Sold:
  Inventory Purchases                $6,000
  Inbound Freight                      $300
  Prep Supplies                        $150
  Total COGS                         $6,450

Gross Profit:                        $8,550 (57%)

Operating Expenses:
  Software (IL, Keepa, SAS, etc.)      $200
  Mileage (sourcing trips)             $400
  Internet/Phone (business %)           $50
  CPA fees                             $250
  Bank fees                             $20
  Other                                 $80
  Total Operating Expenses           $1,000

Net Operating Income:                $7,550 (50%)

Other:
  Sales tax (informational)               $0
  Owner draw                         $5,000

Retained earnings:                   $2,550
```

This seller is healthy: 57% gross margin, 50% net operating margin, retaining 17% for reinvestment.

## Cash flow vs profit

Two different things:

### Profit (P&L)
What you've made on paper. Include accrued sales (Amazon will pay 14 days after sale).

### Cash flow
What's actually in your bank.

You can be **profitable but cash-strapped:** sales accruing but not yet deposited; inventory bought but not yet sold; tax payments due.

Track both:
- **Profit** via P&L weekly
- **Cash flow** via bank balance + 14-day projection

Conservative: keep 30 days of operating expenses + 60 days of sourcing budget in cash.

## Common bookkeeping mistakes

### Mistake 1: Mixing personal + business
You bought lunch with the business card. Business owes Lunch \$15.
Or: you bought a personal item with business funds. Personal owes Business \$50.

**Fix:** strict separation. If you slip up, immediately reverse via owner draw or contribution.

### Mistake 2: Ignoring small expenses
"\$3 here, \$5 there — too small to track." Over a year, these total to \$1,000+ unrecorded.

**Fix:** track everything. Modern tools auto-import transactions. No excuse.

### Mistake 3: Forgetting cashback
You bought \$1,000 of inventory, got \$50 cashback. You marked the \$1,000 as COGS. The \$50 is income? Cost reduction? Both?

**Fix:** **cashback reduces COGS** (it's not income). Mark it as a credit in your inventory purchase line, reducing the net cost.

### Mistake 4: Late COGS entry
You shipped inventory in March but didn't enter cost in IL until June. By then, you've forgotten the actual cost.

**Fix:** enter cost the day you ship. Or use auto-pull from purchase records.

### Mistake 5: Not closing the books
Months go by without final close. You don't know if you're profitable. Tax filing becomes panicked guessing.

**Fix:** monthly close. Even if rough. Discipline > perfection.

## When to hire a bookkeeper

Triggers:
- You spend >5 hours/week on bookkeeping
- Past \$25K/month revenue
- You have employees / VAs (payroll)
- You hate bookkeeping (procrastination = errors)
- Multiple business entities

Cost: \$200–\$1,000/month for monthly bookkeeping.

Find via:
- Discord recommendations
- Reseller-specific firms: Bookskeep, AccountingProse
- Local accountants who serve Amazon sellers

## Year-end ritual

Critical December actions:

### Reconcile inventory
- Physical count of inventory at home + reconcile to FBA report
- Adjust books if discrepancies > 5%

### Maximize legitimate deductions
- Pay annual subscriptions (vs monthly) for software you use
- Purchase business equipment if needed (reseller-specific)
- Make charitable donations (if charitable contributions are tax-strategy relevant)

### Estimated tax payment
- Final Q4 quarterly tax payment due January 15
- Calculate based on Q4 P&L

### Send to CPA
- Final P&L, balance sheet, supporting docs to CPA early January
- Request return draft by late February
- File by April 15 (or extend to October 15)

## Tools-by-revenue summary

| Revenue/month | Bookkeeping setup |
|---|---|
| <\$2K | Wave + spreadsheet, DIY |
| \$2K–\$10K | InventoryLab + SellerBoard, DIY |
| \$10K–\$30K | InventoryLab + SellerBoard + QuickBooks for general ledger |
| \$30K–\$100K | Above + monthly bookkeeper or part-time CPA |
| \$100K+ | Above + dedicated CPA + possibly fractional CFO |

***

Next: [Year-end & 1099-K →](year-end.md)

*Last updated: 2026-05-05*
