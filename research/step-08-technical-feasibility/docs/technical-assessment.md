# Technical Assessment Framework

A structured framework for evaluating indie app partnerships based on technical complexity and rebuild feasibility.

---

## Complexity Tiers

Moonshot uses a tiered approach to estimate rebuild timelines based on app complexity.

### Tier 1: Simple Apps (6-8 weeks)
**Primary Target for Moonshot**

**Characteristics:**
- 5-10 screens
- 1-3 core features
- Basic CRUD operations
- Standard UI patterns (no custom animations)
- BaaS-compatible backend (Firebase, Supabase)
- Single platform (iOS or Android)
- No compliance requirements

**Examples:**
- Habit trackers
- Simple expense trackers
- Focus/productivity timers
- Flashcard apps
- Unit converters
- Basic calculators with history

**Development Breakdown:**
| Phase | Timeline |
|-------|----------|
| Planning & Setup | 1 week |
| Core Development | 3-4 weeks |
| Polish & Integration | 1-2 weeks |
| Testing & Submission | 1 week |

---

### Tier 2: Medium Apps (10-12 weeks)
**Selective - Requires Careful Scoping**

**Characteristics:**
- 10-25 screens
- 3-5 core features
- API integrations
- In-app purchases or subscriptions
- Basic geolocation or push notifications
- User profiles and settings
- Moderate backend complexity

**Examples:**
- Fitness trackers (simple workout library)
- Recipe apps (provided database)
- Journal/diary apps (text-only)
- Budget trackers with reports

**Development Breakdown:**
| Phase | Timeline |
|-------|----------|
| Planning & Setup | 1-2 weeks |
| Core Development | 5-7 weeks |
| Polish & Integration | 2-3 weeks |
| Testing & Submission | 1-2 weeks |

---

### Tier 3: Complex Apps (16+ weeks)
**Avoid - Outside Moonshot's Target**

**Characteristics:**
- 25+ screens
- 5+ features with interdependencies
- Real-time synchronization
- Custom backend systems
- Video/audio processing
- Social networking features
- Compliance requirements (HIPAA, PCI)

**Examples:**
- Social networks
- Marketplace apps
- Media editing apps
- Real-time collaboration tools
- Healthcare/fintech apps

**Recommendation:** Decline partnership or negotiate extended timeline and higher investment.

---

## Complexity Scorecard

Use this 8-point scorecard to objectively assess app complexity. Each criterion scores 1-5.

### Scoring Instructions
Rate each criterion on a 1-5 scale, then sum for total score.

| # | Criterion | 1 (Simple) | 3 (Medium) | 5 (Complex) |
|---|-----------|------------|------------|-------------|
| 1 | **Core Features** | 1-2 features | 3-5 features | 6+ features |
| 2 | **Backend Complexity** | BaaS (Firebase) | REST API integration | Custom microservices |
| 3 | **Data Model** | Simple CRUD | Relational (3-5 tables) | Complex relationships |
| 4 | **UI Complexity** | Standard patterns | Custom components | Heavy animations |
| 5 | **Third-Party Integrations** | 0-1 | 2-3 | 4+ |
| 6 | **User Base Size** | <10K MAU | 10K-50K MAU | >50K MAU |
| 7 | **Compliance Requirements** | None | Basic privacy | HIPAA/PCI/COPPA |
| 8 | **Migration Complexity** | Greenfield | Data export needed | Complex data migration |

### Score Interpretation

| Total Score | Tier | Timeline | Recommendation |
|-------------|------|----------|----------------|
| **8-16** | Tier 1 | 6-8 weeks | Proceed - ideal fit |
| **17-24** | Tier 2 | 10-12 weeks | Caution - scope aggressively |
| **25-32** | Tier 3 | 16+ weeks | Consider declining |
| **33-40** | - | - | Reject - too complex |

---

## Scope Boundaries

