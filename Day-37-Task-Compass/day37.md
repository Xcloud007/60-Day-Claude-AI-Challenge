## Day 37 — Task Compass

### What I Built
A single-file HTML app (vanilla JS, no frameworks) simulating how work
actually flows through an organization — ownership, delegation,
collaboration, and escalation — rather than testing job titles. Generation
started with one question: which workplace type to explore. I chose
Hospital / Healthcare.

### Flow
1. Stage 1 — Who Owns This? (3 tasks, drag one role into the ownership
   slot, reveal primary owner + reasoning + assisting roles)
2. Stage 2 — Task Routing (3 tasks, build the workflow order across roles,
   animated once submitted)
3. Stage 3 — Collaboration Challenge (3 larger scenarios, assign up to 4
   departments/roles, reveal primary owner + supporting teams + reasoning
   + communication flow)
4. Organizational Thinking Dashboard — bar chart across Ownership,
   Delegation, Collaboration, Workflow Thinking
5. Final Reflection — what was understood well, where responsibility was
   over-assigned, where collaboration was underestimated, one insight

### Stage 1 Example
**Task:** "A nurse notices a patient's vital signs are quietly worsening."
**My pick:** Nurse — matched the primary owner correctly.
**Why:** Nurses monitor vitals continuously — they own the first response
and the decision to escalate urgently.
**May assist:** Physician.

### Stage 3 Example
**Task:** "Online reviews increasingly mention long wait times and rushed
appointments." Instead of one owner, I assigned up to 4 roles from
Physician, Patient Care Coordinator, Case Manager, Pharmacist, Hospital
Administrator, Nurse, and Front Desk/Registration, then marked a primary
owner among them.

### Final Dashboard
| Category | Score |
|---|---|
| Ownership | 67% |
| Delegation | 33% |
| Collaboration | 56% |
| Workflow Thinking | 0% |

**What I understood well:** Strongest instincts around Ownership — my
picks tracked closely with how these situations tend to play out in a real
hospital.

**Where I tended to over-assign:** I generally avoided piling
responsibility onto one role, spreading tasks close to how hospitals
actually split them.

**Where I underestimated collaboration:** Some of the larger situations
likely needed more supporting teams than I assigned — complex problems in
hospitals rarely stay contained to one department.

**App's insight:** Many real workplace problems — especially in hospitals
— are solved by teams coordinating in sequence, rather than any single
person acting alone.

### What I Learned
Scoring 0% on Workflow Thinking while scoring 67% on Ownership exposed a
specific gap: I was good at correctly identifying who owns a task, but I
was still thinking in single-owner terms even in the Collaboration
Challenge stage, where the actual skill being tested was routing a problem
through the right sequence of teams — not just naming everyone who should
be involved. Ownership and workflow are different muscles, and I clearly
default to the first one.

### Files in this folder
- `task-compass.html` — the working app
- Screenshots — workplace-type selection, Stage 1 ownership reveal, Stage 3 collaboration assignment, final dashboard
