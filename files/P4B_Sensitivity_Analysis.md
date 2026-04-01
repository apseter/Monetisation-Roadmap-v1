# P4B: SENSITIVITY ANALYSIS
## Stress-Testing the Financial Model — What Happens When Key Variables Shift
### Modular-Liner Trail Shorts D2C Brand | March 2026 | Confidential

---

> **P4B Subproject Summary:** This document systematically tests how the P4A financial model responds when 12 key variables change. For each variable, we model the base case, pessimistic case, and optimistic case, showing the exact impact on contribution margin, break-even orders, and Year 1 profitability. The final section combines multiple adverse variables into a "perfect storm" scenario to find the true breaking point of the business model.

> **P4B Core Finding:** The business model survives any single variable going wrong. It breaks when 3+ variables go wrong simultaneously (FOB rises + return rate spikes + bundle rate drops). The single most dangerous variable is bundle adoption rate — if it falls below 35%, the business model fundamentally doesn't work at current pricing.

---

## P4B TABLE OF CONTENTS

1. P4B.1: Methodology & Base Case Assumptions
2. P4B.2: Variable 1 — FOB Cost (Product COGS)
3. P4B.3: Variable 2 — Bundle Adoption Rate
4. P4B.4: Variable 3 — Return Rate
5. P4B.5: Variable 4 — Shipping Cost (UK)
6. P4B.6: Variable 5 — Payment Processing Rate
7. P4B.7: Variable 6 — Customer Acquisition Cost (CAC)
8. P4B.8: Variable 7 — Average Order Value (AOV)
9. P4B.9: Variable 8 — GBP/USD Exchange Rate
10. P4B.10: Variable 9 — Sell-Through Rate (Year 1)
11. P4B.11: Variable 10 — EU vs UK Order Mix
12. P4B.12: Variable 11 — Repeat Purchase Rate
13. P4B.13: Variable 12 — Wholesale vs DTC Mix
14. P4B.14: Combined Scenario Analysis (Stress Tests)
15. P4B.15: Sensitivity Summary — Tornado Chart Data
16. P4B.16: Key Insights & Decision Rules
17. P4B.17: P4B Action Items

---

## P4B.1: METHODOLOGY & BASE CASE ASSUMPTIONS

### P4B.1.1: Base Case Parameters

All sensitivities are measured against these base case values from P4A:

| Variable | Base Case Value | Source |
|---|---|---|
| Outer FOB cost | £6.50 ($8.25) | P2A |
| Liner FOB cost | £3.93 ($5.00) | P2A |
| Bundle retail price | £39 (VAT-inclusive) | P4A.3 |
| Bundle ex-VAT revenue | £32.50 | P4A.4 |
| UK shipping (Evri ParcelShop) | £2.62 | P3A |
| Payment processing | ~2.5% | P4A.6 |
| Returns provision | 20% of orders | P4A.4 |
| Return cost per return | £10.00 | P3A |
| Bundle adoption rate | 60% of orders | P4A.8 |
| Weighted AOV | ~£39 | P4A |
| UK:EU order split | 70:30 | P4A |
| Year 1 orders (base case) | 180 | P4A.10 |
| Sell-through rate | 60% (180/300 units) | P4A.10 |
| CAC (blended) | £15 | P4A.7 |
| GBP/USD rate | 1.27 | Current rate |
| Repeat purchase rate (12 months) | 30% | P10A.9 |

### P4B.1.2: How to Read Each Analysis

For each variable, we show: the pessimistic, base, and optimistic values; the impact on system bundle contribution margin (the primary product); the impact on break-even orders; and the Year 1 revenue/profit impact. Green = improvement, Red = deterioration.

---

## P4B.2: VARIABLE 1 — FOB COST (PRODUCT COGS)

### P4B.2.1: What Could Change

FOB cost depends on: fabric price from China (commodity fluctuation), factory CMT rates in Sialkot (negotiation, volume), trim costs (snaps, elastic, zippers), and GBP/USD exchange rate.

