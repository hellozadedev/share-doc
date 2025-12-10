Smart move - eliminates the free user bleed. Here's your complete analysis.

---

## Cost Structure

**Fixed Monthly Costs**

| Expense | Cost |
|---------|------|
| AWS - Main Dashboard (8GB) | $40 |
| AWS - n8n (8GB) | $40 |
| SendGrid | $20 |
| MongoDB | $100 |
| Other | $100 |
| **Infra Total** | **$300** |
| Developer | $3,000 |
| **Grand Total** | **$3,300** |

---

**Per Customer Revenue**

| | Amount |
|---|--------|
| Plan Price | $14.99 |
| Stripe Fee (2.9% + $0.30) | -$0.73 |
| OpenAI (80 × $0.067) | -$5.33 |
| **Net Profit Per Customer** | **$8.93** |

---

## Breakeven Analysis

| Scenario | Fixed Cost | Customers Needed |
|----------|------------|------------------|
| Without Developer | $300 | **34** |
| With Developer | $3,300 | **370** |

---

## Profitability Table (Without Developer)

| Paid Customers | Revenue | Stripe | OpenAI | Fixed | **Net Profit** |
|----------------|---------|--------|--------|-------|----------------|
| 34 | $510 | -$25 | -$181 | -$300 | **$0** (breakeven) |
| 50 | $750 | -$37 | -$267 | -$300 | **+$147** |
| 75 | $1,124 | -$55 | -$400 | -$300 | **+$370** |
| 100 | $1,499 | -$73 | -$533 | -$300 | **+$593** |
| 150 | $2,249 | -$110 | -$800 | -$300 | **+$1,040** |
| 200 | $2,998 | -$146 | -$1,066 | -$300 | **+$1,486** |

---

## Profitability Table (With Developer)

| Paid Customers | Revenue | Stripe | OpenAI | Fixed | **Net Profit** |
|----------------|---------|--------|--------|-------|----------------|
| 370 | $5,546 | -$270 | -$1,972 | -$3,300 | **$0** (breakeven) |
| 400 | $5,996 | -$292 | -$2,132 | -$3,300 | **+$272** |
| 500 | $7,495 | -$365 | -$2,665 | -$3,300 | **+$1,165** |
| 750 | $11,243 | -$548 | -$3,998 | -$3,300 | **+$3,398** |
| 1000 | $14,990 | -$730 | -$5,330 | -$3,300 | **+$5,630** |
| 1500 | $22,485 | -$1,095 | -$7,995 | -$3,300 | **+$10,095** |
| 2000 | $29,980 | -$1,460 | -$10,660 | -$3,300 | **+$14,560** |

---

## Monthly Revenue Milestones

| Milestone | Customers Needed | Monthly Profit |
|-----------|------------------|----------------|
| Cover infra only | 34 | $0 |
| Cover all costs | 370 | $0 |
| $5k profit | 930 | $5,008 |
| $10k profit | 1,490 | $10,003 |
| $20k profit | 2,610 | $20,009 |

---

## Annual Projection (With Developer)

| Customers | Monthly Profit | Annual Profit |
|-----------|----------------|---------------|
| 400 | $272 | $3,264 |
| 500 | $1,165 | $13,980 |
| 750 | $3,398 | $40,776 |
| 1000 | $5,630 | $67,560 |
| 1500 | $10,095 | $121,140 |

---

## Key Metrics

| Metric | Value |
|--------|-------|
| Gross margin per customer | **59.6%** |
| Customer Lifetime Value (12 mo) | $107.16 |
| Max CAC to stay profitable | ~$50-60 |
| Revenue per scan | $0.187 |
| Cost per scan | $0.076 |

---

## Risk Analysis

| Risk | Impact | Mitigation |
|------|--------|------------|
| OpenAI price increase | Margin squeeze | Build buffer or adjust scan count |
| Low conversion | Can't cover developer | Start without developer, hire at 200+ customers |
| High churn | LTV drops | Focus on sticky features, annual plans |
| Server overload | Need to scale AWS | Upgrade at 500+ users |

---

## My Recommendation

**Phase 1 (0-100 customers):** Run without dedicated developer. You're profitable at 34 customers.

**Phase 2 (100-300 customers):** Hire part-time or contractor. Validate demand.

**Phase 3 (300+ customers):** Bring on full-time developer. You'll hit breakeven around 370.

---

**Bottom Line**

| | Without Developer | With Developer |
|---|-------------------|----------------|
| Breakeven | 34 customers | 370 customers |
| Target for healthy profit | 100+ | 500+ |
| Monthly profit at target | $593 | $1,165 |

---

No free tier = no bleed. Every user pays. Clean model.

Want me to create a spreadsheet with these projections?
