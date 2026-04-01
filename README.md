# 🔥 Cinder — Quit Smoking. Get Paid to Stay Quit.

Cinder is a digital health platform prototype designed for the Chinese market that combines **financial commitment contracts**, **continuous biometric monitoring**, and **social accountability** to drive smoking cessation — delivered as a WeChat Mini-Program experience.

This prototype was built as part of a UCLA Anderson Global Immersion course project.

---

## 🚀 Live Demo

> Open `cinder-app.html` directly in any browser — no installation or build step required.

---

## 📱 App Screens & How to Navigate

### 1. 🏠 Onboarding
The first screen you'll see. It shows the core value proposition and key market stats.
- Tap **"开始戒烟 — Start Quitting"** to begin the pledge setup flow
- Tap **"View Demo Dashboard →"** to skip straight to the dashboard with pre-filled demo data

---

### 2. 💰 Pledge Setup
Set your personal financial commitment and connect your devices.

- **Pledge slider** — drag to set your stake (¥100–¥2,000). The funding breakdown updates live to show the 3× multiplier effect:
  - Your personal stake
  - Employer match (100%)
  - Friends & family crowdfund (via WeChat Moments)
- **Preset chips** — tap ¥300 / ¥500 / ¥1,000 / ¥2,000 for quick selection
- **Device toggles** — connect Huawei Health (HRV + heart rate), WeChat Pay (transaction monitoring), and acoustic monitoring (cough tracking)
- Tap **"Lock In Pledge & Begin"** to start your quit journey

---

### 3. 📊 Dashboard
Your live quit headquarters. Shows:

- **Streak counter** — days smoke-free, funds unlocked, days to next payout
- **Week view** — green = clean day, orange = today
- **Verification status** — real-time status of spend monitoring, heart rate, and cough tracking
- **Pledge pool progress** — visual breakdown of how much you've earned back
- **Health metrics** — resting heart rate, HRV, blood oxygen SpO₂, and daily cough frequency vs. your baseline
- **Supporter wall** — names and amounts pledged by friends and family

> 💡 Tap **"Simulate JITAI Alert"** at the bottom of the supporter wall to see the intervention system in action.

---

### 4. ⚡ JITAI Alert (Just-In-Time Adaptive Intervention)
The core behavioral mechanism. Triggered when the algorithm detects vulnerability — a stress spike in HRV *plus* GPS proximity to a tobacco vendor.

The screen shows:
- What triggered the alert (location + biometric readings)
- The full financial stakes broken down by source (your money, employer's, your family's)
- Two response options: **walk away** or **start a breathing exercise**

Both buttons return you to the dashboard.

---

### 5. 🏆 Weekly Payout
Accessed via the **Rewards** tab in the bottom nav. Shows:
- Weekly payout amount unlocked to WeChat Pay
- Cumulative earnings progress
- Side-by-side health improvements since quit date

---

## 🛠 Technical Notes

- **Single file** — everything is contained in `cinder-app.html` (HTML, CSS, JS)
- **No dependencies** — no npm, no build step, no backend required
- **Mobile-first** — designed at 390×844px (iPhone 14 dimensions); best viewed on mobile or in browser DevTools mobile view
- **Fonts** — loaded from Google Fonts (requires internet connection): Noto Sans SC, DM Serif Display, Space Mono

---

## 👥 Team

| Name | Role |
|------|------|
| Annemarie | Context, Risk |
| Alex | Context, Overall Flow |
| Abhishek | Product/Service Innovation |
| Amy | Product/Service Innovation, Financials |
| Charlotte | Vibe Coding, Financials |
| Anthony | Execution |

---

## 📚 Key Research Citations

- **WeChat WeQuit RCT** (The Lancet, 2023) — validated WeChat as cessation delivery mechanism; 11.94% vs. 2.81% abstinence at 26 weeks
- **Sense2Quit** (JMIR, 2025) — 97.52% F1-score for AI smoking gesture detection on consumer smartwatches
- **HRV-based craving prediction** (NIH/PMC, 2024) — BiLSTM model predicts smoking events from HRV + GPS data
- **Bristol StopWatch Trial** (2024/2025) — 61% of participants reconsidered smoking after smartwatch JITAI nudge
- **Peking University Worksite RCT** (2024) — validated employer worksite as optimal cluster for financial cessation incentives in China
