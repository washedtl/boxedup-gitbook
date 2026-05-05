# Account suspension playbook

🔴 **Critical.** Account suspension happens to nearly every reseller eventually — usually for things you didn't do, sometimes for things you did. The difference between a 1-week reinstatement and a permanent ban is your response in the first 48 hours.

## The four flavors of suspension

| Type | Severity | Typical duration | Reinstatement rate |
|---|---|---|---|
| **Listing suppressed** | Lowest | 1–14 days | 95% with POA |
| **ASIN-level suspension** | Low | 7–30 days | 85% with POA |
| **Account-level suspension** | High | 30–90 days | 60–80% |
| **Account-level permanent ban** | Highest | Forever | 10–20% (need expert help) |

The earlier you act, the better the outcome.

## What triggers suspension

In approximate order of frequency:

1. **IP complaints** — brand owner files inauthentic / counterfeit / trademark claim
2. **Inauthentic complaints** — Amazon auto-flags based on customer messaging or pattern
3. **Used sold as new** — customer complaint that your "new" unit was opened
4. **Account health metrics** — ODR > 1%, late shipment > 4%, cancellation > 2.5% (FBM)
5. **Drop-shipping detection** — packaging/return labels show another retailer
6. **Multiple accounts** — Amazon detects you operating two accounts (ToS violation)
7. **Fraudulent activity** — credit card chargebacks, fake reviews, manipulated rankings
8. **Restricted product** — selling something you weren't allowed to (haz, IP, etc.)
9. **Counterfeit confirmation** — test-buy by Amazon or brand confirmed fake

## The first 48 hours

When you get the suspension email, time is the enemy. Steps in order:

### Hour 0: Read the email carefully

Amazon's emails are templated and vague. Look for:
- **Specific ASIN(s) listed** — narrow scope = better
- **Specific complaint type** — "inauthentic," "trademark," "used as new"
- **Performance metrics cited** — ODR, late shipment, etc.
- **Deadline for response** — usually 17 days but sometimes 7

Screenshot the email. Save it.

### Hours 1–4: Triage

Don't respond yet. Investigate first:

- **Pull the ASIN's order history** — find the specific orders that triggered the complaint
- **Check Account Health** — what's the actual metric showing red?
- **Pull customer messages** — are there negative messages on that ASIN?
- **Pull A-to-Z claims** — any pending or recent?
- **Compare your shipped unit to the listing** — was anything off?

You're building a story of what happened.

### Hours 4–24: Plan of Action draft

Amazon's reinstatement process requires a **Plan of Action (POA)** with three sections:

```
1. Root cause — what specifically went wrong
2. Corrective action — what you did to fix it immediately
3. Preventive action — what process changes prevent recurrence
```

The POA gets graded by an Amazon rep. **Quality matters more than length.** Generic POAs ("we'll do better") fail. Specific ones win.

### Hours 24–48: Submit + wait

- Account Health → Suspended → Reinstate
- Paste your POA in the form
- Attach evidence (receipts, invoices, photos)
- Submit

Amazon's response: 24 hours to 14 days.

## A sample winning POA

For an inauthentic complaint on a single ASIN:

```
Subject: Reinstatement Plan — ASIN B0XXXXX (Inauthentic complaint)

Root cause:
On [date], a customer filed an inauthentic complaint on ASIN B0XXXXX
(Stanley 40oz Tumbler). The complaint stated they suspected the
product was counterfeit. After investigation, I believe the customer
was confused because:

- The unit I shipped was a Walmart-exclusive variant with slightly
  different packaging than the standard listing imagery
- I sourced this product legitimately from [Walmart receipt attached]
- The product is authentic Stanley merchandise; however, I should
  have anticipated that the variant packaging could cause confusion

Corrective action:
1. I have suspended all FBA listings of this ASIN
2. I have removed the existing FBA inventory of this ASIN via removal
   order (Order #XXXXX)
3. I have refunded the customer in full for the order in question
4. I have audited my entire inventory for similar variant-packaging
   risks

Preventive action:
1. Sourcing audit: I will no longer source variant-packaging items
   for listings where the standard imagery doesn't match the
   product's exact packaging
2. Documentation: Going forward, I will photograph every unit shipped
   to FBA, with batch codes visible
3. Wholesale path: For Stanley products specifically, I am pursuing
   a wholesale relationship with [distributor name] to ensure all
   future inventory matches listing imagery exactly
4. Customer communication: I have added language to my account profile
   explaining that variant packaging may differ slightly while products
   remain authentic

Attached:
- Walmart receipt dated [date] showing purchase of 5 Stanley 40oz
  Tumblers at $29.97 each
- Photo of Stanley's authentic batch code on the unit shipped
- Removal order confirmation
- Customer refund confirmation

Thank you for your time and consideration.
```

