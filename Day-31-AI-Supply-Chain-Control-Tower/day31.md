## Day 31 — AI Supply Chain Control Tower

### What I Built
A single-file HTML app (HTML, CSS, vanilla JavaScript only — no
frameworks, no backend) simulating a real-time Operations Control Center.
The player acts as Head of Operations for 3 minutes, triaging a growing
stream of operational alerts while 8 live KPIs react to every decision.

### KPIs Tracked
Service Level %, Customer Satisfaction, Inventory Health, Transportation
Efficiency, Operating Cost, Revenue Protected, Score, Remaining Time.

### Alert Types
Port Congestion, Supplier Delay, Truck Breakdown, Warehouse Running Out of
Stock, Customs Inspection, Demand Spike, Factory Machine Failure, Weather
Disruption, Wrong Inventory Count, Damaged Shipment — each with a title,
description, priority, time remaining, and business impact.

### Player Actions
Expedite Shipment, Use Backup Supplier, Reroute Trucks, Increase
Production, Transfer Inventory, Approve Air Freight, Ignore, Delay
Decision — each with different, sometimes delayed, consequences.

### My Playthrough
| Element | Detail |
|---|---|
| Final Score | 870 |
| Grade | A- |
| Toughest Alert | Port Congestion and a Warehouse Stockout hitting simultaneously, both high priority |
| Decision | Approved air freight for the warehouse first; rerouted trucks for the port congestion |

### What I Learned
Picking the objectively correct action for a given alert mattered less
than the order I handled alerts in. Two individually correct decisions
still cost KPI points when the lower-priority alert kept degrading in the
background while I resolved the other one first. The real skill the
simulation was testing was sequencing and triage under time pressure, not
just knowing the right response to each incident type.

### Files in this folder
- `ai-supply-chain-control-tower.html` — the working app
- Screenshots — live dashboard mid-game, a single alert with action buttons, final performance dashboard
