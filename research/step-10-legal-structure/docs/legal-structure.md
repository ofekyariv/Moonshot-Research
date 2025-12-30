# Legal Structure & Agreements

*Research completed December 2025. See [step10-legal-structure.html](step10-legal-structure.html) for full visual report.*

---

## Executive Summary

- **Revenue Split:** Tiered: 70/30 pilot → 65/35 growth → 60/40 at scale (developer keeps majority)
- **Entity:** Delaware LLC recommended ($300 filing + $90/year)
- **IP Model:** Dual ownership with cross-licenses (developer keeps original, Moonshot owns new code)
- **Legal Costs Year 1:** ~$2,400 (DIY via Rocket Lawyer + occasional attorney review)
- **International:** Use Deel/Remote.com ($49/month) for compliance

---

## Revenue Share Terms

### Recommended Split
| Phase | Developer | Moonshot | Rationale |
|-------|-----------|----------|-----------|
| Pilot (first 3-5 deals) | 70% | 30% | Attract early adopters, build trust |
| Growth | 65% | 35% | After proving 2x revenue improvement |
| Scale | 60% | 40% | Mature partnerships with track record |
| High-value apps (500K+ users) | 70% | 30% | Competitive deals; lower % on larger base |

### Industry Benchmarks
- **Patreon:** 80-95% to creator (low-touch)
- **YouTube:** 55% to creator (full platform)
- **Indie Game Publishers:** 70% to developer (marketing, QA)
- **Full-Service Publishers:** 50% to developer (porting, localization, marketing)

### Net Revenue Definition
Revenue share calculated on **proceeds actually received** after:
- Platform fees (Apple/Google 15-30%)
- Refunds and chargebacks
- Payment processing fees
- Taxes collected (sales tax, VAT)

### Payment Terms
- **Frequency:** Monthly
- **Timing:** Net-60 days (aligned with app store payout cycles)
- **Minimum threshold:** $100 before payout
- **Verification:** Third-party analytics (AppFigures, RevenueCat) accessible to both parties

---

## Intellectual Property Framework

### Dual Ownership Model (Recommended)

**Developer Owns:**
- Original app concept & design
- Original codebase (if any)
- App name & trademark
- Brand assets & identity
- User data & relationships

**Moonshot Owns:**
- Newly written code (the rewrite)
- Shared infrastructure & SDKs
- Monetization implementations
- Analytics integrations

### License Structure

**Developer receives:**
- Exclusive, perpetual, royalty-free license to use Moonshot's code for their app
- Ensures developer can always operate their app, even post-partnership

**Moonshot receives:**
- Non-exclusive license to reuse generic/framework components in other partnerships
- Does NOT include app-specific logic or branding

### Termination Scenarios
1. **Mutual termination:** Developer can buy out Moonshot's code at formula-based price (6-12 months revenue × 1.5-3x)
2. **Developer breach:** Moonshot retains code, can re-publish under different brand
3. **Moonshot breach:** Developer gets automatic code ownership at nominal cost

---

## App Store Account Strategy

### Recommended Approach
App stays in **developer's account**. Moonshot added with appropriate access roles.

| Platform | Moonshot Roles | Purpose |
|----------|----------------|---------|
| Apple App Store | App Manager + Sales | Publish updates, manage monetization, view revenue |
| Google Play | Admin + Finances | Full operational access, revenue visibility |

### Revenue Flow
1. Revenue goes to developer's account
2. Developer remits Moonshot's share monthly (via ACH)
3. Both parties have access to third-party revenue tracking (AppFigures/RevenueCat)

### Alternative: Transfer to Moonshot
- For very high-trust situations or acquisitions
- Moonshot receives all revenue, pays developer their share
- More control but requires stronger relationship

---

## Key Contract Clauses

### Term & Renewal
- **Initial term:** 2-3 years
- **Auto-renewal:** 1-year terms
- **Notice period:** 90 days before renewal to opt out
- **Performance clause:** Either party can terminate if revenue < agreed threshold for 6+ consecutive months

### Termination
- **For convenience:** 90-180 days notice after initial term
- **For cause:** 30-day cure period for material breach
- **Immediate grounds:** Non-payment (60+ days), IP infringement, criminal activity
- **Post-termination:** Licenses survive per agreement terms

### Buyout Provisions
- **Formula:** 6-12 months trailing revenue × 1.5-3x multiple
- **Payment terms:** Allow 12-24 month installments
- **Right of first refusal:** If developer sells app, Moonshot gets first right to buy
- **Code purchase:** Developer can buy out Moonshot's code at termination

### Non-Compete
- **During term:** Developer won't partner with competing accelerators for same app
- **Post-term:** 12-month limitation on directly competing services only
- **Scope:** Keep narrow (geographic + service focus) for enforceability

