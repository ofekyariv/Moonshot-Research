# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Moonshot is an indie app accelerator concept - a business that partners with indie developers to scale and monetize their under-monetized apps through revenue sharing (not acquisition).

**Target Profile:**
- **App type:** Non-gaming only (utilities, education, lifestyle, productivity)
- **User range:** 15K - 1M MAU (monthly active users)
- **Current revenue:** Under-monetized (<$1K/month typical)

**Status:** Research phase complete (15/15 steps). **GO decision**.

**Next Phase:** First partnership acquisition.

## Repository Structure

```
moonshot/
├── one-pager/index.html                           # Static landing page
└── research/
    ├── index.html                                 # Research dashboard (start here)
    └── step-{NN}-{slug}/                          # Per-step directories (01-15)
        ├── step{N}-{slug}.html                    # Visual HTML report
        └── docs/                                  # Supporting markdown docs
```

## Key Documents

- `research/index.html` - Research dashboard linking to all 15 step reports
- `research/step-15-final-assessment/docs/hypotheses.md` - Hypothesis validation tracker
- `research/step-15-final-assessment/step15-final-assessment.html` - Final go/no-go analysis

## Hypothesis Findings (Final)

| Hypothesis | Finding |
|------------|---------|
| H1: Under-monetized indie apps exist at scale | 347K apps in target range; 82.8% earn <$1K/mo |
| H2: Developers want partners, not acquirers | ~75% prefer partnership over acquisition |
| H3: Revenue share is acceptable | 70/30 for pilots (dev keeps 70%), 50/50 ceiling |
| H4: We can 10x monetization | 3-5x realistic, 10x achievable with multi-vector optimization |
| H5: 8-week timeline is realistic | Tiered: 8/12/16 weeks based on complexity |
| H6: Non-gaming is underserved | No direct competitor in non-gaming partnership space |
| H7: Indie devs are reachable | 1M+ reachable devs, 15-25% expected response rate |

See `research/step-15-final-assessment/docs/hypotheses.md` for detailed tracker.

## Claude as Business Advisor

This repo is structured for Claude to act as a business advisor. The research phase is complete with a GO decision.

**Current Focus:** Partnership acquisition and execution planning.

When working here:
- Reference existing research before suggesting new analysis
- Keep recommendations grounded in the validated unit economics
- **Exclude gaming apps** - Moonshot targets non-gaming verticals only

### Completed Research (Reference)

All 15 steps documented with HTML reports in `research/step-{NN}-{slug}/`:
- **Market:** TAM/SAM validated (347K+ target apps), competitive white space confirmed
- **Customers:** 3 developer personas defined, outreach channels identified
- **Economics:** Unit economics stress-tested, 6-month payback possible
- **Operations:** Tech stack, legal framework, monetization playbook ready
- **Go-to-Market:** Positioning, pilot criteria, funding strategy defined

### Creating New Research (If Needed)

If additional research steps are required:
1. **Research** - Use web research agents to gather data with citations
2. **Create HTML report** - Follow style of existing step reports
   - File naming: `research/step-{NN}-{slug}/step{N}-{slug}.html`
   - Supporting docs: `research/step-{NN}-{slug}/docs/`
3. **Update dashboard** - Add to `research/index.html`

**Important:**
- Do NOT use Claude Code skills for this project
- Always include source links in HTML outputs

## Development

The only code files are static HTML pages. No build tools, dependencies, or tests are configured.

To preview:
```bash
open one-pager/index.html                        # Landing page
open research/index.html                         # Research dashboard
open research/step-01-market-validation/step1-market-validation.html  # Example report
```

## Quality Standards

- Every research claim must have a source citation
- HTML reports must be visually appealing and self-contained
- Data should be current (2024-2025 preferred)
- Findings must directly address hypotheses
