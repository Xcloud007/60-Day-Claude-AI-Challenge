## Day 30 — Supply Chain Builder

### What I Built
A single-file HTML app (React via CDN + Babel JSX, no build step) that
teaches supply chain fundamentals by having the player build one from
scratch for a randomly generated company, with a plain-English trade-off
explanation after every decision.

### Flow
1. Welcome screen introducing supply chains in simple language
2. Random company profile (industry, products, countries served, demand level)
3. Guided build-out across 5 decisions:
   - Number of suppliers (single or multiple)
   - Factory location
   - Warehouse strategy
   - Transportation method (road, rail, sea, air)
   - Inventory strategy (low, balanced, high)
4. Live metrics after every choice: Cost, Delivery Speed, Risk, Customer
   Satisfaction, Sustainability
5. Final dashboard: Overall Supply Chain Score (0-100), strengths,
   weaknesses, biggest risk, and three practical improvements

### My Playthrough
| Element | Detail |
|---|---|
| Biggest-impact decision | Multiple suppliers over a single supplier |
| Effect | Risk and Sustainability improved noticeably; Cost rose slightly; Delivery Speed barely changed |
| Final Supply Chain Score | 81/100 |

### What I Learned
Supplier count had a bigger effect on the final score than transportation
or inventory strategy, even though those two felt like the more obvious
levers going in. A single-supplier setup is a structural point of failure
that no later transportation or warehousing choice can fully offset. The
practical takeaway: supply chain resilience is mostly decided at the
earliest decision points, not the ones that feel most "operational."

### Files in this folder
- `supply-chain-builder.html` — the working app
- Screenshots — company profile screen, mid-decision metrics screen, final dashboard