### P4B.2.2: Sensitivity Table — System Bundle (UK)

| Scenario | Bundle FOB | Bundle Ex-VAT Revenue | Variable Costs | Contribution | Margin % | Break-Even Orders |
|---|---|---|---|---|---|---|
| **Optimistic** | £8.50 (-£1.93) | £32.50 | £16.85 | **£15.65** | **48.2%** | ~265 |
| **Base case** | £10.43 | £32.50 | £18.78 | **£13.72** | **42.2%** | ~303 |
| **Pessimistic** | £13.00 (+£2.57) | £32.50 | £21.35 | **£11.15** | **34.3%** | ~373 |
| **Worst case** | £15.50 (+£5.07) | £32.50 | £23.85 | **£8.65** | **26.6%** | ~481 |

### P4B.2.3: Impact Assessment

FOB increasing by 25% (£10.43 → £13.00) reduces contribution margin by 8 percentage points and increases break-even by 70 orders. The model survives this — margins remain above 30%. FOB would need to reach ~£24 (a 130% increase) before the bundle becomes unprofitable on UK orders. **Verdict: LOW sensitivity. The model is robust to FOB increases.**

---

## P4B.3: VARIABLE 2 — BUNDLE ADOPTION RATE

### P4B.3.1: Why This Is the Most Dangerous Variable

The entire pricing architecture assumes 60% of customers buy bundles (not individual items). If customers overwhelmingly buy outers alone (£28) or liners alone (£15), the weighted AOV and margin profile collapses.

### P4B.3.2: Sensitivity Table — Weighted AOV & Contribution

| Bundle Rate | Product Mix | Weighted AOV | Weighted Contribution (UK) | Year 1 Revenue (180 orders) |
|---|---|---|---|---|
| **80%** | 80% bundles, 15% outer, 5% liner | £40.70 | £14.78 | £7,326 |
| **60% (Base)** | 60% bundles, 25% outer, 10% liner, 5% double | £38.95 | £12.69 | £7,011 |
| **40%** | 40% bundles, 40% outer, 15% liner, 5% double | £35.20 | £9.91 | £6,336 |
| **25%** | 25% bundles, 50% outer, 20% liner, 5% double | £31.85 | £7.56 | £5,733 |
| **10%** | 10% bundles, 60% outer, 25% liner, 5% double | £28.10 | £5.03 | £5,058 |

### P4B.3.3: Impact Assessment

At 40% bundle rate, Year 1 revenue drops by £675 and weighted contribution falls to £9.91 (from £12.69). At 25% bundle rate, the business is barely covering variable costs. Below 35% bundle rate, the LTV:CAC ratio drops below 1.0 — meaning you lose money on every customer acquired through paid channels.

**Verdict: HIGHEST SENSITIVITY. Bundle adoption rate is the single most important variable in the entire business model.** Every product page design decision, email sequence, and marketing message should be engineered to push bundles.

### P4B.3.4: Decision Rule

If bundle rate is <40% after 50 orders:
1. Increase bundle discount from 9% to 15% (£39 → £37 or £36)
2. Default product page to bundle (not outer)
3. Remove standalone liner from navigation (only show as add-on)
4. Add "Complete Your System" forced-choice at checkout
5. If still <40% after 100 orders: fundamentally rethink pricing architecture

---

## P4B.4: VARIABLE 3 — RETURN RATE

### P4B.4.1: Sensitivity Table — System Bundle (UK)

| Return Rate | Returns Provision per Order | Bundle Contribution | Margin % | Year 1 Impact (180 orders) |
|---|---|---|---|---|
| **10%** | £1.00 | £15.72 | 48.4% | +£360 vs base |
| **15%** | £1.50 | £14.72 | 45.3% | +£180 vs base |
| **20% (Base)** | £2.00 | £13.72 | 42.2% | Base |
| **25%** | £2.50 | £12.72 | 39.1% | -£180 vs base |
| **30%** | £3.00 | £11.72 | 36.1% | -£360 vs base |
| **35%** | £3.50 | £10.72 | 33.0% | -£540 vs base |

