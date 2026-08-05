## Day 33 — Media Integrity Analyzer

### What I Built
A single-file HTML app (pure vanilla CSS/JS, no frameworks) that teaches
media literacy through guided discovery — guess first, then reveal the
mechanism behind a misleading headline or an emotionally manipulative post.

### Flow
1. Color theme selection (including Claude Orange)
2. Challenge 1 — Headline Detective: fictional headline + article, "Would
   you click this?" (Yes/Maybe/No), identify misleading parts, then reveal
   Headline Accuracy Score, highlighted mismatches, explanation, fair
   rewritten headline, and key takeaway
3. Challenge 2 — Emotion Detector: fictional post/caption, identify feeling
   and influencing words, then reveal target audience, intended emotional
   response, manipulation technique, highlighted phrases, neutral rewrite,
   and key takeaway
4. Live metrics throughout: Headline Accuracy, Source Reliability,
   Emotional Manipulation, Audience Targeting
5. Final Media Integrity Dashboard: Overall Score, what was learned,
   biggest red flag, three practical habits

### My Playthrough
| Challenge | What Happened |
|---|---|
| Headline Detective | Said "Yes, I'd click this" — the headline used a causal verb ("causes") the article only supported as a correlation |
| Emotion Detector | Felt urgency/alarm — reveal showed this was the intended response, built via scarcity language and an unnamed "experts warn" appeal to authority |

### What I Learned
The headline that fooled me was not obviously false — it was a true-sounding
claim with a stronger verb than the evidence actually supported. That
reframed the whole exercise: media manipulation usually is not lying, it is
framing true information to feel bigger or more certain than it is. The
practical habit I'm taking from this: before reacting to a headline, check
whether its verb is doing more work than the article underneath it proves.

### Files in this folder
- `media-integrity-analyzer.html` — the working app
- Screenshots — theme picker, Headline Detective reveal, Emotion Detector reveal, final dashboard
