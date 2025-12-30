# Technical Stack & Approach

## Native Rewrite Philosophy

### Why Native?
1. **Performance** - Better UX, faster load times, smoother animations
2. **Monetization** - Native ad SDKs perform better
3. **Analytics** - Deeper integration with platform analytics
4. **Maintenance** - Single codebase per platform, no framework updates

### Tradeoffs
- Higher initial cost (two codebases)
- Longer timeline vs cross-platform
- Need expertise in both iOS and Android

---

## Tech Stack

### Android
- **Language:** Kotlin
- **Architecture:** MVVM + Clean Architecture
- **UI:** Jetpack Compose (or XML for simpler apps)
- **DI:** Hilt
- **Networking:** Retrofit + OkHttp
- **Local storage:** Room
- **Analytics:** Firebase Analytics, Mixpanel
- **Ads:** AdMob, ironSource, Unity Ads
- **Crash reporting:** Firebase Crashlytics

### iOS
- **Language:** Swift
- **Architecture:** MVVM + Combine
- **UI:** SwiftUI (or UIKit for compatibility)
- **Networking:** URLSession / Alamofire
- **Local storage:** Core Data / SwiftData
- **Analytics:** Firebase Analytics, Mixpanel
- **Ads:** AdMob, ironSource
- **Crash reporting:** Firebase Crashlytics

### Backend (if needed)
- **Simple:** Firebase (Auth, Firestore, Functions)
- **Complex:** Node.js or Python on AWS/GCP
- **Payments:** RevenueCat for subscriptions

---

## Rewrite Process

### Phase 1: Assessment (Week 1)
- [ ] Analyze existing codebase
- [ ] Document all features
- [ ] Identify third-party dependencies
- [ ] Estimate effort per feature

### Phase 2: Core Build (Weeks 2-5)
- [ ] Set up project structure
- [ ] Implement core features
- [ ] Integrate analytics from day 1
- [ ] Basic UI implementation

### Phase 3: Polish & Monetization (Weeks 6-7)
- [ ] UI/UX refinements
- [ ] Ad integration
- [ ] Subscription/IAP setup
- [ ] Performance optimization

### Phase 4: Launch (Week 8)
- [ ] Beta testing
- [ ] App store submission
- [ ] Gradual rollout
- [ ] Monitor metrics

---

## Tooling
- **Project management:** Linear, Notion
- **Design:** Figma
- **CI/CD:** Fastlane, GitHub Actions
- **App distribution:** TestFlight, Firebase App Distribution

---

## Shared Infrastructure (Multi-App Portfolio)

### Scaling Context

| Year | Team Size | Portfolio Size | Infra Focus |
|------|-----------|----------------|-------------|
| 1 | 2 (solo + iOS eng) | 5-10 apps | Free tiers, minimal ops |
| 2 | 5-10 people | 10-25 apps | Paid tiers, automation |
| 3 | 20-100 people | 25-50 apps | Enterprise, dedicated ops |

---

### Analytics Layer

| Tool | Pricing | Multi-App Score | Recommendation |
|------|---------|-----------------|----------------|
| **Firebase Analytics** | FREE (unlimited) | ⭐⭐⭐⭐⭐ | Year 1-3: Essential backbone |
| **Mixpanel** | Free: 1M events/mo, Growth: $25/mo | ⭐⭐⭐⭐ | Year 1-2: Behavioral analytics |
| **Amplitude** | Free: 1M events/mo, Plus: $49/mo | ⭐⭐⭐⭐ | Alternative to Mixpanel |
| **RevenueCat** | Free: <$10K MTR, Growth: $250/mo | ⭐⭐⭐⭐⭐ | Essential for subscriptions |

**Recommendation:** Firebase (all apps) + Mixpanel/Amplitude (behavioral) + RevenueCat (subscriptions)

---

### Ad Mediation

| Platform | Pricing | Multi-App Score | Notes |
|----------|---------|-----------------|-------|
| **MAX (AppLovin)** | FREE for publishers | ⭐⭐⭐⭐⭐ | 5% fee charged to advertisers, not you |
| **ironSource (Unity)** | FREE for publishers | ⭐⭐⭐⭐ | Strong gaming focus |
| **AdMob Mediation** | FREE | ⭐⭐⭐ | Simpler but less advanced |

**Recommendation:** MAX by AppLovin - free, 60%+ market share, best eCPM optimization

---

### Backend-as-a-Service

| Tool | Free Tier | Paid Pricing | Multi-App Score |
|------|-----------|--------------|-----------------|
| **Firebase** | Generous (Spark plan) | Pay-as-you-go (Blaze) | ⭐⭐⭐⭐⭐ |
| **Supabase** | 2 projects, 500MB | $25/project/mo | ⭐⭐⭐ |
| **AWS Amplify** | 12 months free tier | Pay-as-you-go | ⭐⭐⭐ |

