## Day 35 — Prompt Puzzle: Master AI Prompting Through Play

### What I Built
A single-file HTML app (React via CDN if reliable offline, otherwise a
vanilla HTML/CSS/JS fallback) that teaches prompt engineering through three
game mechanics rather than a tutorial format. Generation started with a
2-question onboarding interview: domain and difficulty.

### Challenge Types
1. Build the Prompt — assemble correct prompt blocks while avoiding distractors
2. Clean the Prompt — fix a weak/messy prompt into an optimized one
3. Choose the Best Prompt — pick the optimized version over weak and
   over-engineered alternatives

### Scoring Tracked
Accuracy, Time, Moves, Wrong Placements, Hints Used, Optimization Bonus —
rolling up into a final Prompt Performance Report (Prompt Score, Rating,
Rank, Prompt DNA visualization, personalized feedback, next milestone,
final optimized prompt).

### My Results
| Metric | Value |
|---|---|
| Prompt Score | 304 |
| Rank | Prompt Novice ("Developing Performance") |
| Accuracy | 39% |
| Total Time | 83s |
| Moves | 8 |
| Wrong Placements | 2 |
| Hints Used | 0 |
| Perfect Scenarios | 1/6 |

**Prompt DNA breakdown:** Clarity 84%, Efficiency 86%, Specificity 33%,
Structure 17%, Optimization 17%.

**Final optimized prompt example given:** "Write a single HTML button
element that triggers a JavaScript alert saying 'Hello!' when clicked.
Keep the code minimal with no external libraries, and show the complete,
ready-to-run code snippet."

### What I Learned
Clarity and efficiency turned out to be a completely different skill from
structure and specificity — my Prompt DNA showed I could write prompts
that were short and easy to understand, while still scoring low on
Structure and Optimization. In the Choose the Best Prompt challenge, the
winning option was not the most detailed one; it was the one that included
just the relevant context (the actual code, the observed vs. expected
output) without padding it with irrelevant instructions. The Clean the
Prompt challenge made the opposite mistake obvious too — a prompt loaded
with unrelated asks ("also explain quantum entanglement," "write it as a
10-page thesis") fails not because it's unclear, but because it lacks
focus. The real lesson: a clear prompt gets understood, but a structured,
specific prompt is what actually gets the right answer on the first try.

### Files in this folder
- `prompt-puzzle.html` — the working app
- Screenshots — domain/difficulty selection, a challenge in progress, final Prompt Performance Report