### P4B.4.2: Impact Assessment

Each 5% increase in return rate costs approximately £0.50 per order in margin. At 30% returns (plausible for a new brand with unvalidated sizing), contribution margin is still above 36% — painful but survivable. The model breaks at ~55% return rate, which would indicate a fundamental product defect.

**Verdict: MODERATE sensitivity. Returns hurt but don't kill the model unless they indicate a product failure.**

### P4B.4.3: Decision Rule

If return rate >25% after 30 returns: investigate sizing (is the grading wrong?). If return rate >30% after 50 returns: pause marketing, fix the size guide, consider offering free exchanges instead of refunds.

---

## P4B.5: VARIABLE 4 — SHIPPING COST (UK)

### P4B.5.1: Sensitivity Table — System Bundle

| Shipping Cost | Carrier | Bundle Contribution | Change vs Base |
|---|---|---|---|
| £1.99 | InPost Lockers | £14.35 | +£0.63 |
| **£2.62 (Base)** | Evri ParcelShop | £13.72 | Base |
| £3.55 | Royal Mail Tracked 48 | £12.79 | -£0.93 |
| £4.50 | DPD Next Day | £11.84 | -£1.88 |

### P4B.5.2: Impact Assessment

Shipping cost has limited impact because it's a small portion of the total variable cost stack. Switching from Evri to DPD would cost £1.88 per order — significant at volume but not model-breaking.

**Verdict: LOW sensitivity. Carrier choice matters but won't make or break the business.**

---

## P4B.6: VARIABLE 5 — PAYMENT PROCESSING RATE

### P4B.6.1: Sensitivity Table

| Processing Rate | Provider Context | Bundle Contribution | Change vs Base |
|---|---|---|---|
| 1.5% + 20p | Stripe standalone (hypothetical) | £14.13 | +£0.41 |
| **2.0% + 25p (~2.5% effective)** | Shopify Payments Basic | £13.72 | Base |
| 3.0% + 25p | Shopify + 3rd party gateway surcharge | £13.39 | -£0.33 |
| 5.0% + 25p | PayPal-heavy customer base | £12.74 | -£0.98 |

### P4B.6.2: Impact Assessment

**Verdict: VERY LOW sensitivity.** Even at 5% processing (worst case), contribution only drops by £0.98. Always use Shopify Payments as primary, but don't obsess over processing fee optimization at this scale.

---

## P4B.7: VARIABLE 6 — CUSTOMER ACQUISITION COST (CAC)

### P4B.7.1: Sensitivity Table — First-Order Profitability

| Blended CAC | Acquisition Source | First-Order Profit (Bundle) | LTV:CAC (3-Year) | Sustainable? |
|---|---|---|---|---|
| £0 | Organic / referral / word-of-mouth | £13.72 | Infinite | ✅ Best possible |
| £8 | Heavy organic with some gifting | £5.72 | 5.1:1 | ✅ Strong |
| **£15 (Base)** | Mixed organic + small paid | -£1.28 | 2.7:1 | ⚠️ Near-viable |
| £25 | Balanced organic + paid | -£11.28 | 1.6:1 | ⚠️ Below threshold |
| £40 | Paid-only acquisition | -£26.28 | 1.0:1 | 🛑 Unsustainable |
| £60 | Expensive paid channels | -£46.28 | 0.7:1 | 🛑 Burning cash |

### P4B.7.2: Impact Assessment

At £15 CAC, the first order is slightly unprofitable (-£1.28) but LTV recovers this with repeat purchases. At £25+ CAC, the business needs >40% repeat rates to break even on customer economics. At £40+ CAC (paid-only), the model is permanently unprofitable.

