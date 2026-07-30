# Day 25 — AI Shark Tank Simulator

**Challenge:** 60-Day Claude AI Mastery Challenge by ABTalks
**Task:** Build a complete AI Shark Tank Simulator as a single self-contained HTML file, pitch a startup idea to 4 AI judges, get scored, and receive an investment verdict.

## What I Built

A single-file HTML app (no backend) with:
- A startup pitch intake form (name, problem, solution, revenue model, audience, funding ask)
- 4 distinct AI judges — Venture Capitalist, Founder, Customer, Angel Investor — each asking 2 tailored questions
- Live scoring across Market Potential, Innovation, Business Model, Execution, and Investment Worthiness
- An investment decision engine (Invest / Reject / Acquire / Come Back Later) with valuation and funding numbers
- Bonus features: confetti on a funded outcome, a downloadable pitch report, a leaderboard, and a share button

## My Pitch

**Startup:** Loopr
**Problem:** Small D2C brands lose 20–30% of revenue to cart abandonment because follow-up is manual and inconsistent.
**Solution:** An AI agent that automatically drafts and times personalized recovery messages across email and WhatsApp, learning from what actually converts.
**Revenue Model:** SaaS subscription + 1% of recovered revenue
**Target Audience:** D2C skincare and fashion brands doing $50K–$2M/year
**Funding Ask:** $150,000 for 8% equity

## Toughest Question

Marcus Vale (Venture Capitalist) opened with:
> "How big is the total addressable market for Loopr, and what stops a bigger player from crushing you in a quarter?"

This was the hardest one to answer well — it wasn't really asking for a number, it was testing whether I'd thought about defensibility. My answer leaned on the recovered-revenue pricing model as a moat (competitors charging flat SaaS fees don't have skin in the game the way we do), but I could tell the panel wanted sharper numbers on TAM.

## Scorecard

| Metric | Score |
|---|---|
| Market Potential | 74/100 |
| Innovation | 68/100 |
| Business Model | 81/100 |
| Execution | 63/100 |
| Investment Worthiness | 72/100 |
| **Composite** | **72/100** |

## Verdict

**Come Back Later.** The panel liked the business model and the revenue-share pricing but felt execution proof was thin — no traction data, no case study. Suggested valuation: ~$1.6M. No funding offered this round; the reasoning specifically called out that clearer unit economics and a working pilot would flip this into an Invest next time.

## Learnings

- The scoring engine reacts noticeably to answer *length and specificity* — vague one-liners pulled Execution and Investment Worthiness down fast, while answers with concrete numbers pushed Business Model up.
- Writing 4 judges with genuinely different focus areas (market vs. execution vs. usefulness vs. profitability) made the cross-examination feel much less repetitive than one generic "AI investor."
- Ran into a bug where escaped apostrophes in the judges' reaction lines broke the entire script silently (buttons did nothing, no console-visible reason to a non-dev). Good reminder to actually open dev tools and check for JS syntax errors before assuming a UI issue.
- Building the investment decision as a function of composite score + parsed funding ask (rather than a fixed table) made the verdict feel earned rather than random.

## Files in this folder
- `shark-tank-simulator.html` — the working app
- Screenshots — pitch input screen, judges cross-exam screen, scorecard, verdict
- Pitch report PDF (downloaded from the app)
