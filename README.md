# SaaS-B2B-KPI-Case-Study
🚀 Live Demo

 directly in any modern browser — no build step, no server, no dependencies to install.


🎯 What Problem This Solves

Most business dashboards show what happened. This dashboard shows why it matters and what to do next.
It was designed around a real SaaS scenario: a B2B collaboration tool running a Land & Expand model with $4M+ MRR — where surface-level metrics looked healthy while hidden signals pointed to emerging risks.


 Problem Statement
**The Business:** A SaaS B2B Collaboration Tool operating on a **Land & Expand**
model (Freemium → Team → Business → Enterprise).
**The Surface Story:** $4.03M MRR, 124.3% NRR, 88% gross margin — everything looks
healthy.
**The Hidden Reality:** Three critical problems were masking serious risks

| Problem | Metric | Risk Level |
|---------|--------|------------|
|  Silent Churn | 28.5% of accounts inactive 60+ days | **CRITICAL** |
|  Feature Discovery Gap | 70% never discover Feature #3 | **HIGH** |
|  UI Redesign Backfire | Support confusion tickets +133% | **HIGH** |

**The Challenge:** Build a dashboard that doesn't just *report* numbers — it
connects KPIs to causal insights and recommended actions.
---
##  What I Learned
### 1. Data Storytelling > Data Visualization
A beautiful chart means nothing without context. Every metric on this dashboard
connects to:
- **What** happened (the number)
- **Why** it happened (the insight)
- **What to do** about it (the action)
> *Example:* NRR of 124% is just a number. NRR of 124% masking 28.5% silent churn
is a story that saves $680K ARR.

### 2. Building From Scratch Teaches You How Tools Work
After configuring Chart.js datasets, dual axes, custom tooltip callbacks, and
responsive breakpoints, I understand what Power BI and Tableau do under the hood.
I'm a better BI developer because I built without one.

### 3. The "So What?" is Everything
Every insight must answer: *"So what? What should we do differently?"*
| Insight | So What? | Action |
|---------|----------|--------|
| Silent churn at 28.5% | $680K ARR at risk | Day-45 intervention playbook |
| 70% miss Feature #3 | 25% expansion revenue locked | Force multi-feature onboarding |
| Confusion tickets +133% | Churn spike in 90 days | In-app contextual guidance |

**The Lesson:** A number without action is just a statistic. A number with a recommended action is business intelligence.
### 4. Technical Depth + Business Context = Competitive Advantage
I can explain both the CSS Grid layout AND why silent churn is a leading indicator
of renewal risk.
---


### Tech Stack
| Layer | Technology | Purpose |
|-------|------------|---------|
| Frontend | HTML5 + CSS3 | Semantic markup, responsive layout |
| Visualization | Chart.js 4.x | Interactive charts with animations |
| Date Handling | chartjs-adapter-date-fns | Time-series support |
| Styling | CSS Custom Properties | Theme consistency, instant color changes |
| Layout | CSS Grid + Flexbox | Responsive without frameworks |
| Interactivity | Vanilla JavaScript (ES6) | Event handling, drill-down simulation


---
##  Key Insights & Solutions
###  Insight 1: Silent Churn Crisis
**The Paradox:** NRR of 124.3% looks healthy, but 28.5% of accounts show zero
logins for 60+ days.
**Root Cause:**
- Reactive churn management (act on cancellation, not disengagement)
- No early warning system
- 100% retention budget on expansion, 0% on resurrection
**Financial Impact:** 342 at-risk accounts = $680K ARR exposure
**Solution:**
- Build "at-risk" playbook triggered by engagement drop (Day 45)
- Launch re-engagement campaign for 60+ day inactive accounts
- Implement account health score: login freq × feature breadth × team size
- Reallocate 20% expansion budget to resurrection
**Expected Impact:** Save $680K ARR, reduce silent churn to <15% in 6 months
---
###  Insight 2: Feature Discovery Gap
**The Discovery:** Accounts using 4+ features generate 3x more expansion revenue.
But 70% never discover Feature #3.
**Root Cause:**
- Onboarding focuses on first action only
- No forced multi-feature exposure
- TTV to Feature #3 is 7.2 days (60% of free users churn by then)
**Solution:**
- Redesign onboarding to force multi-feature exposure in first 7 days
- Measure TTV to Feature #3 as primary onboarding KPI
- Add feature discovery prompts at Day 3 and Day 5
- Create integration marketplace highlights for Team plan users
**Expected Impact:** +25% expansion revenue, 50% increase in 4+ feature adoption
---
###  Insight 3: UI Redesign Backfire
**The Warning:** Support confusion tickets spiked 133% post-redesign. CSAT stayed
flat — users confused, not angry (yet).
**Root Cause:**
- Redesign improved aesthetics but degraded discoverability
- No contextual guidance for redesigned features
- Confusion precedes churn by 90 days (historical pattern)
**Solution:**
- Categorize tickets: target confusion <25% of total
- If confusion >40%, halt new features, run usability sprints
- Implement in-app contextual guidance (tooltips + checklists)
- A/B test old vs new UI for power users
**Expected Impact:** -40% support cost, prevent projected churn spike

