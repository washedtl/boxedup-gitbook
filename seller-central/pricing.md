# Pricing automations & rules

🟡 **Intermediate.** Pricing on Amazon is a moving target. Buy Box price changes hourly. Manual repricing doesn't scale. Automated repricing is the default at scale — but a bad repricer wrecks margins faster than no repricing at all.

## Why pricing matters

Buy Box wins ~85% of sales. Buy Box winners are determined partly by price (combined with metrics, fulfillment method, etc.).

If your price is even \$0.50 above the next FBA seller, you can lose Buy Box. If it's \$0.50 below, you win — but if you go too low, you race-to-bottom your own margin.

The art: stay competitive without unnecessary price drops.

## Manual vs automated repricing

### Manual repricing
- You set prices once, monitor weekly
- No fee, no software
- Works if you have <30 SKUs or low-velocity inventory

### Automated repricing
- Software updates prices in real-time based on rules
- Fees: \$10–\$200/month depending on tier
- Required at scale (>100 SKUs)

Most BoxedUp members start manual, automate around \$10K/month revenue.

## How automated repricers work

A repricer monitors:
- Other sellers' prices on each listing
- Buy Box winner and price
- Your inventory level
- Your minimum + maximum price (set by you)

It then adjusts your price automatically:
- Match the Buy Box (if your competitor takes it)
- Stay just below the next FBA offer (if you can while above your minimum)
- Stay at your minimum if you can't undercut profitably
- Sometimes raise price (if competitors leave the listing)

## The minimum + maximum price floor

Every SKU you list needs:

### Minimum (floor)
The lowest price you'll ever sell at. Usually:
- Cost + 30% (RA)
- Cost + 20% (OA)
- Cost + 15% (wholesale)
- Or: your break-even after all fees

**Critical:** repricers will sometimes "race to bottom" if you don't set a hard minimum. Always set a floor to prevent below-cost sales.

### Maximum (ceiling)
The highest price you'd ask. Usually:
- 2× cost (for normal flips)
- 3× cost (for hot replens with stable demand)
- Higher (for restock plays during stockouts)

The maximum prevents your repricer from going too low when you're alone on a listing during a stockout.

## Repricer rule examples

### Rule 1: Compete with FBA only
"Match Buy Box, but only if Buy Box is FBA. Ignore FBM offers."

This prevents your repricer from chasing low-priced FBM offers that don't actually compete for Buy Box.

### Rule 2: Stay above the next-lowest FBA
"Set my price \$0.05 below the next-lowest FBA, but never below my minimum."

Standard competitive rule. Wins Buy Box rotation when possible.

### Rule 3: Raise price when no competition
"If I'm the only FBA seller, raise price to maximum."

Captures upside during competitor stockouts.

### Rule 4: Fixed price for replens
"For SKU X, lock at \$24.99. Don't reprice."

Some replens you've optimized for — don't let the repricer touch them.

### Rule 5: Hold price during launches
"For first 14 days after listing, don't reprice."

When you're trying to build review velocity, don't muddy the waters with price changes.

## Repricer tools comparison

| Tool | Cost | Best for |
|---|---|---|
| **Aura** | \$97+/mo | Solo sellers, cheap, reliable |
| **RepricerExpress** | \$55+/mo | Small to medium operations |
| **BQool** | \$25+/mo | Budget-conscious sellers |
| **Informed.co** | \$120+/mo | Mid-size sellers, AI features |
| **Seller Snap** | \$300+/mo | Large operations, advanced rules |
| **Channel Multi-Lister** | \$75+/mo | Multi-marketplace sellers |
| **Native Amazon Repricer** | Free | Beginners, basic only |

For BoxedUp scale (most members \$5K–\$30K/month): **Aura** or **BQool** strikes the right cost-to-feature balance.

## Common repricing mistakes

### Mistake 1: Race to the bottom
Two FBA sellers both running aggressive repricers. They both keep undercutting each other every minute.

Result: \$25 listing crashes to \$15 in a week. Both lose margin.

**Fix:** set realistic minimums. Don't engage in war pricing. If competition won't stop the spiral, walk from the listing.

### Mistake 2: Forgetting the floor
You set up a repricer rule but forgot to set minimum. It sells units at \$5 each — below your \$8 cost.

**Fix:** every SKU MUST have a minimum. Audit weekly.

### Mistake 3: Not adjusting for fees
You set minimum at "cost + 10%" but didn't account for FBA fees. Net margin is negative.