**Verdict: HIGH sensitivity. Organic acquisition is not optional — it's existential.** The model only works with a blended CAC below £20. This reinforces P5A's community-first strategy.

### P4B.7.3: Decision Rule

If blended CAC exceeds £20 after 60 days: cut paid spend immediately. Double down on organic, events, and community. If blended CAC exceeds £30: marketing strategy is fundamentally wrong — investigate product-market fit, messaging, or targeting.

---

## P4B.8: VARIABLE 7 — AVERAGE ORDER VALUE (AOV)

### P4B.8.1: Sensitivity Table

| AOV Driver | Weighted AOV | Revenue per 180 Orders | Change vs Base |
|---|---|---|---|
| Most buy double bundles (£49) | £46.50 | £8,370 | +£1,359 |
| Add-on items (socks, cap at Year 2) | £44.00 | £7,920 | +£909 |
| **Base case (60% bundles)** | £38.95 | £7,011 | Base |
| Most buy outer only | £31.00 | £5,580 | -£1,431 |
| Heavy liner-only sales | £22.00 | £3,960 | -£3,051 |

### P4B.8.2: Impact Assessment

AOV is directly coupled to bundle rate (P4B.3). The most impactful AOV lever is pushing customers from system bundle (£39) to double bundle (£49) — each upgrade adds £10 revenue and £4.15 contribution. Adding complementary products in Year 2 (socks, cap, buff) raises AOV without changing the core product.

**Verdict: HIGH sensitivity (but driven by bundle rate, already covered in P4B.3).**

---

## P4B.9: VARIABLE 8 — GBP/USD EXCHANGE RATE

### P4B.9.1: How FX Affects COGS

Fabric is priced in USD. Factory CMT is in PKR (correlated with USD). A weaker GBP increases COGS.

| GBP/USD | Bundle FOB in GBP | Change in FOB | Contribution Impact |
|---|---|---|---|
| 1.40 (GBP strong) | £9.46 | -£0.97 | +£0.97 per order |
| **1.27 (Base)** | £10.43 | Base | Base |
| 1.20 (GBP weak) | £11.04 | +£0.61 | -£0.61 per order |
| 1.10 (GBP very weak) | £12.05 | +£1.62 | -£1.62 per order |
| 1.00 (parity) | £13.25 | +£2.82 | -£2.82 per order |

### P4B.9.2: Impact Assessment

A 10% GBP depreciation (1.27 → 1.14) costs ~£1.00 per order. At 180 orders, that's £180 — painful but manageable. GBP/USD would need to reach parity (1.00) to seriously threaten margins, which is historically unprecedented in recent decades.

**Verdict: LOW-MODERATE sensitivity. Current pricing has ~10% FX buffer built in.**

---

## P4B.10: VARIABLE 9 — SELL-THROUGH RATE (YEAR 1)

### P4B.10.1: Sensitivity Table — 300 Unit Run

| Sell-Through | Units Sold | Revenue | Variable Costs | Fixed Costs (12mo) | Marketing | Unsold Inventory (at cost) | Net P/L |
|---|---|---|---|---|---|---|---|
| **90%** | 270 | £10,530 | £3,807 | £1,440 | £3,000 | £960 | +£2,283 |
| **70%** | 210 | £8,190 | £2,964 | £1,440 | £3,000 | £2,880 | +£786 |
| **60% (Base)** | 180 | £7,020 | £2,541 | £1,440 | £3,000 | £3,840 | +£39 |
| **40%** | 120 | £4,680 | £1,694 | £1,440 | £2,000 | £5,760 | -£454 |
| **20%** | 60 | £2,340 | £847 | £1,440 | £1,000 | £7,680 | -£947 |

*Note: Net P/L excludes initial Run 1 investment (~£9,700) and unsold inventory value. All scenarios show an operating loss when Run 1 investment is included.*

### P4B.10.2: Impact Assessment

