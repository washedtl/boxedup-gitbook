# Account Health dashboard

🟡 **Intermediate.** Account Health is the central dashboard Amazon uses to grade you as a seller. Understanding what's measured, what triggers warnings, and how to defend metrics is the difference between a stable account and a chronically-suspended one.

## Where to find it

Seller Central → Performance → Account Health.

The dashboard shows three main areas:
1. **Customer Service Performance** — defects, late shipments, cancellations
2. **Product Policy Compliance** — IP complaints, restricted product issues
3. **Shipping Performance** — for FBM sellers

## The metrics that matter most

### Order Defect Rate (ODR)
**What it is:** % of orders with a defect (negative feedback, A-to-Z claim, chargeback)

**Targets:**
- 🟢 Healthy: <1%
- 🟡 Warning: 1–2%
- 🔴 Risk: >2%

**Why it matters:** ODR > 2% sustained = account suspension. Single most-important metric.

**Defenses:**
- Respond to negative feedback within 48 hours, offer resolution
- Refund proactively before A-to-Z claims are filed
- Don't dispute chargebacks unless you have iron-clad evidence

### Late Shipment Rate (LSR) — FBM only
**What it is:** % of FBM orders shipped late

**Targets:**
- 🟢 Healthy: <4%
- 🟡 Warning: 4–7%
- 🔴 Risk: >7%

**Why it matters:** LSR > 7% triggers account-level action.

**Defenses:**
- Ship daily for FBM
- Set realistic ship-by dates (don't promise next-day if you can't deliver)
- Use vacation mode when traveling

### Pre-Fulfillment Cancel Rate
**What it is:** % of orders you cancel before shipping

**Targets:**
- 🟢 Healthy: <2.5%
- 🟡 Warning: 2.5–3.5%
- 🔴 Risk: >3.5%

**Why it matters:** Tells Amazon you're overselling or have inventory chaos.

**Defenses:**
- Maintain accurate inventory counts
- Don't list items you don't have
- For FBM stockouts, mark out of stock immediately

### Valid Tracking Rate (FBM)
**What it is:** % of FBM orders with valid tracking

**Targets:**
- 🟢 Healthy: >95%
- 🟡 Warning: 90–95%
- 🔴 Risk: <90%

**Defenses:** always ship with tracking, upload tracking IDs promptly.

### On-Time Delivery Rate (FBM)
**What it is:** % of FBM orders delivered on or before promised date

**Targets:**
- 🟢 Healthy: >97%
- 🟡 Warning: 95–97%
- 🔴 Risk: <95%

**Defenses:** ship promptly, use reliable carriers, build buffer days into ship-by promises.

### Customer Service Dissatisfaction Rate (CSDR)
**What it is:** % of customer messages flagged as unhappy by Amazon's review system

**Targets:** keep below 25% of message responses

**Defenses:**
- Respond within 24 hours always
- Be apologetic and solution-oriented
- Don't argue or blame customers in messages

## Product Policy Compliance metrics

### Suspected Intellectual Property Violations
Recent IP claims filed against your account.

**Targets:** 0 ideal; 1–2 manageable; 3+ in 90 days = high risk.

**Defenses:**
- Source from authorized channels
- Avoid Tier 1 IP-protected brands without invoices
- Save receipts for 18+ months
- Respond to complaints with full POAs

### Received Intellectual Property Complaints
IP complaints filed by brand owners.

**Targets:** 0 ideal.

**Defenses:** same as above.

### Product Authenticity Customer Complaints
Customer messages claiming counterfeit/inauthentic.

**Targets:** 0 ideal; if any, refund + escalate to investigate sourcing.

### Product Condition Customer Complaints
"Received used as new," "received damaged," etc.

**Targets:** <1% of orders.

**Defenses:** ship only inventory you've inspected, prep correctly, don't risk used inventory marked as new.

### Product Safety Customer Complaints
Safety-related issues.

**Targets:** 0 — these escalate fastest to Amazon's safety review team.

### Listing Policy Violations
Title/description/image violations Amazon flags.

**Targets:** 0 — fix immediately.

### Restricted Product Policy Violations
Selling something you weren't allowed to.

**Targets:** 0 — instant suspension risk.

## Account Health Rating (AHR) score

Amazon recently introduced **AHR** — a single 0–1000 score that summarizes your account.

| AHR | Status |
|---|---|
| 800–1000 | 🟢 Healthy |
| 200–799 | 🟡 At risk (warnings active) |
| 0–199 | 🔴 Critical (suspension imminent) |

The AHR fluctuates daily based on your underlying metrics. Watching it weekly catches problems before they become suspensions.

## The weekly review

Once you have an active account, do this every Monday morning (5–10 minutes):

