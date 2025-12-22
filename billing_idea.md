# Syntrix Billing Plan

## Overview

Syntrix uses **user-based billing** where the store owner pays for all stores they own. Billing is based on the number of unique purchase events tracked across all owned stores.

## Pricing Tiers

| Tier | Purchase Range | Rate |
|------|----------------|------|
| **Trial** | 0 - 9 purchases | **Free** |
| **Base** | 10+ purchases | **$15/month per store** (includes first 500 purchases per store) |
| **Tier 1** | 501 - 5,000 purchases | **$50 per 1,000 purchases** |
| **Tier 2** | 5,001+ purchases | Volume discounts (5% off every 5,000, floor at $40/1K) |

## How It Works

### Trial Period
- First **10 purchases** are completely free
- No payment method required
- Full access to all features

### Base Charge
- Once you exceed 10 purchases, base pricing begins
- **$15/month per store** you own
- Includes **500 purchases per store** in the base price
- Example: 2 stores = $30/month base, includes 1,000 purchases

### Usage-Based Pricing (Tier 1)
- Applies to purchases beyond the included amount
- **$50 per 1,000 purchases** ($0.05 per purchase)
- Covers purchases from 501 to 5,000

### Volume Discounts (Tier 2)
- Kicks in after 5,000 purchases
- **5% discount** for every additional 5,000 purchases
- Minimum rate floor: **$40 per 1,000 purchases**

## Example Calculations

### Example 1: Small Store
**1 store, 300 purchases/month**

| Component | Calculation | Amount |
|-----------|-------------|--------|
| Base charge | $15 × 1 store | $15.00 |
| Usage | 300 included in base | $0.00 |
| **Total** | | **$15.00/month** |

### Example 2: Growing Business
**2 stores, 1,500 purchases/month**

| Component | Calculation | Amount |
|-----------|-------------|--------|
| Base charge | $15 × 2 stores | $30.00 |
| Included | 500 × 2 stores = 1,000 | $0.00 |
| Tier 1 | 500 × ($50/1000) | $25.00 |
| **Total** | | **$55.00/month** |

### Example 3: High Volume
**1 store, 8,000 purchases/month**

| Component | Calculation | Amount |
|-----------|-------------|--------|
| Base charge | $15 × 1 store | $15.00 |
| Included | 500 purchases | $0.00 |
| Tier 1 | 4,500 × ($50/1000) | $225.00 |
| Tier 2 | 3,000 × ($47.50/1000) | $142.50 |
| **Total** | | **$382.50/month** |

## Billing Statuses

| Status | Description | Store Access |
|--------|-------------|--------------|
| `trial` | Under 10 purchases, no payment required | Full access |
| `pending_payment` | Trial ended, payment method required | Paused |
| `active` | Payment method on file, billing active | Full access |
| `past_due` | Payment failed, in grace period | Full access |
| `locked` | Grace period expired, account locked | Paused |
| `cancelled` | Subscription cancelled | Paused |

## Billing Cycle

1. **Billing Anchor**: Set when payment method is first added
2. **Monthly Cycle**: Bills on the same day each month
3. **Usage Tracking**: Purchase events counted per billing period
4. **Invoice Generation**: Created at end of each billing period

## Grace Period

- **3 days** after a failed payment before account is locked
- During grace period, stores remain accessible
- Multiple retry attempts are made
- Email notifications sent for failed payments

## Payment Methods

- Credit/debit cards accepted via Stripe
- Supported cards: Visa, Mastercard, American Express, Discover
- Automatic monthly billing
- Invoices and receipts available in dashboard

## Configuration Defaults

| Setting | Default Value |
|---------|---------------|
| Trial Purchase Limit | 10 |
| Base Price | $15.00/store |
| Included Purchases | 500/store |
| Tier 1 Rate | $50.00/1K |
| Tier 1 Max | 5,000 |
| Tier 2 Discount Step | 5,000 |
| Tier 2 Discount % | 5% |
| Tier 2 Min Rate | $40.00/1K |
| Grace Period | 3 days |

*Note: These values are configurable by super admins in the admin panel.*