At 60% sell-through, operations roughly break even (excluding Run 1 investment). Below 40%, the business loses cash even on operations. Above 70%, the business generates positive operating cash flow. The Run 1 investment (£9,700) is only recovered at near-complete sellout + Run 2 success.

**Verdict: HIGH sensitivity. The difference between 40% and 70% sell-through is the difference between "need more marketing" and "this is working."**

---

## P4B.11: VARIABLE 10 — EU VS UK ORDER MIX

### P4B.11.1: Sensitivity Table — Weighted Contribution per Order

| UK:EU Split | Weighted Bundle Contribution | Year 1 Total Contribution (180 orders) | Change vs Base |
|---|---|---|---|
| 90:10 (UK-dominated) | £13.14 | £2,365 | +£137 |
| **70:30 (Base)** | £11.97 | £2,155 | Base |
| 50:50 (Equal split) | £10.81 | £1,946 | -£209 |
| 30:70 (EU-dominated) | £9.65 | £1,737 | -£418 |

### P4B.11.2: Impact Assessment

Each 10% shift from UK to EU costs ~£70 in Year 1 contribution. EU orders are structurally less profitable due to higher shipping (£6.89 vs £2.62) and higher payment processing (~4.5% vs ~2.5%). Standalone liner to EU LOSES money.

**Verdict: MODERATE sensitivity. Push UK-first strategy. Defer EU investment until UK is profitable.**

---

## P4B.12: VARIABLE 11 — REPEAT PURCHASE RATE

### P4B.12.1: Sensitivity Table — 12-Month Impact (From 180 First-Time Buyers)

| Repeat Rate | Repeat Orders | Repeat Revenue | Repeat Contribution | Total Year 1+2 LTV Impact |
|---|---|---|---|---|
| **50%** | 90 | £3,510 | £1,235 | Excellent — approaching brand loyalty |
| **40%** | 72 | £2,808 | £988 | Strong |
| **30% (Base)** | 54 | £2,106 | £741 | Acceptable |
| **20%** | 36 | £1,404 | £494 | Below threshold |
| **10%** | 18 | £702 | £247 | Critical — customers don't come back |
| **0%** | 0 | £0 | £0 | Product failure or terrible CX |

### P4B.12.2: Impact Assessment

The difference between 20% and 40% repeat rate is £494 in additional contribution — enough to cover 2+ months of fixed costs. More importantly, repeat rate is the clearest signal of product-market fit. Below 20% means customers tried the product and didn't love it enough to return.

**Verdict: HIGH sensitivity for long-term viability. Not model-breaking in Year 1 but determines Year 2+ survival.**

---

## P4B.13: VARIABLE 12 — WHOLESALE VS DTC MIX

### P4B.13.1: Sensitivity Table — 200 Units Sold

| Channel Mix | DTC Units (42% margin) | Wholesale Units (47% margin on wholesale price) | Event Units (50% margin) | Total Contribution |
|---|---|---|---|---|
| 100% DTC | 200 × £13.72 | 0 | 0 | £2,744 |
| **70% DTC / 15% Events / 15% Wholesale (Recommended)** | 140 × £13.72 | 30 × £9.07 | 30 × £19.50 | £2,578 |
| 50% DTC / 30% Wholesale / 20% Events | 100 × £13.72 | 60 × £9.07 | 40 × £19.50 | £2,696 |
| 30% DTC / 50% Wholesale / 20% Events | 60 × £13.72 | 100 × £9.07 | 40 × £19.50 | £2,510 |

### P4B.13.2: Impact Assessment

Wholesale margins are lower per unit (£9.07 vs £13.72 DTC) but wholesale requires zero marketing spend, zero shipping cost, and zero CS cost. Event sales are the highest-margin channel at £19.50 contribution (50%+ margin — no shipping, packaging, or returns).