### Step 1: Check ODR
Click into Customer Service Performance.
- ODR: should be <1%
- If 1–2%: investigate which orders contributed; act
- If >2%: consider listing-level action (drop slow movers that produce defects)

### Step 2: Check IP claims
Click into Product Policy Compliance.
- Any new claims since last week?
- If yes: open the claim, plan response within 24 hours

### Step 3: Check listing health
Inventory → Manage Inventory → filter "Suppressed" and "Stranded"
- Suppressed: fix or remove
- Stranded: file removal order

### Step 4: Check restock limits
Inventory → Inventory Performance → Capacity Manager
- Are you approaching cap?
- If yes: pause new shipments, focus on selling-through

### Step 5: Note any trends
Are metrics trending in the wrong direction even if not yet warning?
- ODR climbing from 0.3% → 0.7% → 1.1% over 3 weeks = something's wrong, investigate now

## Responding to warnings

When Amazon sends a "Performance Notification":

### Tier 1: Performance reminder
"Your X metric is approaching the threshold." 
- **Action:** investigate and improve. Not yet a suspension trigger.

### Tier 2: Performance warning
"Your X metric is below standard."
- **Action:** required to submit a Plan of Action (POA) within 17 days. Failure to respond = suspension.

### Tier 3: Account warning
"Your account is at risk of suspension."
- **Action:** immediate POA required. Treat as urgent.

### Tier 4: Account suspended
- **Action:** see [suspension playbook](../anti-patterns/suspension.md). Submit POA within 17 days.

### Tier 5: Account deactivated permanently
- **Action:** legal/specialist help. Reinstatement rate <30%.

## POA template for Account Health warnings

For most performance warnings, here's a useful template:

```
Subject: Plan of Action — [Metric name] performance

Root cause:
We have analyzed our [metric] over the past 90 days and identified
the following root causes:

1. [Specific cause 1, e.g., late shipments due to inventory miscounts]
2. [Specific cause 2, e.g., customer complaints due to packaging damage]
3. [Etc.]

Corrective action:
We have taken the following immediate actions:
1. [Action 1, e.g., audited all SKU inventory counts]
2. [Action 2, e.g., upgraded packaging for fragile items]
3. [Action 3, e.g., implemented daily inventory sync]

Preventive action:
To prevent future issues:
1. [Process change 1, e.g., daily inventory reconciliation]
2. [Process change 2, e.g., quality-control checklist before shipping]
3. [Process change 3, e.g., weekly metric review]

Specific metrics improvement target:
We commit to bringing [metric] below [target] within 30 days.

Attached:
- Current metric data
- Process documentation
- [Any relevant evidence]

Thank you for your time.
```

Generic enough to adapt; specific enough to satisfy Amazon's POA reviewer.

## What kills accounts beyond metrics

Sometimes you can have perfect metrics and still get suspended. Less obvious risks:

### Multi-account violation
Operating two accounts (one main, one "for FBM" or "for spouse"). Amazon detects and bans.

### Buy-side TOS violations
Using Prime to source for resale. Multiple accounts to bypass quantity limits.

### Sketchy review activity
Your products getting suspiciously fast 5-star reviews from new accounts. Fake-review investigations are devastating.

### Unauthorized data scraping
Using bots that violate Amazon's ToS to scrape data. Account suspended for "misuse of services."

### Drop-shipping with retailer packaging
You drop-shipped from Walmart to a customer; the customer received a Walmart-branded box. Amazon detects.

These don't show on Account Health until enforcement happens. Avoid the behavior, period.

## Monitoring tools

Three free + paid options:

### Native Account Health (free)
What we've described above. Adequate for solo sellers.

### Account Health Notifications (free)
Settings → Notification preferences → Account Health alerts.
- Email + SMS when metrics cross thresholds
- Real-time defect notifications
- Recommended for everyone

### SellerBoard alerting
SellerBoard already pulls Account Health metrics. Configure alerts in the dashboard for ODR + IP-claim notifications via Discord/Slack/email — no extra tooling needed.

## Recovery from a bad period

If your metrics tank, recovery is possible but takes time:

### 30 days: stop the bleeding
- Pause sourcing
- Refund proactively on any complaints
- Drop slow movers that contribute to defects

### 60 days: clean baseline
- Metrics start to recover
- Focus on core SKUs with proven low-defect performance
- Build a 30-day clean track record

### 90 days: re-expand
- Metrics back to healthy ranges
- Begin sourcing again, but conservatively
- Source only proven categories, no experiments

### 180 days: forgiveness
- Older defects cycle off the rolling window
- AHR rebuilds toward 800+
- Account effectively "graduated" again

Patience is mandatory. Trying to "scale through" a metric problem just compounds it.

***

Next: [Reimbursements: lost, damaged, weight →](reimbursements.md)

*Last updated: 2026-05-05*