---
##  How to Run Locally
### Prerequisites
- Any modern web browser (Chrome, Firefox, Safari, Edge)
- No build tools, no dependencies, no installation
### Steps
```bash
# 1. Clone the repository
git clone https://github.com/[YOUR_USERNAME]/[YOUR_REPO_NAME].git
# 2. Navigate to the project folder
cd [YOUR_REPO_NAME]
# 3. Open in browser (or use Live Server in VS Code)
open index.html
```
That's it. The dashboard loads instantly with all charts rendered client-side.
---
##  Project Structure
```
saas-kpi-dashboard/
n
nnn index.html # Main dashboard file
nnn README.md # This file
nnn assets/
n nnn screenshots/ # Dashboard preview images
n nnn css/ # (Optional) External stylesheets
n
nnn data/ # (Optional) Data files for API integration
nnn kpi_data.json
```
---
##  Key Metrics at a Glance
| Metric | Value | Trend | Status |
|--------|-------|-------|--------|
| Monthly Recurring Revenue | $4.03M | ↑ +18% MoM |  Healthy |
| Net Revenue Retention | 124.3% | ↑ +2.1pp |  Healthy |
| PQL Rate | 5.6% | ↑ +0.2pp |  Improving |
| Time to Value | 2.1 days | ↓ -0.8 days |  Improving |
| Enterprise Sales Cycle | 42 days | ↓ -23 days |  Improving |
| Gross Margin | 88% | ↑ +1pp QoQ |  Healthy |
| Support Tickets / $100K | 12.1 | ↑ +25% |  Alert |
| Silent Churn Rate | 28.5% | ↑ +12pp |  Critical |
---
##  Formulas Used
### Net Revenue Retention (NRR)
```
NRR = [(Starting MRR + Expansion MRR - Contraction MRR - Churned MRR) / Starting
MRR] × 100
```
### Silent Churn Rate
```
Silent Churn Rate = (Accounts with Zero Logins 60+ Days / Total Paying Accounts) ×
100
```
### Support Tickets per $100K MRR
```
Tickets per $100K = Total Support Tickets / (MRR / $100,000)
```
### PQL Rate
```
PQL Rate = (Number of PQLs / Total Free/Trial Users) × 100
```
### Time to Value (TTV)
```
TTV = Timestamp of First Value Moment - Timestamp of Account Creation
```
---
##  What Makes This Different
| Typical Dashboard | This Dashboard |
|-------------------|----------------|
| Reports what happened | Explains **why** it happened |
| Static charts | Interactive drill-down simulation |
| Numbers only | Narrative insights + action items |
| Tool-dependent | Built from scratch — full ownership |
| One-size-fits-all | Custom UX for executive decision-making |
---
##  Why HTML/Chart.js Instead of Power BI?
**Short answer:** I can use Power BI. I chose to build from scratch to prove deeper
capabilities.
**Long answer:**
- **Full customization:** Every pixel, interaction, and animation is controlled
- **Zero licensing:** No per-user costs, no Microsoft ecosystem dependency
- **Version control:** Every change tracked in Git, CI/CD ready
- **Performance:** Lightweight, fast loading, works on any device
- **Portfolio value:** Demonstrates full-stack data storytelling, not just tool
operation
> *"Knowing how to build visualizations from scratch makes me better at pushing
Power BI beyond its default templates."*
---
##  Future Enhancements
- [ ] Connect to live API for real-time data updates
- [ ] Add user authentication and role-based views
- [ ] Implement filter controls (date range, segment, plan tier)
- [ ] Export to PDF/PNG functionality
- [ ] Dark/light theme toggle
- [ ] Add predictive churn model with ML
---
##  Contact
I'm currently exploring opportunities in **Data Analytics**, **Product Analytics**,
and **Business Intelligence**.
If you're building data-driven products and need someone who connects technical
execution to business impact — let's talk.

- n Email: sasiofficial022@gmail.com
- n LinkedIn: https://www.linkedin.com/in/sasikumar806/
- n Portfolio: https://sasi-dev-portfolio.vercel.app/
-
---
##  License
This project is licensed under the MIT License — feel free to use, modify, and
share.
---
> **Built with by Sasi Kumar** | Data period: Jan 2024 – Jun 2026 | Case Study:
SaaS B2B Collaboration Tool
