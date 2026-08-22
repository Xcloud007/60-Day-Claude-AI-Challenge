## Day 46 — Autonomous Agent Studio

### What I Built
A single self-contained HTML app orchestrating a real multi-agent pipeline
against the live Claude API — not a fixed sequence, but an actual loop that
re-calls Evaluator, Critic, and Improver each round with a live API call,
continuing until a stop condition fires at runtime rather than a pre-set
round count.

### Interview Setup
| Question | My Answer |
|---|---|
| Spec | Write a Python function `parse_log_lines(lines)` that takes a list of raw web server log strings (Common Log Format) and returns a list of dicts with keys: ip, timestamp, method, path, status, size. Malformed lines should be skipped, not crash the function. Include a small `__main__` example. |
| Target score to stop (threshold) | 90 / 100 — high bar |
| Hard iteration cap (safety fallback) | 8 rounds |

### Agent Roster
| Agent | Responsibility |
|---|---|
| Planner | Turns the raw spec into a concrete implementation plan: function signature, edge cases, test strategy |
| Executor | Writes the first complete draft of the code from the plan |
| Safety Monitor | Screens each draft for dangerous operations (file/network/system access, eval, secrets) before scoring |
| Evaluator | Scores the draft 0–100 against a fixed rubric: correctness, robustness, style, docs |
| Critic | Reads the draft + score and lists concrete, actionable issues the Evaluator's number doesn't capture |
| Memory Manager | Distills lessons across rounds so the Improver stops repeating fixed mistakes |
| Improver | Rewrites the draft using the evaluation, critique, and memory — produces the next round's code |
| Final Reviewer | Runs once, after a stop condition fires: polishes the winning draft and writes the closing summary |

### How the Stop-Check Governs the Loop
Every round, after Evaluator + Critic + Memory Manager finish, three checks
run in this order — the first one that fires ends the loop and hands off
to the Final Reviewer:
1. **Plateau** — the rubric score improved by less than 2 points for two
   consecutive rounds (diminishing returns; not worth another live call).
2. **Threshold** — the score crosses the chosen target (90/100 here); the
   code is good enough by the set rubric.
3. **Hard cap** — a safety fallback, never the intended ending. If neither
   check fires, the loop stops anyway at 8 rounds so it can't run forever.

State threads forward explicitly: each Evaluator call sees the current
draft plus the fixed rubric; each Critic call sees the draft plus that
round's evaluation; each Improver call sees the draft, evaluation,
critique, and the Memory Manager's distilled lessons from every prior
round.

### What I Learned
Laying out the agent roster made it clear that the Memory Manager is the
component that actually makes the system self-improving rather than
self-repeating — without it, each Improver pass only has the current
round's critique to work from, and late rounds could keep re-making early
mistakes. Building this also surfaced a real infrastructure constraint:
calling a live model API directly from a static local HTML file is a
genuine systems problem, not just a prompt detail — a browser doesn't let
a local page freely call an external API without the right setup around
it. Designing an orchestration loop on paper is straightforward; getting
the first live call through reliably is where the actual engineering work
starts.

### Files in this folder
- `autonomous-agent-studio.html` — the working app
- Screenshots — interview/spec setup, live pipeline agent roster and loop diagram
