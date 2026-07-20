## Day 17 — Vehicle Cost Analysis Dashboard

### Vehicle Details
- Model: Chevrolet Enjoy
- Fuel Type: Diesel
- Usage: Mixed (City + Highway)
- Monthly KM: ~1000 km
- Car Age: 10+ years (Old category)

### What Claude Generated
A complete single-file HTML dashboard with:
- KPI cards showing cost/km, monthly cost, E85 comparisons
- SVG bar chart comparing cost/km across all fuel types
- SVG doughnut chart showing CO₂/km per fuel type
- SVG line chart showing cost/km vs vehicle age (0–12 years)
  with vertical marker at 10 years
- Animated E85 score gauge out of 10
- Fuel comparison cards with pros, cons and best-use cases

### Key Findings from Dataset

**Diesel vs Other Fuels:**
- Diesel offers lower cost/km compared to Petrol
- CO₂ emissions higher than CNG and EV but lower than E85
- At 10+ years, maintenance cost/km increases significantly
  compared to newer vehicles

**E85 Paradox:**
- E85 appears cheaper at the pump
- But lower mileage makes the running cost higher than Petrol
- Break-even price calculation shows E85 is rarely beneficial
  for older high-mileage vehicles like mine

**Age Impact:**
- Old category (10+ years) shows highest maintenance cost/km
- Cost/km for aged vehicles is notably higher than new ones
- Upgrading to a newer vehicle could be more economical
  in the long run

### Most Surprising Insight
A 10+ year old diesel vehicle costs significantly more per km
in maintenance alone compared to a newer CNG vehicle —
the dashboard made this instantly visible through the
age vs cost line chart.

### Key Learnings
- Claude can process real CSV data and generate complete
  visual dashboards without any coding
- Pure SVG charts with no CDN dependencies load faster
  and work offline
- Data visualization reveals patterns that raw numbers hide
- The E85 paradox shows why cheaper pump price doesn't
  always mean cheaper running cost
- Age-based cost analysis is a powerful tool for
  vehicle upgrade decisions