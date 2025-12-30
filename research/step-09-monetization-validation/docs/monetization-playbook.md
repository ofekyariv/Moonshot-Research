# Monetization Playbook

*Updated December 2025 based on Step 9 research. See [step9-monetization-validation.html](step9-monetization-validation.html) for full validation report.*

---

## Executive Summary

**H4 Validated:** 10x monetization improvement is achievable for under-monetized indie apps through multi-vector optimization.

| Strategy | Impact | Timeline |
|----------|--------|----------|
| Model shift (ad-only → hybrid) | 3-8x | Immediate |
| Conversion optimization | 1.5-3x | 1-3 months |
| Pricing optimization | 1.3-2x | 1 month |
| Ad network optimization | 2-3x | 1-2 months |
| **Combined (compounding)** | **9-15x** | **6-12 months** |

---

## ARPU Benchmarks by Category

### Target Categories (Non-Gaming)

| Category | Ad-Only ARPU | Subscription ARPU | Gap |
|----------|--------------|-------------------|-----|
| Utilities | $0.10-0.50/mo | $3-8/mo | 6-16x |
| Education | $0.50-2.00/mo | $10-25/mo | 5-20x |
| Lifestyle/Wellness | $0.25-1.50/mo | $8-20/mo | 5-32x |
| Productivity | $1-5/mo | $20-30/mo | 4-20x |

### Revenue per 1,000 MAU (Monthly)

| Model | Revenue | Notes |
|-------|---------|-------|
| Ad-only (poor) | $50-90 | Banner + minimal interstitials |
| Freemium | $130 | 2.6% conversion |
| Subscription | $500-1,000 | 5% conversion @ $10/mo |
| Hybrid (optimal) | $600-1,200 | Ads for free tier + 5% subscription |

---

## Revenue Streams

### 1. Advertising

**Best for:** High DAU, utility apps, free tier users

#### eCPM Benchmarks (US, 2024-2025)

| Ad Type | iOS | Android | When to Use |
|---------|-----|---------|-------------|
| Rewarded Video | $13.81 | $12.91 | User-initiated, best UX + revenue |
| Interstitial | $9.58 | $11.06 | After task completion only |
| Native | $6-9 | $5-8 | Content feeds, blended |
| Banner | $0.27-1.90 | $0.60-1.62 | Persistent, low impact |
| App Open | $7.35-10.51 | $6-9 | App launch |

#### Ad Network Recommendations

**Primary:** AdMob (Google)
- Best baseline, Firebase integration, reliable fill rates
- Free to use, excellent documentation

**Mediation (choose one):**
- AppLovin MAX - Best for revenue maximization (10-25% lift via bidding)
- ironSource LevelPlay - Good for apps with gamified elements

**Avoid for non-gaming:**
- Unity Ads (gaming-focused advertisers)
- Meta Audience Network (quality issues, high accidental clicks)

#### Recommended Stack

1. **Month 1-2:** AdMob only, 2-3 formats
2. **Month 3-4:** Add AppLovin MAX bidding adapter (+15-25% lift)
3. **Month 5+:** Full mediation with 3-5 networks (+25-35% lift)

#### Best Practices

- **Frequency cap:** 1 interstitial per 3-5 min, max 3-4 per session
- **First session:** No ads in first 2-3 opens
- **Rewarded video:** No hard limit (user-initiated), 5-10 daily cap
- **Fill rate target:** 85%+ with mediation
- **Retention tolerance:** Accept 2-3% D7 drop for monetization

---

### 2. Subscriptions

**Best for:** Apps with ongoing value, premium features, habit-forming apps

#### Pricing Benchmarks (2024-2025)

| Tier | Monthly | Annual | Notes |
|------|---------|--------|-------|
| Standard | $9.99 | $29.99 | Industry standard |
| Premium | $14.99-19.99 | $49.99-79.99 | Feature-rich apps |
| Budget | $4.99 | $19.99 | Price-sensitive markets |

**Discount strategy:** 40-60% off annual (2 months free is common)

#### Conversion Benchmarks

| Metric | Target | Top Performers |
|--------|--------|----------------|
| Download-to-paid | 1.7% (global avg) | 5-10% |
| Trial-to-paid (opt-in) | 17-18% | 25%+ |
| Trial-to-paid (opt-out) | 48-51% | 60%+ |
| Freemium-to-paid | 2.6% | 5%+ |

**By category:**
- Education: 24.8% trial-to-paid (highest)
- Health/Fitness: 9.4% download-to-paid
- Productivity: 29% trial-to-paid

#### Trial Strategy

| Length | Conversion | Best For |
|--------|------------|----------|
| 3-day | Lower | Quick-value utilities |
| 7-day | **79%** (highest) | Most apps |
| 14-day | Moderate | Complex/learning apps |
| 17-32 day | 48.8% | B2B/productivity |

**Key insight:** Opt-out trials (card required) convert 2.8x better than opt-in.

#### Churn Benchmarks

| Rating | Monthly Churn | Annual Churn |
|--------|---------------|--------------|
| Exceptional | <1.5% | <15% |
| Manageable | 3-5% | 31-46% |
| Concerning | >7% | >60% |

**Median:** 4.1% monthly churn (95.9% retention)

#### Subscription Tools

