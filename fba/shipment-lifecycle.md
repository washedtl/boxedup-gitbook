# How a shipment actually flows

🟢 **Beginner.** Walking through what happens from "I have inventory in hand" to "the unit is live on Amazon and customers can buy it." Most beginners don't understand the actual mechanics until they've shipped 5–10 boxes.

## The 7 stages

```
1. Source             ──>  You buy inventory
2. Prep               ──>  Polybag, label, bubble
3. Build shipment     ──>  Tell Amazon what & where
4. Print labels       ──>  Box label + UPS shipping label
5. Carrier pickup     ──>  UPS picks up / you drop off
6. Receiving          ──>  Amazon scans units in
7. Available          ──>  Live on Amazon, sellable
```

Total elapsed time: typically **5–10 days** from shipment-creation to "Available."

## Stage 1: Source

Buy inventory from a retailer, wholesaler, or supplier. Get a receipt. Take a photo. Save it.

You now have units sitting in your home or warehouse.

## Stage 2: Prep

Each unit needs an FNSKU label (Amazon's barcode for your specific SKU) and may need additional prep depending on category. Common requirements:

- **Polybagging** — soft goods, multi-piece toys, anything where parts could separate
- **Bubble wrap** — fragile items
- **Labels-on-units** — the FNSKU sticker, typically on the side of the package
- **Stickered cover-ups** — covering UPC if there's a "made for [retailer]" mention
- **Suffocation warning** — required on polybags ≥5" opening

See the [Prep matrix](../reference/prep-matrix.md) for a full category-by-category breakdown.

> **Pro tip:** order a [DYMO LabelWriter 450](https://www.amazon.com/) (or 550) and a stack of polybags + suffocation labels in bulk before your first shipment. Doing prep with regular printer paper + tape is misery.

## Stage 3: Build shipment

In Seller Central → Inventory → Shipments → Create shipment.

You tell Amazon:
- **Which products** (by SKU + quantity)
- **Box dimensions and weight**
- **Ship-from address** (your home/warehouse)
- **Carrier** (Amazon Partnered Carrier, usually UPS)

Amazon then runs **placement optimization** — they decide which warehouse(s) to send your stuff to. You get one of three placement options:

| Placement option | Inbound fee | Speed |
|---|---|---|
| **Amazon-Optimized Shipment Splits** | \$0–\$0.30/unit | Fastest receive |
| **Partial Shipment Splits** | \$0.50–\$1.00/unit | Medium |
| **Minimal Shipment Splits** | \$1.00–\$1.50/unit | Slowest receive |

The "minimal splits" option means everything goes to ONE warehouse — convenient for you (one box, one label) but Amazon charges you for the convenience because it's slower and harder for them.

**The BoxedUp default**: Amazon-Optimized Shipment Splits if you're shipping multiple SKUs in one batch. The placement fee is small and the receive time is faster.

## Stage 4: Print labels

You get two label types per box:

1. **FBA shipment label** — the big QR code Amazon needs to identify your shipment when it arrives at the warehouse
2. **Carrier label** — your UPS or USPS shipping label, paid for by you (Amazon Partnered Carrier rates are usually 30–50% cheaper than retail UPS)

Print both. Tape FBA label to the **top** of the box (so warehouse workers see it first). Tape carrier label to the **side** or top.

If you're shipping multiple boxes, each gets its own pair of labels.

## Stage 5: Carrier pickup or drop-off

Three options:
- **Schedule UPS pickup** — UPS comes to your door, ~\$5 fee, sometimes free with Amazon Partnered Carrier
- **Drop off at UPS Store / The UPS Store** — free, you do the work
- **Drop off at FedEx / USPS** — only if you chose those carriers

Once dropped/picked up, tracking number activates. You can monitor in Seller Central → Manage Shipments.

## Stage 6: Receiving

This is where time disappears. Amazon's typical SLA:

- **Arrives at warehouse** — 2–5 days after pickup (UPS ground)
- **Check-in** — same day to 3 days
- **Counted/scanned/distributed to bins** — 1–7 days
- **Available for sale** — once everything's binned

In Q4 (Oct–Dec) receive times **balloon to 2+ weeks** as Amazon's warehouses backlog. Plan ahead — Q4 inventory needs to ship by mid-November to hit holiday sales.

> **Watch for "stuck" shipments.** If your shipment's been "Receiving" for >10 days without any units checked in, open a case in Seller Central → Help → Inbound shipment problem. They'll often manually expedite.

## Stage 7: Available

Units appear in your inventory dashboard with status `In Stock`. Listing goes live. Sales start.

If you priced competitively and have Buy Box, expect first sale within hours. If not, recheck:
- Are you priced at or below current Buy Box?
- Is your offer FBA?
- Are there 0 stock-out alerts?
- Is the listing's BSR moving (sales happening)?

## What goes wrong

Common failure modes and fixes:

| Problem | Cause | Fix |
|---|---|---|
| Shipment stuck "Working" forever | You didn't print labels yet | Inventory → Shipments → Continue |
| "Received less than expected" | Damage in transit / mis-pick | Open reimbursement case |
| Units sitting in Receiving 10+ days | Q4 backlog or warehouse issue | Open case after 10 days |
| FNSKU label peeled off | Bad sticker or rough handling | Amazon will sometimes re-label for a fee, or destroy |
| Wrong carton dimensions in shipment plan | You eyeballed | Always weigh + measure; oversize charge if wrong |

## Cost-per-unit shipping math

Inbound shipping is real money. Quick estimate:

- A 50 lb box of small items (≈80 units of \$25 product) ships for ~\$25 via Amazon Partnered Carrier
- Per-unit inbound: \$0.31

For oversize:
- A 70 lb box of bulky items (≈12 units) ships for ~\$45
- Per-unit inbound: \$3.75 — bake this into ROI

> **Don't underbuild boxes.** A 12×12×12" box with 5 items inside wastes space and gets you charged for dim-weight you didn't need to pay. Pack tight.

## Pro shipping habits

After ~10 shipments you'll develop these:

1. **Batch your prep** — never prep one unit at a time. Block 2 hours, prep 50 units, save context-switching
2. **Standardize box sizes** — pick 2–3 common sizes; bulk-buy them; never pick custom-size again
3. **Pre-print FNSKU sheet labels** — for replens, print a stack ahead and apply during prep
4. **Photo every box before sealing** — protects you on damage claims
5. **Save tracking numbers** — when you need to chase a stuck shipment, you'll thank yourself

***

Next: [Prep requirements →](prep-requirements.md)

*Last updated: 2026-05-05*