**Recommendation:** Firebase for most apps - unlimited projects, excellent free tier, integrated with analytics

---

### CI/CD for Mobile

| Tool | Free Tier | Paid Plans | Multi-App Score |
|------|-----------|------------|-----------------|
| **Fastlane** | FREE (open source) | Self-hosted | ⭐⭐⭐⭐⭐ |
| **GitHub Actions** | 2,000 min/mo free | $0.008/min (macOS) | ⭐⭐⭐⭐ |
| **Bitrise** | 300 credits/mo, 1 app | $89-192/mo | ⭐⭐⭐ |

**Recommendation:** Fastlane + GitHub Actions for cost efficiency. Bitrise if dedicated mobile CI needed.

---

### Customer Support

| Tool | Pricing (per user/mo) | Multi-Brand | Recommendation |
|------|----------------------|-------------|----------------|
| **Help Scout** | $25 Standard, $60 Plus | ✅ Unlimited mailboxes | ⭐ BEST VALUE Year 1-3 |
| **Freshdesk** | Free (10 agents), $15-49 paid | ✅ Growth+ plans | Good alternative |
| **Zendesk** | $55-115 | ✅ Growth+ plans | Expensive, enterprise |
| **Intercom** | $29-132 + usage | ⚠️ Limited | Best for in-app chat |

**Recommendation:** Help Scout ($100-240/mo for 4 users) - unlimited mailboxes perfect for app portfolio

---

### Crash Reporting & Monitoring

| Tool | Pricing | Multi-App Score | Notes |
|------|---------|-----------------|-------|
| **Firebase Crashlytics** | FREE (unlimited) | ⭐⭐⭐⭐⭐ | Industry standard |
| **Sentry** | Free tier, $29-89/mo | ⭐⭐⭐⭐ | Advanced error tracking |
| **Bugsnag** | $59-249/mo | ⭐⭐⭐ | Similar to Sentry |

**Recommendation:** Firebase Crashlytics (all apps) + Sentry (if advanced debugging needed)

---

### Feature Flags & Remote Config

| Tool | Free Tier | Paid Plans | Multi-App Score |
|------|-----------|------------|-----------------|
| **Firebase Remote Config** | FREE (unlimited) | N/A | ⭐⭐⭐⭐ |
| **Statsig** | 1M events/mo | $150/mo (10M events) | ⭐⭐⭐⭐⭐ |
| **LaunchDarkly** | 1K MAU | $12/connection + MAU | ⭐⭐ (expensive at scale) |

**Recommendation:** Firebase Remote Config (basic) or Statsig (advanced) - both have generous free tiers

---

### ASO & Review Management

| Tool | Pricing | Multi-App Score | Notes |
|------|---------|-----------------|-------|
| **ASOdesk** | $59 (5 apps) - $399 (40 apps) | ⭐⭐⭐⭐⭐ | Best value |
| **AppFollow** | $97-597/mo by app count | ⭐⭐⭐⭐ | Best features |
| **AppTweak** | Custom (~$200-800/mo) | ⭐⭐⭐ | ASO-focused |

**Recommendation:** ASOdesk for Year 1-2 ($59-179/mo), AppFollow for Year 3+

---

## Cost Estimates by Year

### Year 1: Bootstrap (2 people, 5-10 apps)
**Target: $0-250/month infrastructure**

| Category | Tool | Monthly Cost |
|----------|------|--------------|
| Analytics | Firebase + Mixpanel Free | $0 |
| Ads | MAX by AppLovin | $0 |
| Backend | Firebase Spark | $0 |
| CI/CD | Fastlane + GitHub Actions | $0 |
| Support | Help Scout (2 users) | $50 |
| Crashes | Firebase Crashlytics | $0 |
| Feature Flags | Firebase Remote Config | $0 |
| ASO/Reviews | ASOdesk Basic | $59 |
| Subscriptions | RevenueCat Free | $0 |
| **Total** | | **$109/month** |

**Per-app cost: ~$11-22/month**

---

### Year 2: Growth (5-10 people, 10-25 apps)
**Target: $500-1,000/month infrastructure**

| Category | Tool | Monthly Cost |
|----------|------|--------------|
| Analytics | Firebase + Mixpanel Growth | $25-50 |
| Ads | MAX by AppLovin | $0 |
| Backend | Firebase Blaze (usage-based) | $50-200 |
| CI/CD | GitHub Actions (paid tier) | $50-100 |
| Support | Help Scout (4 users) | $100-240 |
| Crashes | Sentry Team | $29-89 |
| Feature Flags | Statsig Free/Pro | $0-150 |
| ASO/Reviews | AppFollow Professional | $297 |
| Subscriptions | RevenueCat (if >$10K MTR) | $0-250 |
| Team Tools | Slack, Linear, Figma | $100-200 |
| **Total** | | **$651-1,576/month** |

