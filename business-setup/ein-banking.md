# EIN, business bank, and books

🟢 → 🟡 — The infrastructure layer of your business. Done in week 1, never touched again. Done wrong, you'll regret it for years.

## EIN — Employer Identification Number

The federal tax ID for your business. Free, takes 5 minutes.

### Why you want one
- Required for business bank account
- Required for wholesale supplier accounts
- Required for reseller certificate
- Required for Brand Registry (in some cases)
- Replaces SSN for most business contexts (privacy)

### How to get one
1. Go to **irs.gov** → "Apply for an EIN online"
2. Verify business type (LLC, sole prop, corporation)
3. Provide owner info (your name + SSN)
4. Receive EIN immediately on screen
5. Save the EIN confirmation letter as PDF (you'll need it later)

Avoid third-party "EIN application services" that charge \$50–\$200 — the IRS does it free.

### Sole prop EIN
Even sole proprietors can (and should) get an EIN:
- Avoids using SSN with vendors / Amazon
- Required for some business banking
- Free, no obligation

## Business bank account

The single most important infrastructure setup.

### Why you need one
- Legal requirement for LLC liability protection
- Tax compliance (don't commingle business + personal)
- Better wholesale supplier credibility
- Cleaner bookkeeping
- Amazon disbursements clean and reportable

### Best banks for resellers

| Bank | Fees | Pros | Cons |
|---|---|---|---|
| **Mercury** | $0 | Online-first, excellent UI, Amazon integration | No physical branches |
| **Relay** | $0 | Specifically for online businesses | No cash deposits |
| **BlueVine** | $0 | High-yield checking, business-friendly | Newer, smaller |
| **Chase Business Complete** | \$15/mo (waivable) | Physical branches, large network | Fee structure |
| **Capital One Business** | $0 (Business Basic) | Solid online + physical | Slow approvals |
| **Bank of America Business** | \$16/mo | Largest physical network | Higher fees |

For most BoxedUp members: **Mercury** is the gold standard.
- Free, no monthly fees
- Excellent integration with Amazon Seller Central
- Real-time transaction notifications
- Send/receive ACH same-day

### Setup process
1. Apply online at the bank's website
2. Submit:
   - LLC paperwork (Articles of Organization)
   - EIN confirmation letter
   - Operating Agreement (if multi-member LLC)
   - Government ID
3. Wait 1–7 days for approval
4. Receive debit card + checks via mail
5. Connect to Amazon Seller Central (Settings → Account Info → Bank Account Information)

Once connected, Amazon disbursements (every 14 days, sometimes 7) deposit into the business account.

## Business credit card

Once you have a business bank account, get a business credit card.

### Why you want one

- **Cashback rewards** — typically 1.5–5% back on purchases
- **Sourcing capital float** — pay later, after you've already sold the inventory
- **Cleaner books** — all sourcing on one card vs scattered across personal cards
- **Builds business credit** — useful for future loans, lines of credit
- **Liability protection** — keeps business expenses separate

### Best cards for resellers

| Card | Annual fee | Rewards | Best for |
|---|---|---|---|
| **Amex Blue Business Cash** | $0 | 2% on first \$50K, then 1% | Default for most sourcing |
| **Chase Ink Cash Business** | $0 | 5% on office supplies, 2% on gas, 1% other | Niche bonus categories |
| **Chase Ink Unlimited Business** | $0 | 1.5% flat on everything | Simpler |
| **Capital One Spark Cash** | \$0–\$95 | 2% flat on everything | Travel-friendly |
| **Amex Business Gold** | \$295 | 4× on top categories | High spenders |

Many BoxedUp members keep 2–3 cards:
- Amex Blue Business Cash for general sourcing (2%)
- Chase Ink Cash for any category fitting the 5% bonus
- Backup card (different network) for retailers that decline Amex

### Stacking with cashback portals

You can stack:
1. Cashback portal (Rakuten / TopCashback) — 1–10%
2. Credit card rewards — 1.5–5%
3. Coupon code — 5–20%

Combined effective discount: 7–15% off retail. Real margin recovery.

## Bookkeeping software

Track every transaction. Required for accurate P&L + taxes.

### Tier 1: Free / cheap
- **Wave** — free, basic accounting
- **InventoryLab** — \$69/mo, includes COGS tracking + listing/shipping
- **SellerBoard** — \$15–\$50/mo, P&L focus
- **SpreadsheetCare** — free, manual

### Tier 2: Mid-range
- **QuickBooks Self-Employed** — \$15/mo, covers most sole props
- **QuickBooks Online Simple Start** — \$30/mo, full bookkeeping
- **FreshBooks** — \$15+/mo, invoicing-focused

### Tier 3: Enterprise
- **Bookskeep** — \$300+/mo, e-commerce-focused with Amazon integration
- **NetSuite** — for \$1M+ businesses

For most BoxedUp members: **InventoryLab + SellerBoard combo (\$80/mo)** + a CPA for annual tax filing covers everything.

## Setting up the books

Day 1 actions:

### Step 1: Connect bank to bookkeeping software
- Auto-import all transactions
- Saves 5+ hours/month of manual entry

### Step 2: Set up chart of accounts
Standard categories for resellers:
- **Income**
  - Amazon sales
  - eBay sales (if applicable)
  - Other marketplace sales
  - Reimbursements (treat as separate income line)
- **Cost of Goods Sold (COGS)**
  - Inventory purchases
  - Inbound shipping
  - Prep supplies
- **Operating Expenses**
  - Software subscriptions
  - Internet, phone (business portion)
  - Travel + mileage (sourcing trips)
  - Bank fees
  - Professional fees (CPA, lawyer)
  - Education / training (within reason)
  - Office supplies
  - Marketing (if applicable)
- **Other**
  - Owner draws (you taking money out)
  - Loan payments

### Step 3: Categorize transactions weekly
Don't let backlog build. Categorize each transaction within 7 days:
- "Amazon-Sales-Settlement" → Income → Amazon Sales
- "Walmart purchase \$X" → COGS → Inventory
- "Adobe subscription" → Operating → Software

After 30 days of discipline, this takes 10 minutes/week.

### Step 4: Reconcile bank statements
At the end of each month, ensure:
- Bookkeeping balance = bank statement balance
- All transactions accounted for

Mismatch >\$10: investigate (often forgotten transactions or duplicates).

## Inventory accounting (FIFO)

Inventory accounting matters for taxes. Default for resellers: **FIFO (First In, First Out)**.

### How it works
You sell inventory in the order acquired:
- Bought 100 units at \$5 in January
- Bought 100 units at \$7 in March
- Sold 50 units in April → COGS = 50 × \$5 = \$250 (Jan inventory)
- Sold 100 units in May → COGS = 50 × \$5 + 50 × \$7 = \$600

InventoryLab tracks this automatically. Manual tracking gets painful >50 SKUs.

### Other methods (rarely better)
- **LIFO (Last In, First Out)** — used for tax minimization in some scenarios; rarely allowed for ecommerce
- **Specific identification** — track each unit individually; only practical for high-value items
- **Weighted average** — average cost across all units; sometimes used for high-volume SKUs

For Amazon resellers: stick with FIFO. It's standard, accepted, and what your tools support.

## Tax-ready records

Year-round, maintain:

- **Receipts** — every business expense (digital or paper)
- **Mileage log** — if you drive for sourcing (write down odometer + purpose)
- **Per-unit COGS** — via InventoryLab or similar
- **Bank statements** — 7 years' retention recommended
- **Invoices issued** — if you do any B2B billing

Year-end actions:
- Print all reports for the year
- Reconcile final balance
- Provide to CPA (or DIY via TurboTax / similar)
- Save tax return + supporting docs forever

## When to hire a CPA

Triggers:
- Past \$50K/year revenue
- LLC with non-trivial expenses
- Multi-state nexus questions
- Considering S-corp election
- Don't enjoy bookkeeping

Cost: \$500–\$3,000/year for typical reseller.

Choose:
- **E-commerce-specialist CPA** > generic small-business CPA
- Gets your category, knows reseller-specific deductions
- Sets up systems for year-round, not just at filing

Find via:
- Discord recommendations (`#resources`)
- Reseller-focused firms: Bookskeep, AccountingProse, e-Comm Tax Pros
- Local accountants who serve Amazon sellers

## Tax-deductible reseller expenses

Common deductions (not exhaustive — confirm with CPA):

✅ **Inventory purchases** — full COGS at sale
✅ **Inbound shipping**
✅ **Prep supplies** (poly, bubble, labels)
✅ **Software** (Inventory Lab, SellerBoard, Keepa, SAS)
✅ **Sourcing mileage / vehicle** (mileage method or actual)
✅ **Home office** (% of home dedicated to business)
✅ **Internet + phone** (business portion)
✅ **Bank fees + interest**
✅ **Professional fees** (CPA, lawyer)
✅ **Education** within reason (paid courses, books, conferences)
✅ **Travel for sourcing** (sourcing trips, conferences)
✅ **Insurance** (business liability if applicable)

Tax law is complex. CPA should advise on edge cases.

## What's NOT deductible

❌ Personal expenses, even if "kind of related"
❌ Items you bought for yourself
❌ Family vacations disguised as "business"
❌ Excessive "education" (\$10K courses on FBA)
❌ Personal wardrobe (unless explicitly required uniform)

If audited, frivolous deductions get rejected + you owe the original tax + penalty.

## Annual ritual

End of each calendar year:

### December
- Reconcile all books
- Make any last legitimate purchases (deductible inventory, software annual subscriptions)
- Review for missing reimbursement claims (file before year-end)

### January
- Receive 1099-K from Amazon (if revenue >\$600 in 2024 onwards)
- Receive 1099s from any other platforms
- Compile P&L statement for the year
- Send to CPA OR file directly

### April
- Tax return filed by April 15 (or extension to October 15)
- Make estimated tax payment for Q1 of new year (if applicable)

### Quarterly (April, June, September, January)
- Pay estimated quarterly taxes (if business is profitable)
- Failing to pay quarterly = underpayment penalty at year-end

***

Next: [Sales tax: nexus, marketplace facilitator, exemptions →](sales-tax.md)

*Last updated: 2026-05-05*