This POA wins because:
- It admits a real cause (variant-packaging confusion) without admitting fault for counterfeiting
- It shows specific, time-stamped corrective actions
- It includes preventive process changes, not vague promises
- It attaches evidence

## What kills POAs

Common mistakes that lead to denial:

❌ **Generic language** — "We will improve our processes" (no, what specifically?)
❌ **Blaming the customer** — "The customer was wrong" (Amazon sides with customers)
❌ **Blaming Amazon** — "Your system flagged us incorrectly" (don't antagonize)
❌ **No evidence attached** — POAs without receipts/invoices rarely win
❌ **Apology theater** — "We are deeply sorry" without specifics is empty
❌ **Mass-copying templates** — Amazon reps see thousands; obvious templates fail

✅ **What wins:** specific, evidenced, accountable, professional.

## Escalation when POAs fail

If your first POA is denied:

### Round 1: Re-file with stronger evidence
- Add more photos
- Include wholesale invoices if you didn't before
- Strengthen the corrective and preventive sections
- Sometimes a different rep approves what the first denied

### Round 2: Hire a POA specialist
- Specialty firms like **Riverbend Consulting** and **Amazon Sellers Lawyer** handle these
- Costs: \$200–\$1,500+ depending on case complexity
- Worth it for accounts with significant inventory at FBA or revenue at risk

### Round 3: Lawyer up
- For permanent bans, only legal pressure (or arbitration via the Amazon Services Agreement) gets accounts back
- Costs: \$2K–\$15K+
- Usually worth it for accounts doing >\$10K/month
- Many sellers' lawyers offer free consultation

### Round 4: Walk away
- Not all suspensions are reinstatable
- For small accounts, the cost of fighting may exceed the value
- Time to start fresh (with caution — multi-account flags will block a new signup if you're not careful)

## Preventive measures

The cheapest reinstatement is the one you never need.

### Sourcing
- Avoid Brand Registered listings without authorized invoices
- Save every receipt for 18 months
- Build wholesale paths for top SKUs
- Avoid known IP-aggressive brands (see [IP complaints](ip-complaints.md))

### Operations
- Monitor Account Health weekly
- Respond to customer messages within 24 hours
- Don't argue with customers; refund and move on for under \$50
- Audit suppressed listings monthly; submit removals immediately

### Account hygiene
- One Amazon account per household IP/payment method (TOS)
- Don't share accounts across business partners using personal emails
- Use a dedicated email + payment method for the seller account
- Never let someone else log in to "help" — security audits trigger flags

## Multi-account violation — the silent killer

If you're suspended once and try to open a new account:

- Amazon detects via IP, payment method, address, device fingerprint, banking info, browser fingerprint
- **They will find it.** Multi-account detection is one of Amazon's most aggressive enforcement systems.
- Result: instant ban on the new account + permanent ban on the original

If you must open a new account after a permanent ban:
- New IP (different ISP, ideally different physical location)
- New EIN (different LLC)
- New bank account
- New device
- Different family member's name (with their full knowledge and consent)
- Different shipping address

Even then, ~50% chance Amazon detects within 6 months. **Multi-accounting is a high-risk play for high-stakes situations only.**

## When suspension is final

Some triggers result in near-permanent bans:

- **Confirmed counterfeit** — selling fake luxury, Apple, Disney, etc.
- **Repeat offender on the same complaint type** (3+ inauthentic complaints in 90 days)
- **Multi-account violation**
- **Fraud (chargebacks, fake reviews, manipulated rankings)**
- **Selling restricted/banned products** (weapons, controlled substances)

These are the bans that don't come back. Avoid the trigger by sourcing legitimately, scaling honestly, and never crossing platform rules.

## A note on emotional management

Suspension is brutal. Your inventory is locked, sales are zero, and the appeal process is opaque. Many BoxedUp members go through this once and quit.

The reality:
- **Most suspensions reinstate** — first-time, single-ASIN, with good POA = 80%+ reinstatement rate
- **The wait is the hardest part** — 1-2 weeks of zero sales feels existential, but it ends
- **Veterans have all been suspended** — every long-term reseller in the Discord has at least one suspension story

If you're suspended, post in `#account-issues` immediately. Members will share their POA templates and walk you through the process. You're not alone in this.

***

Next: [Counterfeit traps when sourcing →](counterfeits.md)

*Last updated: 2026-05-05*
