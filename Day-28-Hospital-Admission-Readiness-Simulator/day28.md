## Day 28 — Hospital Admission Readiness Simulator

### What I Built
A single self-contained HTML app that scores how "ready" a hospital
admission is in real time, based on provider/physician details, diagnosis,
admission type, Prior Authorization status, and admission date — then lets
you resolve outstanding issues until the case is admission-ready.

### Inputs
| Field | Purpose |
|---|---|
| Provider & Physician Details | Identifies who is requesting the admission |
| Diagnosis & Admission Type | Drives which clinical criteria apply |
| Prior Authorization Status | Approved / Pending / Not Submitted |
| Admission Date | Used for urgency and timeline scoring |

### Risk Categories Tracked
- Documentation risk
- Insurance / PA risk
- Bed availability risk
- Clinical risk

### Workflow
Enter details → initial readiness score calculated → resolve PA scenario
(approve, leave pending, or appeal) → complete workflow actions to close
out documentation/insurance/bed/clinical risks → Governance Snapshot →
final admission decision.

### What I Learned
Admission readiness is not a single yes/no gate — it is four risk
categories that all have to close in parallel before a bed can safely
open. A case can be clinically ready and still blocked by an unresolved
Prior Authorization or an unconfirmed bed. The Governance Snapshot made
the operational side visible: what admissions teams actually track is not
just "was the patient admitted" but how many risks were still open at each
stage and how long each one took to resolve. That reframed Prior
Authorization for me as one risk category among several, not the whole
admission process.

### Files in this folder
- `hospital-admission-readiness-simulator.html` — the working app
- Screenshots — initial low-readiness screen, mid-resolution screen, Governance Snapshot, final admission decision