**Fix:** minimum should be your true break-even AFTER fees. SAS or your scanner shows the math.

### Mistake 4: Same rules for all SKUs
A high-velocity replen has different repricing needs than a slow seasonal item.

**Fix:** rule-based per-SKU configuration. Most repricers support custom rules per category or SKU.

### Mistake 5: Reacting to FBM
Your repricer drops price to match an FBM seller at \$15 (your FBA Buy Box was \$22). FBA at \$15 sometimes wins, but you're now below your break-even.

**Fix:** rule "Compete with FBA only, ignore FBM."

## When NOT to use a repricer

Specific scenarios where automated repricing isn't right:

### Brand-new ASIN
First 14–30 days, you want stable price for review-velocity build. Don't auto-reprice.

### Single-seller listing
You're the only one. Repricer has nothing to compare against. Set a fixed price and review monthly.

### Clearance / disposal scenarios
You're aggressively trying to clear inventory. Manually drop price; don't let auto-repricer get cute.

### High-margin niches
Listings with 50%+ margin and stable Buy Box. Repricer churn does more harm than good.

## Pricing strategy by channel

### RA-sourced inventory
- Aim for 30%+ ROI minimum
- Minimum price: cost + 35%
- Maximum: market Buy Box current
- Reprice: standard "match Buy Box, don't go below minimum"

### OA-sourced inventory
- Aim for 20%+ ROI minimum
- Minimum: cost + 25%
- Standard repricing

### Wholesale-sourced inventory
- Aim for 15%+ ROI minimum
- Minimum: respect MAP (brand's minimum advertised price)
- Maximum: MSRP
- Reprice: stay between MAP and MSRP

### Restock-monitor wins
- Buy at retail; sell at elevated 3P prices
- Minimum: cost × 1.5 (you have margin to play with)
- Maximum: market 3P price
- Reprice: stay competitive but don't lead the race down

### Bundle / private label
- Self-set price; less competition pressure
- Manual pricing usually fine
- Adjust seasonally and as competition emerges

## Real-time monitoring

Even with automation, watch:

### Daily (5 min)
- Top 10 SKUs by revenue: any price drops?
- Buy Box win rate: still 70%+?

### Weekly (15 min)
- Per-SKU profit margins: any erosion?
- Inventory aging: any SKUs getting stuck?
- Repricer rule effectiveness: any SKUs racing to floor?

### Monthly
- Audit minimum/maximum prices: still valid given fee changes?
- Review repricer rule changes Amazon may have implemented
- Compare to competitor strategy: are they undercutting more aggressively?

## Pricing during stockouts

When you (or competitors) run out:

### When you go OOS
- Price doesn't matter (no sellable inventory)
- Don't adjust
- Plan reorder cycle

### When competitor goes OOS
- You may now be solo or in smaller pool
- Repricer should auto-raise price
- Verify it's working as expected

### When ALL FBA goes OOS (only FBM remains)
- FBA returns trigger Buy Box re-allocation
- You can ride elevated 3P pricing if you restock first

This is the [Restock/Monitor strategy](../sourcing/restock-monitor-strategy.md) in action — pricing matters less than speed.

## Pricing for new listings

For listings you create yourself (private label, bundles):

### Strategy 1: Penetration pricing
Launch at 10–20% below competitive parity to drive initial reviews + sales velocity.

### Strategy 2: Premium positioning
Launch above market if your branding/quality justifies it. Slower velocity, higher margin.

### Strategy 3: Match-and-build
Match competitive parity. No price advantage, but build with marketing + reviews.

For most arbitrage sellers, this isn't relevant — you're competing on existing listings, not creating new ones.

## Avoiding price-tank patterns

Some patterns indicate Buy Box price is about to crash:

### Pattern 1: Offer count spike
3 → 12 sellers in 14 days = race-to-bottom incoming.

**Action:** lower your inventory commitment; don't reorder if scaled in.

### Pattern 2: Multiple FBA sellers reduce inventory
Three competitors visible in inventory levels (Keepa shows). All have lower than usual stock = they're trying to clear inventory.

**Action:** they're worried about future demand. You should be too.

### Pattern 3: Brand started flooding
Suddenly 30+ FBA listings for same brand appear. Brand is over-distributing.

**Action:** prices will tank as everyone competes. Walk.

***

Next: [Reports you should run weekly →](reports.md)

*Last updated: 2026-05-05*
