## Day 26 — Prior Authorization Workflow Simulator

### What I Built
A single self-contained HTML app (no frameworks, no CDNs, no localStorage —
all state in JavaScript memory) that gamifies the US healthcare Prior
Authorization process as a drag-and-drop workflow across three lanes:
Patient, Provider, and Payer.

### Scenarios Included
| Scenario | Procedure |
|---|---|
| Elective Surgery | Total Knee Replacement |
| Advanced Imaging | Lumbar Spine MRI |
| Specialty Medication | Biologic Therapy for RA |
| Inpatient Admission | Admission for Pneumonia |

### Core Workflow
Clinical Order → Medical Necessity Evaluation → Document Collection →
Submit to Payer → Payer Intake → Utilization Review → Payer Decision →
(branches to Pend / Appeal / Peer-to-Peer as needed) → Outcome Communicated

### Features Implemented
- Drag-and-drop case movement between stage columns (click-to-advance fallback)
- Medical necessity checklist specific to each scenario
- Document collection with required vs. distractor documents
- Scoring-driven payer decision (necessity completeness + document completeness + speed)
- Full Pend → resubmit loop and Denial → Appeal → Peer-to-Peer → Final Decision branch
- Days elapsed counter and Efficiency score, both affected by choices made
- Progress tracker across the top, updating live
- Confetti celebration on approval
- Workflow summary modal with a full step log
- Restart / New Patient flow

### What I Learned
Document completeness carried the most weight in whether a request got
approved, pended, or denied — even more than the "clinical severity" framing
suggests. A single missing required document was enough to trigger a Pend,
which alone added several days before the case could be reviewed again.
Modeling the decision as a weighted score (necessity criteria + document
completeness + turnaround speed) made it obvious that most real-world PA
friction is a documentation and workflow-design problem, not a clinical
disagreement problem.

### Files in this folder
- `pa-workflow-simulator.html` — the working app
- Screenshots — dashboard/tracker, workflow in progress, payer decision, workflow summary
