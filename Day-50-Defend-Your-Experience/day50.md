## Day 50 — Defend Your Experience

### What I Built
A single self-contained HTML app designed to run inside Claude's artifact
environment, calling the Anthropic Messages API directly (no backend, no
API key setup required). The user uploads a resume, LinkedIn profile,
portfolio, bio, project, research write-up, performance review, startup
story, or freelance work sample. Instead of reviewing the document for
quality, the app extracts every meaningful claim inside it and treats each
one as something that must be defended under questioning.

### How It Works
1. **Interview-first setup:** the app asks what the user wants to defend,
   why they're preparing, the expected audience, and (if not already known)
   their preferred visual style — before generating anything.
2. **Adaptive challenge, not a fixed script:** every answer the user gives
   shapes the next follow-up question. The interview deepens and gets more
   specific over time rather than working through a generic template.
3. **Claim extraction:** every meaningful statement in the uploaded
   document — an achievement, a metric, a responsibility, a project — is
   pulled out individually and challenged, surfacing vague claims and
   missing evidence rather than accepting them at face value.
4. **Defense Report:** a final summary showing which experiences are
   well-defended, which need improvement, and concrete direction on how to
   strengthen the weaker ones before a real interview.

### Design Principles
- The objective is explicitly not to improve the resume itself — it's to
  build the user's ability to defend every claim they've already made
  about themselves.
- Confidence indicators and progress tracking run throughout the session,
  not just at the end.
- Supports drag-and-drop upload, local storage, session history, exports,
  and graceful fallback handling for temporary API errors (e.g. rate
  limits).
- Empty states and onboarding are written to make the tool's purpose
  obvious to a first-time user with zero context.

### What I Learned
Most resume/interview-prep tools optimize the document itself — better
phrasing, stronger verbs, tighter formatting. This tool works from a
different premise: the real risk isn't how a claim reads on paper, it's
the gap between what's written and what the person can actually explain
under a real follow-up question. That gap is invisible until someone
specifically probes for it, which is exactly what a first-round interviewer
does. Building an adaptive interviewer — one where each answer determines
the next, harder question — made it obvious how differently that pressure
tests a claim compared to a one-time resume review.

### Files in this folder
- `defend-your-experience.html` — the working app
- Screenshots — upload/interview setup, a mid-conversation challenge, final Defense Report
