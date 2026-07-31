## Day 27 — Prior Authorization Story Simulator

### What I Built
A single self-contained HTML app (Tailwind CDN + vanilla JavaScript, chat
bubbles built with createElement/appendChild only) that tells the Prior
Authorization process as an interactive 8-chapter story rather than a
process diagram — following one patient, Rahul, end to end.

### Characters
| Character | Role | Position |
|---|---|---|
| Rahul | Patient | Left, chat bubble |
| Priya | Healthcare Operations Specialist | Right, chat bubble |
| Narrator / Dr. Patel | Context and clinical notes | Centered italic text |

### Story Chapters
1. Doctor Visit — Dr. Patel diagnoses Rheumatoid Arthritis, prescribes Humira
2. Insurance Roadblock — PA submitted directly from provider to StarCare Health (illustrative payer)
3. What is PA? — Priya explains PA in plain language, including AMA 2023 PA Survey data on treatment delays
4. Insurance Review — eligibility, clinical documentation, ICD-10 match, step therapy history
5. Denial — denied for missing step therapy documentation; system-side cost noted (2+ staff hours per denial)
6. Appeal — document gathering, Letter of Medical Necessity, formal appeal filing
7. Approval — PA approved, saved on file permanently, reference number issued
8. Takeaways — Patient perspective (Rahul) + System perspective (denial rate, appeal rate, resolution time)

### Design Choices
- Two branching dialogue choices after every scene, affecting tone and detail
  of the conversation without changing the underlying 8-chapter structure
- Progress bar updates live across all 8 chapters
- StarCare Health labeled as an illustrative example throughout, not a real payer
- Beginner-friendly language throughout, aimed at someone with no healthcare
  operations background

### What I Learned
The denial in the story was never about the diagnosis or the treatment
choice — it was a documentation gap (missing step therapy history). That
reframed PA denials for me: most are not clinical disagreements, they are
missing data points in a specific format the payer requires. The system-side
stat that stuck with me most was that a single denial costs a physician's
office 2+ staff hours to resolve — which turns PA friction into a staffing
and operations cost, not just a patient-experience issue. I also learned
that once a PA like this is approved, it can be saved on file permanently,
removing the need to repeat the process for every refill.

### Files in this folder
- `pa-story-simulator.html` — the working app
- Screenshots — Doctor Visit scene, Denial scene, Approval scene, Takeaways screen