### Must Include (MVP)
Essential for any rebuild:
- [ ] User authentication (email/OAuth)
- [ ] Core value feature (#1 reason users use the app)
- [ ] Basic data persistence (cloud sync)
- [ ] Crash reporting (Crashlytics)
- [ ] Basic analytics (screen views, key events)
- [ ] App Store/Play Store compliance

### Should Include (If Time Allows)
Important but can ship without:
- [ ] Push notifications
- [ ] Settings screen
- [ ] Onboarding (2-3 screens)
- [ ] Basic error states
- [ ] Loading states
- [ ] Empty states

### Could Include (Phase 2)
Defer to post-launch:
- [ ] Advanced analytics dashboards
- [ ] Social sharing
- [ ] Advanced search/filtering
- [ ] Export data feature
- [ ] Multiple themes
- [ ] Internationalization (i18n)

### Won't Include (Out of Scope)
Reject apps requiring these, or defer indefinitely:
- [ ] Real-time collaboration
- [ ] Video/audio processing
- [ ] UGC with moderation
- [ ] Offline-first with sync
- [ ] Custom mapping/routing
- [ ] AI/ML custom models

---

## Red Flag Features

**Automatic Rejection Criteria**

If an app contains any of these features, it exceeds the 8-week timeline:

| Red Flag | Why It's Complex | Typical Timeline Impact |
|----------|------------------|------------------------|
| **Real-time multiplayer** | WebSocket infrastructure, state sync, conflict resolution | +6-8 weeks |
| **User-generated content moderation** | Content review, abuse prevention, legal liability | +4-6 weeks |
| **Custom video/photo editing** | Media processing, filters, rendering | +8-12 weeks |
| **Offline-first architecture** | Local database, sync engine, conflict resolution | +3-4 weeks |
| **Social networking features** | Profiles, feeds, following, activity streams | +6-8 weeks |
| **Complex e-commerce/marketplace** | Multi-vendor, inventory, orders, disputes | +8-12 weeks |
| **Custom maps/geolocation** | Routing, geofencing, real-time tracking | +4-6 weeks |
| **Blockchain/crypto** | Wallet integration, security, regulatory | +6-10 weeks |
| **HIPAA/PCI/COPPA compliance** | Security audits, legal review, testing | +3-6 weeks |
| **Multi-tenant SaaS** | Tenant isolation, per-tenant customization | +4-6 weeks |

---

## App Archetype Guide

### Accept (Tier 1 - Primary Targets)

| App Type | Why It Works | Timeline |
|----------|--------------|----------|
| **Habit Trackers** | Simple CRUD, streak logic, minimal backend | 6-7 weeks |
| **Expense Trackers** | Data entry + categories, local-first | 7-8 weeks |
| **Focus Timers** | Timer logic, session logging, minimal UI | 5-6 weeks |
| **Flashcard Apps** | Card decks, spaced repetition algorithm | 6-8 weeks |
| **Simple Utilities** | Calculators, converters, reference tools | 4-6 weeks |
| **Educational Quizzes** | Question database, progress tracking | 6-8 weeks |

### Caution (Tier 2 - Selective)

| App Type | Complexity Concerns | Recommendation |
|----------|---------------------|----------------|
| **Fitness Trackers** | Custom exercise builder adds complexity | Accept if workout library is static |
| **Recipe Apps** | UGC requires moderation | Accept if recipe database is provided |
| **Journal Apps** | Rich media (photos, voice) adds time | Accept if text-only |
| **Budget Apps** | Bank integrations are complex | Accept if manual entry only |

### Avoid (Tier 3 - Decline)

| App Type | Why to Decline |
|----------|----------------|
| **Social Networks** | Profiles, feeds, messaging = 12-16+ weeks |
| **Marketplaces** | Multi-vendor, payments, disputes = 12-20+ weeks |
| **Media Editors** | Video/photo processing = 16-24+ weeks |
| **Collaboration Tools** | Real-time sync = 12-18+ weeks |
| **Dating Apps** | Matching, chat, moderation = 12-16+ weeks |

---

## Tech Stack Recommendations

For maximum speed within 8-week timeline:

### Cross-Platform Framework
| Option | When to Use | Timeline Impact |
|--------|-------------|-----------------|
| **Flutter** | Greenfield, team knows Dart | Fastest for both platforms |
| **React Native** | Team knows React | Good ecosystem |
| **Native (Swift/Kotlin)** | Single platform, or existing codebase | Best performance |

### Backend-as-a-Service (BaaS)
| Option | Best For | Features |
|--------|----------|----------|
| **Firebase** | Quick prototyping, Google ecosystem | Auth, Firestore, Storage, Functions |
| **Supabase** | PostgreSQL needs, open-source preference | Auth, Database, Storage, Edge Functions |
| **AWS Amplify** | Already in AWS ecosystem | Full AWS integration |

**Avoid custom backend unless:**
- Existing backend is well-documented and reusable
- App has unique requirements BaaS can't handle
- Timeline is 12+ weeks

### Monetization
| Tool | Use Case |
|------|----------|
| **RevenueCat** | Subscriptions (simplifies IAP) |
| **Stripe** | One-time payments, paywalls |
| **AdMob** | Banner/interstitial ads |

### Analytics & Crash Reporting
| Tool | Use Case |
|------|----------|
| **Firebase Analytics** | Free, integrates with other Firebase |
| **Mixpanel** | Better event tracking and funnels |
| **Firebase Crashlytics** | Free crash reporting |

---

## Assessment Checklist

Use this checklist during initial app evaluation:

### Technical Due Diligence
- [ ] Reviewed app in App Store / Play Store
- [ ] Counted screens (target: <10)
- [ ] Identified core features (target: 1-3)
- [ ] Checked for red flag features
- [ ] Assessed backend complexity
- [ ] Checked for compliance requirements
- [ ] Evaluated data migration needs
- [ ] Calculated complexity score

### Developer Discussion Points
- [ ] Understand current tech stack
- [ ] Access to existing codebase (read-only for reference)
- [ ] Analytics access (identify high-engagement features)
- [ ] User data export requirements
- [ ] Feature priorities (what can be cut?)
- [ ] Platform priorities (iOS first? Android first?)

### Go/No-Go Decision
- [ ] Complexity score is 16 or below (Tier 1)
- [ ] No red flag features present
- [ ] Developer agrees to scope constraints
- [ ] Monetization opportunity is clear
- [ ] Timeline expectations are aligned

---

## Timeline Templates

### Tier 1 App (8-Week Sprint)
```
Week 1: Setup & Architecture
- Project setup, CI/CD, design system
- Authentication integration
- Database schema design

Week 2-3: Core Feature Development
- Primary user workflow
- Data persistence
- Basic UI implementation

Week 4-5: Secondary Features
- Settings, profile
- Additional workflows
- Analytics integration

Week 6: Monetization & Polish
- Payment/subscription integration
- Ad placement
- UI refinements

Week 7: Testing & QA
- Bug fixes
- Performance optimization
- Beta testing

Week 8: Launch
- App Store submission
- Gradual rollout
- Monitoring setup
```

### Tier 2 App (12-Week Sprint)
```
Weeks 1-2: Discovery & Setup
Weeks 3-6: Core Development
Weeks 7-9: Secondary Features
Weeks 10-11: Polish & Testing
Week 12: Launch
```

---

*Last updated: December 2025*
*Sources: Agency timeline research, Dashlane case study, industry complexity frameworks*
