# Prep requirements (poly, bubble, suffocation, etc.)

🟢 → 🟡 — Amazon's prep rules are unforgiving. A unit shipped without correct prep can be destroyed, returned to you at your cost, or block your inventory from being received. Read this before your first shipment.

## The prep types

| Prep type | What it is | When required |
|---|---|---|
| **Polybag** | Sealed plastic bag | Soft goods, multi-piece, anything with separable parts |
| **Bubble wrap** | Bubble protection | Fragile items (glass, ceramic, porcelain) |
| **Taping** | Sealing the original box | Boxed items where the box might open in transit |
| **Suffocation warning** | Specific warning text on bag | Any polybag with opening ≥5" |
| **FNSKU labeling** | Amazon's barcode on the unit | All FBA units (no exceptions) |
| **Cover-up labeling** | Sticker over UPC or "made for [retailer]" text | Items meant for retailer-specific channels |
| **Sets / Bundle stickers** | "Sold as set, do not separate" | Multi-pack listings |
| **Expiration sticker** | Visible expiration date | Grocery, supplements, beauty |

## When polybag is required

Polybag is the most common prep step. Amazon requires it on:

- **Soft goods** — apparel, plush toys, fabric items
- **Multi-piece toys / games** with parts that could fall out
- **Items with exposed adhesive surfaces** — stickers, tape products
- **Pillows, bedding, towels** — anything that could absorb moisture
- **Liquid-adjacent products** — anything that could leak in transit (yes, even sealed)

The bag must be:
- **Sealed** (not just zip-top — heat-sealed or self-adhesive)
- **Transparent or translucent** (so warehouse workers can scan UPC through it)
- **Within 0.5" of unit dimensions** (no excess flapping)
- **With suffocation warning** if opening ≥ 5"

> **Polybag thickness:** Amazon requires ≥1.5 mil. The 1 mil bags from cheap online sellers won't pass.

## Suffocation warning — exact text required

If your polybag opening is 5" or larger, you need this text printed on it:

```
WARNING: To avoid danger of suffocation, keep this bag away from
babies and children. Do not use this bag in cribs, beds, carriages,
or playpens. This bag is not a toy.
```

You can buy:
- **Pre-printed polybags with suffocation warning** (most common — Amazon's preferred path)
- **Suffocation warning labels** to apply onto generic polybags

For BoxedUp scale: bulk-order 6"×9" + 9"×12" + 12"×15" pre-printed suffocation polybags from Uline, Veritiv, or Amazon itself. Costs ~\$0.10–\$0.25/unit.

## FNSKU labeling

This is the **non-negotiable** prep step. Every FBA unit needs an FNSKU label:

- Amazon's barcode for your specific SKU
- Format: `X` followed by 9 alphanumeric characters (e.g., `X001ABC234`)
- Must be **scannable** — printed on label paper, not regular paper
- Must be **placed on a flat surface**, not a curved seam
- Must **cover the original UPC** (or both must be visible — but covering is safer to prevent commingling)

**The FBA-cost-cutter:** "Stickerless, commingled" inventory.

When you list a brand-new ASIN, Amazon offers two options:
- ✅ **Use Amazon-supplied FNSKU label** (default) — your inventory stays segregated
- ⚠️ **Stickerless / commingled** — Amazon pools all sellers' inventory by UPC; saves prep time but **YOU CAN BE BLAMED for someone else's counterfeit fulfilling your sale**

**The BoxedUp rule: never use stickerless.** Always FNSKU-label every unit. Yes, it's more work. Yes, it protects your account.

## Cover-up labeling

Some retail products say "Sold exclusively at Walmart" or have a Walmart-specific UPC. Amazon doesn't care that you bought it legally at Walmart — they care that the listing UPC matches the unit UPC.

Two scenarios:
- **Same UPC**, "made for [retailer]" text only — usually fine to ship as-is
- **Retailer-specific UPC** that doesn't match the listing — you must cover the UPC with an opaque sticker

⚠️ **Retailer-exclusive items are an inauthentic-claim risk.** Some brands flag them. If you're sourcing Costco-exclusive Kirkland items or Walmart-exclusive variants, do extra due diligence.

## Sets and bundles

If you're shipping a multi-pack as a single sellable unit:

- All pieces must be **physically connected** (taped, polybagged together, or in a sealed inner box)
- Apply a **"Sold as set, do not separate"** sticker on the outside
- Apply your FNSKU on the outside set, not on individual pieces

Without the "Sold as set" sticker, warehouse workers will sometimes split the set into individual units and you'll have phantom inventory issues.

## Hazmat prep

Some products are classified hazmat by Amazon's algorithm:
- Anything with a battery (lithium-ion especially)
- Aerosol cans
- Anything flammable
- Some cleaning products
- Magnetized items (e.g., some toys with magnets)

Hazmat units require:
- **MSDS (Material Safety Data Sheet) submission** before listing
- **Approval from Amazon's hazmat review team** (1–6 weeks)
- **Special inbound prep** — sealed in original packaging, no leaks
- **Restricted shipping methods** — usually ground only

Many BoxedUp members avoid hazmat entirely because of the approval lag. Worth knowing the rule even if you're not selling hazmat — it'll come up.

## The category prep matrix

Quick reference (full version: [Prep matrix](../reference/prep-matrix.md)):

| Category | Polybag | Bubble | Suffocation warning | Notes |
|---|---|---|---|---|
| Books | No | No | No | Just FNSKU |
| Toys (boxed) | No | No | No | Just FNSKU; tape if box opens |
| Toys (loose pieces) | Yes | No | If ≥ 5" opening | "Sold as set" sticker |
| Plush toys | Yes | No | Yes | Always polybag soft goods |
| Apparel | Yes | No | Yes | Polybag with suffocation warning required |
| Glass / ceramic | No | Yes | No | Bubble wrap mandatory |
| Electronics | Maybe | If fragile | No | Often boxed; check by item |
| Beauty (liquid) | Yes | Sometimes | If polybagged ≥ 5" | Anti-leak prep |
| Food / Grocery | Yes (often) | No | Sometimes | Expiration date visible |
| Hazmat | Special | Special | Per spec | Pre-approved only |

## When prep fails

Amazon's response to prep violations:

- **Minor (missing FNSKU)** — they'll FNSKU-label for you and charge \$0.30/unit
- **Moderate (no polybag on required item)** — warning + chargeback to you
- **Major (no suffocation warning, prep fee)** — \$0.30–\$1.00/unit prep fee + warehouse delay
- **Severe (hazmat without approval)** — listing suspension + potential account-level action
- **Repeat offender** — Amazon disables your "no prep" SKU options globally

After your first chargeback, you'll never skip prep again.

## Prep services — when to outsource

For BoxedUp members shipping >100 units/month, prep services make sense:

- **Cost** — typically \$0.50–\$1.50/unit + monthly minimum (~\$500–\$2000)
- **What they do** — receive your inventory, prep, FNSKU-label, build shipment, ship to FBA
- **Where to find** — directories like Prep Centers Network, FBA Prep Logistics
- **The catch** — prep centers in low-tax states (NH, OR, MT, DE, AK) are most common; you'll ship inventory cross-country

The math works once your time is worth more than the prep fee. For most members that's around the \$5K–\$10K/month revenue mark.

***

Next: [Building shipping plans →](shipping-plans.md)

*Last updated: 2026-05-05*