**Per-app cost: ~$26-63/month**

---

### Year 3: Scale (20-100 people, 25-50 apps)
**Target: $2,000-5,000/month infrastructure**

| Category | Tool | Monthly Cost |
|----------|------|--------------|
| Analytics | Firebase + Amplitude Plus | $50-100 |
| Ads | MAX by AppLovin | $0 |
| Backend | Firebase Blaze + potential AWS | $200-500 |
| CI/CD | Bitrise Pro or scaled GitHub | $200-500 |
| Support | Help Scout (8+ users) | $400-800 |
| Crashes | Sentry Business | $89-200 |
| Feature Flags | Statsig Pro | $150-300 |
| ASO/Reviews | AppFollow Business | $597 |
| Subscriptions | RevenueCat Scale | $250-500 |
| Monitoring | PagerDuty/OpsGenie | $100-300 |
| Team Tools | Slack, Linear, Figma (team) | $500-1,000 |
| **Total** | | **$2,536-4,797/month** |

**Per-app cost: ~$51-96/month**

---

## Key Insights

### Free Tier Winners
These tools scale from 0 to 50 apps without requiring paid upgrades:
- **Firebase Analytics** - Unlimited apps, unlimited events
- **Firebase Crashlytics** - Unlimited crashes
- **MAX by AppLovin** - Free ad mediation (they charge advertisers)
- **Firebase Remote Config** - Unlimited parameters

### Cost Scaling Inflection Points
1. **$10K MTR** - RevenueCat moves from free to paid
2. **10 apps** - ASOdesk/AppFollow tier increases
3. **10 team members** - Support and collaboration tools increase
4. **1M events/mo** - Analytics platforms hit paid tiers

### Hidden Costs to Watch
- **App store fees:** $99/year iOS + $25 one-time Android per account
- **CI/CD macOS builds:** 10x more expensive than Linux
- **Firebase Blaze:** Usage-based can spike with Cloud Functions
- **Support tool seats:** Costs scale linearly with team size

### Architecture Recommendations

**Shared vs Per-App:**
- ✅ **Shared:** Analytics dashboard, Ad mediation account, Support inbox, CI/CD pipelines
- ❌ **Per-App:** Firebase projects, App store listings, User databases

**Multi-Tenant Considerations:**
- Keep Firebase projects separate per app (easier billing, isolation)
- Use shared dashboards for cross-portfolio visibility
- Centralize CI/CD with Fastlane + shared GitHub Actions workflows

---

## Tools NOT Recommended (Too Expensive)

### App Intelligence Platforms
These are designed for enterprise - skip until Year 3+ if investor reporting requires it:

| Tool | Pricing | Why Skip |
|------|---------|----------|
| **data.ai (App Annie)** | $20,000-50,000+/year | Enterprise-only, overkill for portfolio management |
| **Sensor Tower** | $499-2,000+/month | Too expensive for early stage |
| **Apptopia** | Custom enterprise | Same as above |
| **SimilarWeb Mobile** | $125-500+/month | Better for web; mobile features limited |

### Expensive Feature Flags
| Tool | Why Skip |
|------|----------|
| **LaunchDarkly** | Pricing scales VERY fast: $500-2,000/mo easily at scale |
| **Split.io** | Enterprise-focused, similar to LaunchDarkly |

---

## Tool Migration Path

| Category | Year 1 | Year 2 | Year 3 |
|----------|--------|--------|--------|
| Analytics | Firebase + Mixpanel Free | Firebase + Mixpanel Growth | Firebase + Amplitude Plus |
| Behavioral | Mixpanel Free (1M events) | Mixpanel Growth ($25/mo) | Amplitude Plus ($49/mo) |
| Support | Help Scout Standard ($25/user) | Help Scout Plus ($60/user) | Help Scout Plus (6+ users) |
| Crashes | Firebase Crashlytics | Crashlytics + Sentry Team | Sentry Business |
| Feature Flags | Firebase Remote Config | Statsig Free | Statsig Pro |
| ASO/Reviews | ASOdesk Basic ($59) | AppFollow Pro ($297) | AppFollow Business ($597) |
| CI/CD | Fastlane + GitHub Free | GitHub Actions paid | Bitrise Pro or scaled GitHub |
| Subscriptions | RevenueCat Free | RevenueCat Free/<$10K | RevenueCat Growth/Scale |

---

## Annual Cost Summary

| Year | Monthly | Annual | Per-App (Monthly) |
|------|---------|--------|-------------------|
| 1 | $109 | $1,308 | $11-22 |
| 2 | $651-1,576 | $7,812-18,912 | $26-63 |
| 3 | $2,536-4,797 | $30,432-57,564 | $51-96 |

**Note:** These are infrastructure costs only. Does not include:
- Salaries/contractors
- App store fees ($99/yr iOS + $25 Android)
- Marketing/UA spend
- Legal costs (see Step 10)