### Dispute Resolution
1. **Step 1:** 30-day informal negotiation
2. **Step 2:** Non-binding mediation (cost: $5-10K)
3. **Step 3:** Binding arbitration via JAMS/AAA
- **Jurisdiction:** Delaware law
- **Why arbitration:** Faster (6-12 months vs 2-4 years), cheaper ($20-50K vs $100K+), private

### Representations & Warranties

**Developer represents:**
- Owns all rights to original app; can enter agreement
- App doesn't infringe third-party IP
- Has rights to all third-party libraries/APIs used
- No existing agreements prevent this partnership

**Moonshot represents:**
- Will write professional-quality code following industry standards
- New code won't infringe third-party IP
- Will maintain app security and comply with store guidelines
- Has expertise to execute monetization strategy

### Indemnification
- **Mutual:** Each party indemnifies for their breaches
- **IP-specific:** Developer indemnifies for original app IP; Moonshot for new code IP
- **Cap:** Liability limited to 12 months revenue received (or $50K minimum)
- **Carve-outs:** Gross negligence, willful misconduct excluded from cap

---

## International Compliance

### United States
- **Entity:** Delaware LLC recommended
- **Reporting:** Issue 1099-NEC for payments $600+/year
- **Tax:** Developer handles their own (15.3% self-employment tax)
- **Payment:** ACH transfer via Wise, Mercury, or traditional bank

### European Union
- **GDPR:** Data Processing Agreement (DPA) required if processing EU user data
- **Classification:** Avoid contractor misclassification (verify true independence)
- **VAT:** May apply on services; developer handles local compliance
- **Payment:** SEPA transfer; pay in EUR or USD

### India
- **TDS Withholding:** 10% under US-India tax treaty (20% default without treaty docs)
- **Process:** Collect Form 15CA/15CB from developer, or use Deel to handle compliance
- **Payment:** SWIFT wire ($25-50 fee) or Wise/Payoneer (lower fees)
- **Currency:** Pay in USD; developer handles conversion

### Other Regions
- Collect W-8BEN form (foreign status) from all international developers
- Agreement clause: Developer responsible for local tax obligations
- Use Deel or Remote.com ($49/contractor/month) for complex situations

---

## Entity Structure

### Delaware LLC (Recommended)
- **Cost:** $300 filing + $90/year franchise tax
- **Tax:** Pass-through (avoid double taxation)
- **Admin:** Low (annual report only)
- **Best for:** Bootstrapped, profitable from start

### Delaware C-Corp (If Raising VC)
- **Cost:** $1,000-3,000 to form
- **Tax:** Double taxation (corporate + dividend)
- **Admin:** High (board meetings, minutes required)
- **Required for:** VC funding (preferred stock structure)

---

## Legal Cost Estimates

### Year 1: DIY Approach (~$2,400)
- Rocket Lawyer: $40/month × 12 = $480
- 2 attorney reviews for complex deals: ~$2,000
- Entity formation (Delaware LLC): $300

### Year 2+: Custom Template (~$5,000/year)
- Custom template creation: $3,000-5,000 (one-time)
- Per-deal reviews (high-value only): $500-1,500 each
- Ongoing counsel as needed: $200-400/hour

### DIY Platform Options
| Platform | Cost | Best For |
|----------|------|----------|
| Rocket Lawyer | $40/month | First 2-3 deals, unlimited docs, attorney access |
| LegalZoom | $199-399/template | One-off documents |
| Clerky | $500-1,000 | Startup fundraising docs (less relevant) |

---

## Documents Needed

### Required
- [ ] Master Partnership Agreement template
- [ ] NDA (for initial discussions)
- [ ] Code Access Agreement

### Optional (use standard versions)
- [ ] App Store Transfer Documentation
- [ ] Privacy Policy Template
- [ ] Terms of Service Template

---

## Next Steps

### Immediate
1. Form Delaware LLC ($300)
2. Obtain EIN from IRS (free, online)
3. Open business bank account (Mercury or Wise)
4. Subscribe to Rocket Lawyer ($40/month)
5. Customize revenue sharing agreement template

### Before First Deal
1. Set up ACH payment capability
2. Subscribe to AppFigures ($99/month) for revenue tracking
3. Register Moonshot trademark ($250-350)
4. Create IP audit checklist for partnership onboarding

### After 3 Partnerships
1. Hire attorney for custom template ($3,000-5,000)
2. Create state-specific versions (US, India, EU)
3. Evaluate Deel/Remote.com for international scale

---

*Last updated: December 2025*
*Full research report: [step10-legal-structure.html](step10-legal-structure.html)*
