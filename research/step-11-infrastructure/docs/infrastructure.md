# Step 11: Operational Infrastructure Planning

**Research Date:** December 28, 2025
**Focus:** iOS + Android Portfolio

## Overview

Infrastructure roadmap for scaling from a 2-person team managing 10 apps to a 100-person company with 50 apps.

## Key Metrics

| Metric | Value |
|--------|-------|
| Year 1 monthly infra cost | $109 |
| Per-app cost (Year 1) | $11-22 |
| Tools that stay FREE at any scale | 4 |
| Ad mediation cost (MAX) | $0 |

---

## Infrastructure Scaling Roadmap

### Year 1: Bootstrap
- **Team:** 2 people (solo + iOS eng)
- **Portfolio:** 5-10 apps
- **Focus:** Free tiers, minimal ops
- **Monthly Cost:** $109/mo (~$11-22 per app)

### Year 2: Growth
- **Team:** 5-10 people
- **Portfolio:** 10-25 apps
- **Focus:** Paid tiers, automation
- **Monthly Cost:** $651-1,576/mo (~$26-63 per app)

### Year 3: Scale
- **Team:** 20-100 people
- **Portfolio:** 25-50 apps
- **Focus:** Enterprise, dedicated ops
- **Monthly Cost:** $2,536-4,797/mo (~$51-96 per app)

---

## Recommended Architecture

Shared infrastructure stack for multi-app portfolio management:

| Layer | Tools |
|-------|-------|
| **Analytics** | Firebase Analytics (FREE), Mixpanel/Amplitude, RevenueCat (FREE <$10K) |
| **Monetization** | MAX by AppLovin (FREE), AdMob, Unity Ads |
| **Backend** | Firebase (Spark FREE), Cloud Functions, Firestore |
| **CI/CD** | Fastlane (FREE), GitHub Actions, TestFlight/Play Console |
| **Monitoring** | Firebase Crashlytics (FREE), Sentry (advanced), Firebase Remote Config (FREE) |
| **Operations** | Help Scout ($25/user), ASOdesk ($59+), Linear/Notion |

---

## Tool Recommendations by Category

### Analytics & Revenue Tracking

| Tool | Pricing | Multi-app Score |
|------|---------|-----------------|
| **Firebase Analytics** ⭐ | FREE (unlimited apps, events) | 5/5 |
| Mixpanel | Free: 1M events, $25/mo+ | 4/5 |
| Amplitude | Free: 1M events, $49/mo+ | 4/5 |
| **RevenueCat** ⭐ | Free: <$10K MTR, $250/mo+ | 5/5 |

### Ad Mediation

| Tool | Pricing | Multi-app Score |
|------|---------|-----------------|
| **MAX by AppLovin** ⭐ | FREE (5% fee to advertisers) | 5/5 (60%+ market share) |
| ironSource (Unity) | FREE for publishers | 4/5 (Gaming focus) |
| AdMob Mediation | FREE | 3/5 (Simpler) |

### Customer Support

| Tool | Pricing | Multi-app Score |
|------|---------|-----------------|
| **Help Scout** ⭐ | $25/user (unlimited mailboxes) | 5/5 |
| Freshdesk | Free (10 agents), $15-49/user | 4/5 |
| Zendesk | $55-115/agent | 4/5 (Expensive) |
| Intercom | $29-132/seat + usage | Best for in-app chat |

### Crash Reporting & Monitoring

| Tool | Pricing | Multi-app Score |
|------|---------|-----------------|
| **Firebase Crashlytics** ⭐ | FREE (unlimited) | 5/5 (Industry standard) |
| Sentry | Free tier, $29-89/mo | 4/5 (Advanced) |
| Bugsnag | $59-249/mo | 3/5 |

### Feature Flags & Remote Config

| Tool | Pricing | Multi-app Score |
|------|---------|-----------------|
| **Firebase Remote Config** ⭐ | FREE (unlimited) | 4/5 |
| **Statsig** ⭐ | Free: 1M events, $150/mo | 5/5 |
| LaunchDarkly | $12/connection + MAU | 2/5 (Very expensive) |

### ASO & Review Management

| Tool | Pricing | Multi-app Score |
|------|---------|-----------------|
| **ASOdesk** ⭐ | $59 (5 apps) - $399 (40 apps) | 5/5 (Best value) |
| AppFollow | $97-597/mo by app count | 4/5 (Best features) |
| AppTweak | Custom (~$200-800/mo) | ASO-focused |

### CI/CD for Mobile

| Tool | Pricing | Multi-app Score |
|------|---------|-----------------|
| **Fastlane** ⭐ | FREE (open source) | 5/5 (Self-hosted) |
| **GitHub Actions** ⭐ | 2,000 min free, $0.008/min macOS | 4/5 |
| Bitrise | $89-192/mo, $250/app release | 3/5 (Mobile-focused) |