**The optimal mix is NOT 100% DTC.** A diversified channel strategy (70% DTC / 15% events / 15% wholesale) reduces risk with only a small margin trade-off, while providing cash flow stability and real-world customer feedback.

**Verdict: LOW sensitivity on margin, HIGH sensitivity on business resilience.**

---

## P4B.14: COMBINED SCENARIO ANALYSIS (STRESS TESTS)

### P4B.14.1: Scenario A — "Everything Goes Right"

| Variable | Value | vs Base |
|---|---|---|
| Bundle rate | 75% | +15% |
| Return rate | 12% | -8% |
| Sell-through | 85% | +25% |
| CAC | £8 (heavy organic) | -£7 |
| Repeat rate | 40% | +10% |

**Result:** Year 1 revenue: £10,500+. Positive operating cash flow from Month 3. Run 2 self-funded. Year 2 trajectory toward profitability.

### P4B.14.2: Scenario B — "Murphy's Law" (3 Things Go Wrong)

| Variable | Value | vs Base |
|---|---|---|
| FOB cost | £13.00 (+25%) | Fabric bait-and-switch or FX move |
| Return rate | 30% | Sizing issues with compression liner |
| Bundle rate | 40% | Customers prefer outer-only |

**Result:** Bundle contribution drops from £13.72 to **£8.24**. Break-even orders jump from 303 to **505**. Year 1 P/L: **-£12,000 to -£14,000** (including Run 1 investment). Run 2 is unjustifiable without fixing product/pricing.

**Survival actions:** Cut bundle price to £35. Fix sizing (re-grade liner). Push double-liner bundle harder. Increase event sales.

### P4B.14.3: Scenario C — "Perfect Storm" (5 Things Go Wrong)

| Variable | Value | vs Base |
|---|---|---|
| FOB cost | £13.00 | +25% |
| Bundle rate | 30% | Customers reject bundle concept |
| Return rate | 35% | Severe sizing problems |
| Sell-through | 30% | 90 units sold in 12 months |
| CAC | £35 | Paid-only, organic fails |

**Result:** Revenue: £2,700. Contribution: £540. Fixed costs: £1,440. Marketing: £3,150. Net P/L: **-£13,750** (excluding Run 1 investment). Total loss: **-£23,450.**

**This is the worst credible scenario.** The business loses the entire investment. 210 unsold units sit in storage. The right response at this point is to wholesale remaining stock at 60-70% off RRP (recover £2,000-3,000), write off the loss, and preserve remaining capital.

### P4B.14.4: Scenario D — "Fast Organic Sellout"

| Variable | Value | vs Base |
|---|---|---|
| Bundle rate | 70% | Above target |
| Sell-through | 95% (285 units in 6 months) | Near-complete sellout |
| CAC | £5 (mostly organic + referral) | Community-driven |
| Repeat rate | 35% | Strong product-market fit |

**Result:** Year 1 revenue: £11,800. Positive operating cash flow. Run 2 ordered at Week 3 (500 units). Year 1 net loss: -£4,200 (Run 1 investment partially recovered). Year 2 trajectory: breakeven by Q2 with larger Run 2.

**This is the best credible scenario** — still a net loss in Year 1 (expected for any apparel startup), but with strong momentum into Year 2.

---

## P4B.15: SENSITIVITY SUMMARY — TORNADO CHART DATA

### P4B.15.1: Variables Ranked by Impact on Bundle Contribution Margin

