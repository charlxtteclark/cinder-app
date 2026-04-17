# 🔥 Cinder — Investor Demo Prototype

> **China's first verified, incentive-based workplace smoking cessation platform.**  
> Built for State-Owned Enterprises facing mandatory ESG reporting deadlines.

This repository contains a fully interactive HTML prototype built for investor presentations and product demos. It simulates the complete Cinder mobile app experience across both the employee and employer user journeys — no backend required.

---

## 🚀 Live Demo

> Open https://charlotteclark.io/cinder-app/ directly in any browser - no installation or build step required.

---

## What is Cinder?

Cinder is a B2B2C SaaS platform that helps Chinese SOEs run verified, incentive-based smoking cessation programs. It addresses a structural market gap: SOEs face a mandatory April 2026 ESG disclosure deadline covering employee health metrics, but no compliant tool exists that combines biochemical verification, financial incentives, and audit-ready reporting.

**How it works:**
- Employees commit a personal stake (¥100–¥1,000) into an escrow-style program
- Their employer matches with a ¥500 bonus per verified quitter
- Abstinence is verified via cotinine saliva testing at Month 3 and Month 6 — not self-reported
- Verified quitters redeem their bonus as a family gift (JD.com, education fund, elder care, travel)
- Employers receive PIPL-compliant, audit-ready ESG reports automatically

**Evidence base:** Cochrane systematic reviews across 20,000+ participants confirm guaranteed financial incentives increase quit rates by 46–49%. Group-based interventions double cessation rates at 6-month follow-up. Peking University is currently running an active RCT with ¥600 incentives in the Chinese context.

---

## Demo Overview

The prototype renders as a 390×844px iPhone shell in the browser. All interactions are live — tap through the full user journey without any server or build step.

### Employee Flow

| Screen | Description |
|--------|-------------|
| **Login** | Role selector with platform stats (300M smokers, +49% quit rate lift, 10× employer ROI) |
| **Commit to Quit** | Matching mechanic — employee sets stake via slider (¥100–¥1,000), employer match displayed, total pool calculated in real time |
| **Dashboard** | Streak hero, weekly calendar, live verification chips, commitment pool progress, health metrics, team leaderboard, encouragement messages |
| **JITAI Alert** | Just-in-time adaptive intervention — triggered by GPS + HRV context, shows full forfeit amount (employee stake + employer match), offers breathing exercise |
| **Breathing Exercise** | Functional 60-second 4-7-8 breathing timer with live phase guidance and progress bar |
| **Cotinine Verification** | 4-step kit flow, test schedule tracker, "Track My Kit" popup modal (links to lab partner) |
| **Gift Catalog** | 4 family gift options (JD.com, Education Fund, Elder Care, Family Travel), employer bonus framing |
| **Gift Confirmation** | Redemption success screen with next payout countdown |
| **Feedback** | Habit voting for future programs (alcohol, weight, sleep, stress), free-text suggestion field |

### Employer Flow

| Screen | Description |
|--------|-------------|
| **Employer Dashboard** | ESG compliance badge, 4 KPI cards, anonymized department competition table, cotinine kit status, ROI calculator, ESG report card |
| **Enroll New Cohort** | Matching configuration (employer match + employee stake range), loss aversion explainer, 3 optional add-on services (cotinine kits, medication referral, cost assistance), projected outcomes calculator |

---

## Running the Demo

No installation, no build step, no dependencies.

```bash
# Clone the repo
git clone https://github.com/your-org/cinder-app.git
cd cinder-app

# Open in browser
open cinder-app.html
```

Or just double-click `cinder-app.html` in Finder / Explorer.

> **Note:** Requires an internet connection for Google Fonts (Fraunces, Space Mono, Noto Sans SC). The prototype renders correctly offline if fonts have been cached by a prior visit.

---

## Navigation Guide

| Action | How |
|--------|-----|
| Employee path | Login → tap "I want to quit smoking" |
| Employer path | Login → tap "I'm an employer / HR" |
| Back navigation | ← button in screen headers |
| Simulate JITAI alert | Dashboard → scroll to Team Encouragement → tap "Simulate JITAI Alert" |
| Live stake sync | Commit to Quit slider → updates Dashboard + JITAI amounts in real time |
| Track My Kit | Cotinine screen → opens popup modal |

---

## Design System

Built to match the Cinder pitch deck color palette exactly.

| Token | Hex | Usage |
|-------|-----|-------|
| Primary blue | `#156082` | Buttons, highlights, active states |
| Dark navy | `#0E2841` | Headings, body text |
| Light blue | `#0F9ED5` | Accents, progress bars |
| Orange | `#E97132` | Commitment stake, warnings |
| Background | `#F4F7FA` | App background |
| Card | `#FFFFFF` | All card surfaces |

**Fonts:**
- `Fraunces` — display / numbers (streak count, bonus amounts)
- `Space Mono` — monospaced data values
- `Noto Sans SC` — body text and Chinese characters

---

## Technical Notes

- **Single file** — entire prototype is `cinder-app.html` (~150KB including embedded brand images)
- **No framework** — vanilla HTML, CSS, and JavaScript only
- **Responsive shell** — fixed 390px width mimicking iPhone 14 Pro; centers at any screen size
- **Live state sync** — slider values propagate across screens (enroll → dashboard → JITAI) via DOM manipulation
- **Embedded assets** — brand images encoded as base64 to eliminate external file dependencies

---

## Business Context

| Metric | Value |
|--------|-------|
| Target market | ~16.6M SOE employees who smoke |
| Software license | ¥200 / enrolled employee / year |
| Employer bonus (pass-through) | ¥500 / verified quitter |
| Cochrane quit rate lift | +46–49% with guaranteed incentives |
| Employer ROI | ~10× (¥8,000–12,000 healthcare savings per quitter) |
| ESG forcing function | April 2026 mandatory disclosure deadline |
| Y3 revenue target | ¥20M ARR (100,000 enrolled employees) |
| Y5 revenue target | ¥127M ARR (500,000 enrolled employees) |
| 5-year IRR | ~34% |

---

## Team

Built by Team Cinder — MBA candidates at UCLA Anderson for Professor Kramer's Global Immersion course.

*This prototype was developed for investor presentations. All employee data shown is illustrative.*
