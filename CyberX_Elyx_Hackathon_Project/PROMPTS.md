# Prompts / Instructions Used

1) Conversation generation rubric:
- Persona: Analytical, time-constrained executive; expects evidence.
- Channels: WhatsApp-like tone; PA (Sarah Tan) used for scheduling.
- Constraints enforced:
  - Diagnostics every 3 months (fasting reminders, results + plan updates).
  - Exercise updates every 2 weeks — Rachel adjusts based on travel fatigue & data.
  - Member-initiated: 2–5 messages per week on average.
  - Travel: 1 week out of every 4; hotel-gym modifications & jet-lag protocols.
  - Adherence ~50% → Neel sends prioritization pivots.
  - Chronic condition: borderline hypertension (BP check-ins & dietary sodium strategies).
  - Wearables: Garmin initially; (optionally Oura) trend callouts tied to sleep/stress.

2) “Why” traceability:
- Every plan update links back to recent evidence: diagnostics, BP notes, sleep/HRV, travel context.

3) Visualization requirements:
- Timeline with filters (by sender/tag).
- Clickable *decision* cards (#plan_update / #exercise_update) → reveal evidence chain.
- Current state panel by date.
- Internal ops metrics: message counts by role; weekly adherence proxy & HRV proxy sparkline.

4) Guardrails:
- Keep clinical phrasing general; no medical diagnosis beyond brief.
- Focus on rationale and behavior change hooks.

