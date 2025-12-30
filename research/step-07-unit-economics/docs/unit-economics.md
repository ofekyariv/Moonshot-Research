# Unit Economics

*Last updated: Step 7 validation (December 2024)*

## Executive Summary

After comprehensive research validation, the unit economics model has been stress-tested with real-world data. Key findings:

- **Development costs:** Aligned with estimates when using offshore/hybrid teams
- **Monetization uplift:** 3-5x realistic (not 10x as originally assumed)
- **Operational costs:** Lower than expected ($125-$400/mo vs $500-$1,200)
- **Payback period:** 9-56 months depending on scenario

---

## Cost Structure

### Per-App Costs (One-Time)

| Item | Low (Offshore) | Mid (Hybrid) | High (US-led) |
|------|----------------|--------------|---------------|
| Native rewrite (iOS) | $15,000 | $25,000 | $40,000 |
| Native rewrite (Android) | $15,000 | $25,000 | $40,000 |
| Design refresh | $3,000 | $8,000 | $15,000 |
| Legal (agreement) | $500 | $700 | $1,000 |
| **Total per app** | **$33,500** | **$58,700** | **$96,000** |

**Development Cost Benchmarks (2024-2025):**
- US freelancers: $50-$150/hr
- Eastern Europe: $40-$90/hr (best value/quality balance)
- India/Southeast Asia: $20-$55/hr
- Simple utility app rewrite: 1-3 months
- Medium complexity app: 3-6 months

