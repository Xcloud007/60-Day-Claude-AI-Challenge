## Day 34 — Marketing Detective

### What I Built
A single-file HTML app (React via CDN + Babel, with a vanilla HTML/CSS/JS
fallback for offline reliability) styled as a detective game rather than a
dashboard — investigating a fictional marketing campaign's failure using a
corkboard-style evidence board.

### Case Structure
Each of the randomly loaded cases includes: Company Name, Industry,
Campaign Objective, Target Audience, Marketing Channels, Budget
Allocation, Campaign Metrics (Reach, CTR, Engagement, Conversions, Sales),
Customer Comments, Social Media Performance, one Primary Marketing
Mistake, three Supporting Clues, a Correct Explanation, and Suggested
Improvements.

### Flow
1. Case Assignment
2. Investigation Board
3. Interactive investigation with evidence cards (campaign objective,
   target audience, channels, customer comments, social report, metrics
   dossier, supporting clues)
4. Solve the Case — identify the primary marketing mistake
5. Case Closed animation
6. Learning Report

### My Investigation — Case #001: Brewtopia Coffee Co.
| Metric | Value |
|---|---|
| Reach | 1.2M |
| CTR | 0.4% |
| Engagement | 2.1% |
| Conversions | 310 |
| Sales | $18,400 |
| Budget Split | Instagram Ads 40%, Influencers 25%, Radio 25%, Flyers 10% |

**Supporting clues:** CTR unusually low despite huge reach; every customer
comment asked "where is this store?"; landing page saw 78% of clicks bounce
within 3 seconds with no location info above the fold.

**Verdict:** 100% correct on first try. Brewtopia ran a beautifully produced
awareness campaign but omitted the single most important call-to-action for
a local business — WHERE to find it. High reach with low conversion, plus
repeated customer confusion about location, pointed directly to a missing
local-intent element, not weak creative or poor targeting.

**Suggested improvements (from the report):** add store locator links/
addresses to every ad and caption, use geo-targeted "Nearest Location"
dynamic ads, add a map pin sticker on Instagram Stories, add "Get
Directions" CTA buttons on paid social.

### What I Learned
A campaign can succeed on reach, creative quality, and even engagement, and
still fail completely if it skips one practical detail that turns interest
into action. For a local business, "where" is not a footnote — it is the
actual call-to-action. The clearest signal wasn't a bad metric on its own,
it was the pattern across three different evidence sources (CTR, customer
comments, landing page behavior) all pointing at the same gap.

### Files in this folder
- `marketing-detective.html` — the working app
- Screenshots — theme picker, investigation board, verdict/learning report screen, full metrics dossier