- **RevenueCat** - Industry standard, cross-platform
- **Apphud** - Good for paywall optimization
- **Adapty** - Strong A/B testing for paywalls

---

### 3. Hybrid Model (Recommended)

**Best for:** Maximizing total revenue across all users

#### Strategy

1. **Free tier:** Ad-supported (rewarded video + native)
2. **Paid tier:** Ad-free + premium features
3. **Result:** Monetize 100% of users

#### Expected Lift

- 20-40% higher total revenue vs subscription-only
- Monetizes users who will never pay
- Lower barrier to entry increases user base

---

### 4. In-App Purchases (IAP)

**Best for:** One-time unlocks, cosmetics, consumables

| Type | Examples | Pricing |
|------|----------|---------|
| Pro unlock | Remove ads, all features | $4.99-9.99 (one-time) |
| Themes/cosmetics | Custom themes, icons | $0.99-2.99 |
| Consumables | Credits, coins | $0.99-4.99 (recurring) |
| Tip jar | Support the developer | $0.99-4.99 |

---

## Category-Specific Strategies

### Utilities (VPN, Scanner, Tools)

**Primary:** Interstitial after task completion
**Secondary:** Banner during usage
**Optional:** Rewarded for premium feature unlock
**Subscription:** $3-8/month for pro tier

### Education (Language, Courses)

**Primary:** Rewarded video for hints/extra content
**Secondary:** Native ads between lessons
**Avoid:** Aggressive interstitials during learning
**Subscription:** $10-25/month (highest ARPU category)

### Lifestyle/Wellness (Fitness, Meditation)

**Primary:** Rewarded video for workouts/sessions
**Secondary:** Native ads in content browse
**Subscription:** $8-20/month, annual pricing works well

### Productivity (Notes, To-Do)

**Primary:** Native ads in list views
**Secondary:** Non-intrusive banners
**Avoid:** Interrupting workflow
**Subscription:** $5-15/month consumer, $20-30 premium

---

## 10x Optimization Path

### Phase 1: Foundation (Month 1-2)

1. Implement AdMob with 2-3 ad formats
2. Add RevenueCat for subscription management
3. Create freemium tier with 3-5 premium features
4. Set pricing: $9.99/month, $29.99/year
5. Measure baseline: ARPDAU, conversion, retention

### Phase 2: Optimize (Month 3-6)

1. Add mediation (AppLovin MAX)
2. Implement 7-day opt-out trial
3. A/B test paywall timing (day 3-7)
4. Add rewarded video for free users
5. Implement dynamic floor pricing for ads

### Phase 3: Scale (Month 6-12)

1. Expand to 5+ mediation partners
2. Add tiered subscription pricing
3. Implement localized pricing
4. User segmentation for personalized ad loads
5. Win-back campaigns for churned users

### Expected Results

| Metric | Baseline | After 6 Months | After 12 Months |
|--------|----------|----------------|-----------------|
| ARPDAU | $0.02-0.03 | $0.08-0.15 | $0.15-0.30 |
| Conversion | 1-2% | 3-5% | 5-8% |
| Monthly churn | 8-10% | 5-7% | 3-5% |
| **Total improvement** | 1x | 3-5x | 7-12x |

---

## Key Metrics to Track

| Metric | Description | Target |
|--------|-------------|--------|
| ARPDAU | Revenue per daily active user | $0.10-0.30 |
| ARPU | Revenue per user (monthly) | $2-10 |
| CVR | Free-to-paid conversion | 5%+ |
| Trial CVR | Trial-to-paid conversion | 40%+ (opt-out) |
| Monthly churn | Subscription cancellation rate | <5% |
| eCPM | Ad revenue per 1,000 impressions | $8-15 (blended) |
| Fill rate | Ad requests filled | 85%+ |
| LTV:CAC | Lifetime value vs acquisition cost | 3:1+ |

---

## Case Study Evidence

| App | Category | Improvement | Strategy | Timeline |
|-----|----------|-------------|----------|----------|
| Uplens | Photo Editor | 10x | Paywall + win-back + analytics | 9 months |
| PlantMe | Lifestyle | 5x | Subscription analytics | 6 months |
| Toss | Fintech | 3x | Native + interstitial ads | 12 months |
| Keiki World | Education | 3.1x | ASO + localization | 12 months |
| Duolingo | Education | 2x | Mediation + bidding | 5 years |
| Breezometer | Utility | 2.1x | Ad network switch | Immediate |

*See [step9-monetization-validation.html](step9-monetization-validation.html) for 14 full case studies.*

---

## Sources

- [RevenueCat State of Subscription Apps 2024](https://www.revenuecat.com/state-of-subscription-apps-2024/)
- [Business of Apps: App Pricing Benchmarks](https://www.businessofapps.com/data/app-pricing/)
- [Adapty: App Subscription Pricing Index](https://adapty.io/app-subscription-pricing-index/)
- [Udonis: eCPM Benchmarks](https://www.blog.udonis.co/mobile-marketing/mobile-apps/ecpms)
- [FirstPageSage: Trial Conversion Benchmarks](https://firstpagesage.com/seo-blog/saas-free-trial-conversion-rate-benchmarks/)
- [Chargebee: Churn Benchmarks](https://www.chargebee.com/blog/churn-benchmarks-churn-rate-retention-strategies/)