*Sources: [Index.dev](https://www.index.dev/blog/freelance-developer-rates-by-country), [Qubit Labs](https://qubit-labs.com/average-hourly-rates-offshore-development-services-software-development-costs-guide/), [CloseLoop](https://closeloop.com/blog/how-much-does-it-cost-to-build-a-mobile-app/)*

### Ongoing Costs (Monthly, Per App)

| Item | Estimate | Notes |
|------|----------|-------|
| Cloud hosting | $25-$100 | Supabase Team or Firebase |
| Analytics | $0 | Amplitude/Mixpanel free tiers (50K MTU) |
| Crash reporting | $0 | Firebase Crashlytics |
| A/B testing | $0 | Firebase Remote Config |
| Ad mediation | $0 | AppLovin MAX, IronSource LevelPlay |
| Maintenance reserve | $100-$300 | Bug fixes, updates |
| **Total** | **$125-$400/mo** | |

*Sources: [Supabase Pricing](https://uibakery.io/blog/supabase-pricing), [Firebase Pricing](https://supertokens.com/blog/firebase-pricing)*

---

## Revenue Model

### Monetization Uplift Benchmarks

| Strategy | Typical Uplift | Source |
|----------|---------------|--------|
| Ad mediation optimization | 70-121% (2x) | Superscale case study |
| Paywall/trial optimization | 150% conversion increase | iDict case study |
| Hybrid monetization (ads + subscription) | 28-121% | AppsFlyer 2024 |
| **Combined realistic uplift** | **3x-5x** | Conservative estimate |

**Key ARPU Benchmarks (Day 90):**
- iOS subscription apps: $8.39
- Android subscription apps: $1.54
- iOS ad-supported: $0.77
- Android ad-supported: $0.35

*Note: iOS generates 5.4x higher subscription ARPU than Android.*

*Sources: [AppsFlyer 2024 Monetization Report](https://www.appsflyer.com/company/newsroom/pr/app-monetization-report/), [Apphud iDict Case Study](https://apphud.com/blog/idict-case-study), [Superscale](https://superscale.com/resources/increase-ad-revenue-instantly-with-these-ad-mediation-changes/)*

### Revenue Scenarios

**Target App Profile: 50K MAU, currently $500/mo**

| Metric | Conservative (3x) | Realistic (5x) | Optimistic (8x) |
|--------|-------------------|----------------|-----------------|
| Post-optimization revenue | $1,500/mo | $2,500/mo | $4,000/mo |
| Moonshot share (50%) | $750/mo | $1,250/mo | $2,000/mo |
| Investment (mid-range) | $58,700 | $58,700 | $58,700 |
| Monthly ops | $200 | $200 | $200 |
| Net monthly | $550/mo | $1,050/mo | $1,800/mo |
| **Payback period** | **107 months** | **56 months** | **33 months** |

**Better Target: 100K MAU, currently $1,000/mo**

| Metric | Conservative (3x) | Realistic (5x) | Optimistic (8x) |
|--------|-------------------|----------------|-----------------|
| Post-optimization revenue | $3,000/mo | $5,000/mo | $8,000/mo |
| Moonshot share (50%) | $1,500/mo | $2,500/mo | $4,000/mo |
| Investment (mid-range) | $58,700 | $58,700 | $58,700 |
| Monthly ops | $200 | $200 | $200 |
| Net monthly | $1,300/mo | $2,300/mo | $3,800/mo |
| **Payback period** | **45 months** | **26 months** | **15 months** |

---

## Stress Test Scenarios

### Pessimistic Scenario
- Development cost: $80K (US-led, scope creep)
- Revenue uplift: 2x (minimal optimization)
- Monthly ops: $400
- Target: 50K MAU app, $500/mo current
- Moonshot net revenue: $100/mo
- **Payback: 800 months - NOT VIABLE**

### Base Case (Revised)
- Development cost: $50K (hybrid team)
- Revenue uplift: 4x
- Monthly ops: $200
- Target: 100K MAU app, $1,000/mo current
- Moonshot net revenue: $1,800/mo
- **Payback: 28 months (2.3 years)**

### Optimistic Scenario
- Development cost: $35K (efficient offshore)
- Revenue uplift: 8x (strong monetization)
- Monthly ops: $125
- Target: 100K MAU app, $1,500/mo current
- Moonshot net revenue: $5,875/mo
- **Payback: 6 months**

---

## Portfolio Model

### Year 1 (Revised)
| Metric | Conservative | Base Case | Optimistic |
|--------|--------------|-----------|------------|
| Apps launched | 3 | 5 | 8 |
| Avg net revenue/app | $1,000/mo | $1,800/mo | $3,000/mo |
| Total monthly revenue (EOY) | $3,000 | $9,000 | $24,000 |
| Total investment | $150,000 | $250,000 | $280,000 |
| Cumulative revenue (Year 1) | $18,000 | $54,000 | $144,000 |

### Year 2 (with compounding)
- Previous apps continue earning
- New apps added (8-12)
- Some apps grow organically
- Revenue compounds as portfolio grows

### Break-Even Analysis

**Fixed monthly costs (team of 2):**
- Salaries: $20,000
- Tools/infra: $500
- Legal/admin: $500
- **Total: $21,000/mo**

**Apps needed to break even:**
- At $1,000 net/app/mo: 21 apps (not realistic Year 1)
- At $2,000 net/app/mo: 11 apps
- At $3,000 net/app/mo: 7 apps

**Implication:** Need to either reduce fixed costs (outsource/bootstrap) or target higher-value apps to reach break-even with fewer partnerships.

---

## Sensitivity Analysis

| Variable | Impact | Mitigation |
|----------|--------|------------|
| Development cost +50% | Payback +50% | Use offshore team, fixed-price contracts |
| Revenue uplift only 2x | Payback doubles | Better app selection, monetization expertise |
| 70/30 split (dev keeps 70%) | Moonshot revenue -40% | Offset with development guarantee |
| MAU declines post-launch | LTV drops significantly | Retention focus in rebuild |
| App store fee increase | Margin compression | Diversify revenue streams |

---

## Revenue Share Benchmarks

| Model | Split | Notes |
|-------|-------|-------|
| App stores (Apple/Google) | 70/30 (dev keeps 70%) | Baseline for self-publishing |
| Gaming publishers | 30-50/50-70 (dev keeps 30-50%) | Includes UA, development |
| SaaS affiliates | 70-80/20-30 (dev keeps 70-80%) | Referral only, no ops |
| **Moonshot target** | **70/30 → 60/40** | Tiered: 70/30 pilot, 65/35 growth, 60/40 at scale |

**Recommendation:** Use tiered structure: 70/30 pilot (developer keeps 70%) → 65/35 growth → 60/40 at scale. 50/50 is ceiling, not target.

*Sources: [Indie Game Revenue Share](https://playfusion.web.id/indie-game-revenue-share/), [Rewardful](https://www.rewardful.com/articles/affiliate-commission-explained)*

---

## Key Metrics to Track

- **CAC (Cost to Acquire App):** Outreach + legal + negotiation time
- **Development Cost:** Hours × rate per app
- **Time to Revenue:** Weeks from start to first optimized monetization
- **Revenue Uplift:** Actual vs baseline revenue improvement
- **LTV per App:** Total expected revenue over partnership lifetime
- **LTV:Investment Ratio:** Target 3:1 or higher over 3 years

---

## Strategic Recommendations

### 1. Target Higher-Value Apps
- **100K+ MAU** (not 15K-50K)
- **$1K-$5K/mo current revenue** (more optimization headroom)
- **iOS-primary** (5.4x higher subscription ARPU)

### 2. Control Development Costs
- Use Eastern Europe developers ($40-$70/hr)
- Fixed-price contracts with clear scope
- Target simple-to-medium complexity apps
- Avoid scope creep with strict MVP definition

### 3. Validate Monetization Before Commitment
- Request current analytics access before partnership
- Estimate uplift potential with benchmarks
- Only proceed if 3x+ uplift appears achievable

### 4. Consider Bootstrap Model
- Reduce fixed costs to $5K-$10K/mo initially
- Use revenue to fund team expansion
- Reach profitability with 3-5 apps instead of 10+

---

## Sources

**Development Costs:**
- [Index.dev Freelance Rates](https://www.index.dev/blog/freelance-developer-rates-by-country)
- [Qubit Labs Offshore Rates](https://qubit-labs.com/average-hourly-rates-offshore-development-services-software-development-costs-guide/)
- [CloseLoop App Cost Guide](https://closeloop.com/blog/how-much-does-it-cost-to-build-a-mobile-app/)

**Monetization:**
- [AppsFlyer 2024 Monetization Report](https://www.appsflyer.com/company/newsroom/pr/app-monetization-report/)
- [Apphud iDict Case Study](https://apphud.com/blog/idict-case-study)
- [Superscale Ad Mediation](https://superscale.com/resources/increase-ad-revenue-instantly-with-these-ad-mediation-changes/)
- [MonetizeMore eCPM Insights](https://www.monetizemore.com/blog/ecpm-insights/)

**Operational Costs:**
- [Supabase Pricing](https://uibakery.io/blog/supabase-pricing)
- [Firebase Pricing](https://supertokens.com/blog/firebase-pricing)
- [Amplitude Pricing](https://userpilot.com/costs/amplitude-pricing/)

**Legal:**
- [ContractsCounsel Costs](https://www.contractscounsel.com/b/operating-agreement-cost)
- [Stripe Atlas vs Clerky](https://www.flowjam.com/blog/stripe-atlas-vs-clerky-which-is-better-for-your-startup)

**Revenue Share:**
- [Indie Game Revenue Share](https://playfusion.web.id/indie-game-revenue-share/)
- [Rewardful Affiliate Guide](https://www.rewardful.com/articles/affiliate-commission-explained)
