## Day 48 — The Verdict Engine

### What I Built
A single self-contained HTML comparison tool that researches real, citable
data for every data point instead of inventing numbers, with adjustable
criteria weights that update the ranking live, a visible Sources panel,
and a collapsible "How this was researched" panel documenting methodology
and source conflicts.

### The Comparison
**Category:** Ultraportable laptops
**Options:** ASUS Zenbook 14 OLED (UX3405), MacBook Air 13" (M3), Lenovo
ThinkPad X1 Carbon Gen 12, Dell XPS 13 9345
**Criteria:** Price (lower is better), Battery Life (higher is better),
Performance (higher is better, mixed benchmarks — flagged), Ports &
Connectivity (higher is better)

### Ranked Result (equal weights, 100% each)
| Rank | Laptop | Score |
|---|---|---|
| 1 | ASUS Zenbook 14 OLED (UX3405) | 249.9 |
| 2 | MacBook Air 13" (M3) | 231.4 |
| 3 | Lenovo ThinkPad X1 Carbon Gen 12 | 222.0 |
| 4 | Dell XPS 13 9345 | 150.1 |

Weights don't need to total 100% — relative weight drives the ranking, and
ranking is normalized (min-max, 0–100) relative to the best/worst performer
among these four laptops only, not an absolute scale.

### How This Was Researched — Key Findings
**Price:** Taken from each outlet's stated starting configuration price at
time of review. The ThinkPad X1 Carbon's $1,500 figure is flagged as an
estimate — reviewers tested configurations ranging from $1,902 to $2,263,
while StorageReview cites $1,500 for the base SKU; street pricing on this
model varies unusually widely.

**Battery life — methodology conflict flagged:** the four laptops were not
tested on the same benchmark. Zenbook 14 and ThinkPad X1 Carbon both used
PCMark 10's "Modern Office" test (directly comparable to each other). The
XPS 13 figure came from Reviewed.com's web-browsing loop, a lighter
workload that tends to produce longer times. The MacBook Air figure is
Apple's own wireless-web rating, since PCMark 10 doesn't run on macOS.
Cross-platform battery comparisons here are labeled directional, not exact.

**Performance:** Geekbench 6 multi-core was used for the MacBook Air,
Zenbook 14, and ThinkPad X1 Carbon, since all three had a directly reported
GB6 figure. The Dell XPS 13 9345 (Snapdragon X Elite) had no GB6 figure
available in the sources gathered, so its score instead used EnosTech's UL
Procyon Computer Vision benchmark — a different test measuring AI/CV
throughput rather than general CPU throughput. Flagged as an
estimate/mixed-methodology figure.

**Ports:** Counted from each outlet's confirmed port list. The MacBook Air
and XPS 13 ship with exactly two high-speed USB-C/Thunderbolt ports and
nothing else built in (no USB-A, no HDMI) — flagged by several reviewers as
a real workflow tax for travelers who need a dongle. The Zenbook and
ThinkPad both include native USB-A and HDMI alongside Thunderbolt.

### Sources Used (15 citations)
Apple official tech specs; Laptop Mag (MacBook Air review, Geekbench leak
coverage, ThinkPad X1 Carbon review); Tom's Guide (MacBook Air review);
InvGate spec database (MacBook Air, ThinkPad X1 Carbon); TechRadar (Dell
XPS 13 review); Reviewed.com (Dell XPS 13 battery test); Consumer Reports
(Dell XPS 13 review); EnosTech (Dell XPS 13 review); PCWorld (Zenbook 14
OLED review); Trusted Reviews (Zenbook 14 OLED battery test); FrontDeskReview
(Zenbook 14 OLED performance data); StorageReview (ThinkPad X1 Carbon
review).

### What I Learned
The most useful thing the tool surfaced wasn't a data point at all — it was
where the data points stopped being comparable. The Dell XPS's Performance
score was quietly built on a completely different benchmark (AI/CV
throughput) than the other three laptops' Geekbench CPU scores, and the
battery life figures spanned three different test methodologies across
four laptops. A comparison tool is only trustworthy if it tells you which
numbers weren't measured the same way — averaging mismatched benchmarks
into one clean-looking ranking would have been the easy, dishonest version
of this tool.

### Files in this folder
- `the-verdict-engine.html` — the working app
- Screenshots — weight/comparison setup, live ranked result, "How this was researched" panel, Sources panel
