# RomanEcom Playbook

Source: "How Apple made him $100m | Roman Khan", What's Working Podcast, YouTube video `PbCr6CttFhA`, uploaded 2026-06-24. Notes are paraphrased from the auto-generated English transcript fetched 2026-06-30.

## Leading Words

- Whale: a larger actor or cultural force creating demand for the category.
- Why now: the inflection that makes the category newly obvious.
- Distribution-first: optimize owner cash distributions before profit growth, and profit growth before new revenue.
- Gravity: unavoidable variable costs between order and delivered customer value.
- Float: supplier-payment breathing room after product is ready to sell.

## Scorecard

| Axis | Green | Red |
| --- | --- | --- |
| Category timing | Search volume or cultural demand is compounding; there is a clear why-now. | Demand is flat, old, or driven mostly by founder passion. |
| Whale | A whale is educating the market: Apple, celebrity, scientific movement, platform shift, dominant incumbent, or mega-influencer. | The brand must create all category awareness itself. |
| Hero SKU | One product has a sharp USP and can carry acquisition. | Many unfocused SKUs, no obvious wedge. |
| PC1 | Gross ecommerce margin survives discounts, shipping revenue, and COGS. | Discounts or product cost erase margin before fulfillment. |
| PC2 | Delivered margin leaves room for CAC after returns, payment fees, inbound, duties, storage, and fulfillment. | Fulfillment gravity makes paid growth fragile. |
| PC3 | Marketing spend is judged against PC2, not against revenue. | CAC is justified with top-line ROAS or vague LTV. |
| OPEX/FTE | OPEX is lean; expensive FTEs create high revenue leverage. | Headcount, offices, software, or process bloat absorb PC3. |
| Supply chain | Components are sourced directly where possible, then assembled. | Factory sells the finished bundle and keeps avoidable margin. |
| Packaging/logistics | Package dimensions and materials are engineered for cost and shipping tiers. | Factory-default packaging raises storage, FBA, and last-mile costs. |
| Float | Terms exceed production plus shipping plus inbound time. | Growth consumes cash faster than terms create float. |

## Category And Acquisition

Start with category, product, and USP. A brand has a real shot when a hero SKU enters the right category at the right time.

Look for hard data first: Google keyword volume, Google Trends, Amazon category growth, marketplace ranking, social search, and retail shelf movement. Roman's Raycon example centered on wireless earbud demand compounding after Apple removed the headphone jack.

Then layer judgment: ask whether a whale is building the market for you. A whale can be an incumbent product, a platform decision, a celebrity with authentic category fit, a cultural figure, a scientific trend, or a strategic acquirer that validates the market.

Do not confuse a durable brand with a good acquisition. Roman's older private-equity screen favored brands with about $25M revenue, profitability, and 7+ years of operating history to avoid COVID-era false positives. His later correction: pay more for higher quality if the category has explosive fundamentals.

Common bad-category markers: passion-led product choice, long lead times, bad payment terms, slow inventory turns, no LTV, no whale, and no distribution advantage.

## Margin Ladder

Use ecommerce contribution profit instead of generic gross margin.

```text
PC1 = revenue - vouchers + shipping fee revenue - product COGS
PC2 = PC1 - delivered-order variable costs
PC3 = PC2 - marketing spend
EBITDA ~= PC3 - OPEX
```

Delivered-order variable costs include returns, exchanges, inbound logistics, duties, payment processing, pick/pack, storage, shipping subsidy, last-mile costs, and other per-order costs needed to get the product into the customer's hands.

CAC must be judged against PC2. If PC2 is 100 and OPEX were zero, 100 is the theoretical CAC ceiling for break-even first-order growth. PC3 is the controlled lever; PC1 and PC2 are gravity unless the operator changes product cost, packaging, shipping, payment fees, returns, or logistics.

## OPEX And FTE

Do not over-index on OPEX percent without checking the denominator. A high-AOV mono-product can show low OPEX percent while a complex retention business needs more operating surface.

Use revenue per expensive FTE. Count employees or contractors above roughly $2,000/month as FTEs for this purpose; treat low-cost VAs separately. Benchmarks from the interview:

- Minimum viable leverage: about $500k revenue per expensive FTE.
- Better target: about $1M revenue per expensive FTE.
- Roman's cited group level: above $3M revenue per expensive FTE.
- OPEX target mentioned: 3% for a very lean brand; 7% was the broader group context.

OPEX cuts matter because every point saved can either become distributions or fund more marketing while competitors carry heavier overhead.

## Supply Chain, Packaging, Logistics

Disintermediate. Do not let one factory hide all margin inside a finished product quote. Break the BOM into components, source key inputs directly, and send components to the assembler.

Packaging is an operator lever, not decoration. Audit:

- Material cost versus quality.
- Empty space and dimensional weight.
- FBA, storage, and last-mile tier thresholds.
- Damage rate and return cost.
- Whether shaving millimeters can move the product into a cheaper shipping category.

Logistics can be a moat when delivery speed, customs clearance, carrier integration, and inbound reliability reduce PC2 gravity.

## Payment Terms And Float

Payment terms decide how much EBITDA can actually leave the business.

```text
lead_to_ready_days = production_days + freight_days + inbound_receiving_days
float_days = supplier_terms_days - lead_to_ready_days
rough_distributable_share = max(0, float_days / supplier_terms_days)
```

Example: net 90 supplier terms and 30 days from PO to warehouse creates about 60 days of float, so roughly two-thirds of EBITDA can be distributed under steady, perfect conditions.

Growth changes the answer. If the business is tripling month over month, inventory needs can consume all float. Always test distributions against the next 13 weeks of POs, receivables, ad spend, inventory, and supplier payments.

## Distribution-First Review

Use this order when judging decisions:

1. Owner distributions.
2. Profit growth.
3. New revenue.

Revenue is last because growth that worsens inventory cash needs, CAC payback, or fulfillment gravity can make owners poorer while the top line looks better.

## Input Checklist

Ask for these fields when absent, but continue with explicit assumptions:

- Revenue, AOV, order count, SKU mix.
- Discounts/vouchers and shipping fee revenue.
- Product COGS by SKU or BOM.
- Returns, exchanges, refunds, chargebacks.
- Payment processing, duties, inbound freight, warehouse, pick/pack, storage, last-mile shipping.
- Marketing spend by channel and payback period.
- OPEX by category.
- Expensive FTE count and VA/back-office count.
- Supplier terms, deposits, production days, freight days, inbound receiving days.
- Inventory on hand, open POs, growth rate, stockout history.
- Category search trend, whale, hero SKU, USP, LTV/retention.