---

## Detailed Cost Breakdown

### Year 1: Bootstrap (2 people, 5-10 apps)

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
| **TOTAL** | | **$109/month** |

### Year 2: Growth (5-10 people, 10-25 apps)

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
| **TOTAL** | | **$651-1,576/month** |

### Year 3: Scale (20-100 people, 25-50 apps)

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
| **TOTAL** | | **$2,536-4,797/month** |

---

## Key Insights

### Free Tier Winners
These tools scale from 0 to 50 apps without paid upgrades:
- Firebase Analytics - Unlimited apps/events
- Firebase Crashlytics - Unlimited crashes
- MAX by AppLovin - Free mediation (advertisers pay)
- Firebase Remote Config - Unlimited parameters

### Cost Inflection Points
Watch for these thresholds that trigger paid tiers:
- $10K MTR - RevenueCat moves to paid
- 10 apps - ASO tools tier up
- 10 team members - Support costs jump
- 1M events/mo - Analytics hit paid tiers

### Hidden Costs to Watch
Often-overlooked expenses that add up:
- App store fees: $99/yr iOS + $25 Android
- macOS CI builds: 10x more than Linux
- Firebase Blaze: Cloud Functions can spike
- Support seats: Linear scaling with team

### Architecture Recommendation
What to share vs. keep separate:
- **SHARE:** Analytics dashboard, ad account, support inbox, CI/CD
- **SEPARATE:** Firebase projects, app store listings, user DBs
- Use shared Fastlane + GitHub Actions workflows
- Keep Firebase projects isolated for billing clarity

---

## Tools NOT Recommended

Too expensive for early-stage portfolio management:

| Tool | Cost | Reason |
|------|------|--------|
| data.ai (App Annie) | $20,000-50,000+/year | Enterprise-only. Overkill for portfolio management. Consider Year 3+ only if investors require it. |
| Sensor Tower | $499-2,000+/month | Too expensive for early stage. Great competitive intelligence but not worth the cost until scale. |
| LaunchDarkly | $500-2,000+/month at scale | Pricing scales VERY fast with MAU. Use Statsig or Firebase Remote Config instead. |
| Zendesk Suite | $55-115/agent/month | 2-3x more expensive than Help Scout with similar features. Enterprise-focused. |

---

## Tool Migration Path

| Category | Year 1 | Year 2 | Year 3 |
|----------|--------|--------|--------|
| Analytics | Firebase + Mixpanel Free | Firebase + Mixpanel Growth | Firebase + Amplitude Plus |
| Support | Help Scout Standard ($25/user) | Help Scout Plus ($60/user) | Help Scout Plus (6+ users) |
| Crash Reporting | Firebase Crashlytics | Crashlytics + Sentry Team | Sentry Business |
| Feature Flags | Firebase Remote Config | Statsig Free | Statsig Pro |
| ASO/Reviews | ASOdesk Basic ($59) | AppFollow Pro ($297) | AppFollow Business ($597) |
| CI/CD | Fastlane + GitHub Free | GitHub Actions paid | Bitrise Pro or scaled GitHub |
| Subscriptions | RevenueCat Free | RevenueCat Free (if <$10K MTR) | RevenueCat Growth/Scale |

### Annual Cost Summary

| Year | Annual Cost |
|------|-------------|
| Year 1 | $1,308 |
| Year 2 | $7.8K-19K |
| Year 3 | $30K-58K |

> **Note:** Infrastructure costs only. Does not include salaries, app store fees ($99/yr iOS + $25 Android), marketing, or legal costs.

---

## Sources & References

- [Firebase Pricing](https://firebase.google.com/pricing)
- [Mixpanel Pricing](https://mixpanel.com/pricing/)
- [Amplitude Analytics](https://amplitude.com)
- [RevenueCat Pricing](https://www.revenuecat.com/pricing/)
- [AppLovin MAX Business Model](https://www.playwire.com/blog/how-does-applovin-make-money)
- [Help Scout Pricing](https://www.helpscout.com/pricing/)
- [Freshdesk Pricing](https://www.freshworks.com/freshdesk/pricing/)
- [Zendesk Pricing](https://www.zendesk.com/pricing)
- [Sentry Pricing](https://sentry.io/pricing/)
- [Statsig Pricing](https://statsig.com/pricing)
- [LaunchDarkly Pricing](https://launchdarkly.com/pricing/)
- [ASOdesk Pricing](https://asodesk.com)
- [AppFollow Pricing](https://appfollow.io)
- [Bitrise Pricing](https://bitrise.io/pricing)
- [AdMob vs ironSource Comparison](https://www.g2.com/compare/google-admob-vs-ironsource)
- [Top Ad Mediation Platforms](https://www.blog.udonis.co/mobile-marketing/top-ad-mediation-platforms-mobile-apps-games)