| Rank | Variable | Pessimistic Impact | Optimistic Impact | Range |
|---|---|---|---|---|
| **1** | **Bundle adoption rate** | **-£3.78** (40% rate) | **+£2.09** (80% rate) | **£5.87** |
| **2** | CAC (blended) | -£11.28 (£25 CAC) | +£5.72 (£8 CAC) | £17.00* |
| **3** | Sell-through rate | -£1,415 Y1 rev (40%) | +£1,359 Y1 rev (90%) | £2,774 |
| **4** | Return rate | -£1.00 (30%) | +£1.00 (10%) | £2.00 |
| **5** | FOB cost | -£2.57 (£13 FOB) | +£1.93 (£8.50 FOB) | £4.50 |
| **6** | Repeat purchase rate | -£247 Y2 (10%) | +£494 Y2 (40%) | £741 |
| **7** | UK:EU order mix | -£0.95 (50:50) | +£0.59 (90:10) | £1.54 |
| **8** | GBP/USD exchange rate | -£1.62 (1.10) | +£0.97 (1.40) | £2.59 |
| **9** | Shipping cost | -£1.88 (DPD) | +£0.63 (InPost) | £2.51 |
| **10** | Payment processing | -£0.98 (5%) | +£0.41 (1.5%) | £1.39 |
| **11** | Wholesale mix | -£166 (30% DTC) | Small gain | ~£166 |
| **12** | AOV (via add-ons) | Neutral | +£1,359 (£46 AOV) | £1,359 |

*CAC impact measured as first-order profitability, not contribution margin directly.

---

## P4B.16: KEY INSIGHTS & DECISION RULES

### P4B.16.1: The Three Variables That Matter Most

1. **Bundle adoption rate** — If <40%, restructure product page and pricing. If <35%, the business model doesn't work.
2. **Customer acquisition cost** — If blended CAC >£20, cut paid spend immediately. Organic must be primary.
3. **Sell-through rate** — If <40% at Month 6, do NOT reorder. Investigate product-market fit.

### P4B.16.2: The Three Variables That Don't Matter Much

1. **Payment processing rate** — Negligible impact. Use Shopify Payments and stop thinking about it.
2. **UK shipping cost** — Small impact. Evri is fine. Don't switch to premium carriers until AOV exceeds £60.
3. **GBP/USD exchange rate** — 10% buffer already built into pricing. Monitor but don't hedge at this scale.

### P4B.16.3: Monthly Sensitivity Check (5 Minutes)

Track these 3 numbers weekly and compare to base case:
- Bundle attach rate (target: >60%, alarm: <40%)
- Return rate (target: <20%, alarm: >30%)
- Blended CAC (target: <£15, alarm: >£25)

If any variable hits the alarm threshold for 2+ consecutive weeks, execute the corresponding decision rule from this document.

---

## P4B.17: P4B ACTION ITEMS

| # | Action | When | Priority |
|---|---|---|---|
| 1 | Confirm actual FOB quotes from Sialkot factories (validates Variable 1) | During supply chain pre-qualification | HIGH |
| 2 | Track bundle rate from Order 1 — dashboard metric | Launch Day | CRITICAL |
| 3 | Track return rate by SKU from Day 1 | Launch Day | HIGH |
| 4 | Track blended CAC weekly (post-purchase survey + UTMs) | Launch Day | HIGH |
| 5 | Run combined scenario analysis with actual data at Day 30 | Day 30 | HIGH |
| 6 | If bundle rate <40% after 50 orders: execute P4B.3.4 decision rule | ~Month 2 | CRITICAL |
| 7 | If CAC >£20 after 60 days: cut paid, go organic-only | ~Month 2-3 | HIGH |
| 8 | Quarterly sensitivity review with actual vs projected variables | Quarterly | MEDIUM |

---

## P4B KEY INSIGHT

> **The business model is resilient to any single variable going wrong — but breaks when 3+ variables deteriorate simultaneously.** The "Perfect Storm" scenario (FOB up + bundle rate down + return rate up + slow sell-through + expensive acquisition) results in a total loss of £23,450. The "Fast Organic Sellout" scenario results in strong momentum into Year 2. The difference between these outcomes is primarily determined by TWO variables: bundle adoption rate and organic customer acquisition. Everything else is noise. Obsess over those two metrics from Day 1.

---

*P4B: Sensitivity Analysis — Stress-Testing the Financial Model*
*Prepared March 2026 | Confidential*
