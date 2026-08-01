## Day 29 — Operation Lifeline: Supply Chain Crisis Lab

### What I Built
A single-file HTML app (React via CDN + Babel JSX, no build step) that
simulates leading a fictional company through a randomized supply chain
crisis — from initial response, through supplier negotiation and executive
decision-making, to a final scored dashboard.

### Flow
1. Welcome screen → Start Simulation
2. Randomly generated company profile (industry, revenue, factories,
   warehouses, suppliers, inventory days, lead time, countries)
3. Randomly assigned crisis (one of: factory fire, supplier bankruptcy,
   port strike, cyberattack, flood, raw material shortage, political
   conflict, shipping delay)
4. War Room — choose 3 of 6 response actions; Cost, Inventory, Profit,
   Delivery Speed, and Customer Satisfaction update via animated bars
5. Negotiation — 4 branching rounds affecting Trust, Price, and Lead Time
6. CEO Boardroom — 5 leadership multiple-choice questions
7. AI Strategy — choose 2 of 5 AI investments (Demand Forecasting,
   Inventory Optimization, Supplier Risk Monitoring, Warehouse Vision,
   Procurement Copilot)
8. Final Dashboard — Overall Crisis Score (0-100) plus Leadership,
   Negotiation, Resilience, Cost Control, Risk Management, and Customer
   Satisfaction sub-scores, with personalized feedback, biggest mistake,
   best decision, and lessons learned

### My Playthrough
| Element | Detail |
|---|---|
| Crisis | Port strike during an active shipment window |
| Strategy | Prioritized alternate freight routing + proactive customer communication over the cheapest short-term fix |
| Final Crisis Score | 78/100 |

### What I Learned
The simulation scores negotiation and boardroom decisions on different
axes entirely — negotiation rewards protecting long-term supplier Trust,
while the boardroom rewards decisive, transparent stakeholder
communication. Optimizing Cost Control alone hurt Resilience, which made
it clear that a real crisis response is several simultaneous trade-offs
(cost, speed, trust, risk, communication), not a single dial to maximize.

### Files in this folder
- `operation-lifeline.html` — the working app
- Screenshots — company profile + crisis screen, War Room decision, negotiation screen, final dashboard
