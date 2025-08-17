# CyberX — Hackathon Prompts

This file contains the exact prompts we used to generate the dataset and video narration with the help of an LLM.

---

## 1. Dataset Generation Prompt

```
You are tasked to generate a realistic WhatsApp-style health management dataset.  

Persona:
- Member: Rohan Patel, 46, Regional Sales Head, travels often.
- Health condition: Borderline hypertension.
- Support team: Doctor, Nutritionist, Physiotherapist, Concierge, Performance Scientist, and PA (Sarah).

Constraints (MUST follow):
- Duration: 8 months.
- Frequency: 2–5 messages per week.
- Diagnostics: Once every 3 months.
- Exercise updates: Every 2 weeks.
- Travel: 1 week out of every 4 (include adjustments in plan).
- Adherence: Around 50% (half of assigned actions are missed).
- Communication style: Short WhatsApp-like messages.

Format (JSON):
[
  {
    "id": 1,
    "ts": "2025-01-15 09:00",
    "sender": "Rohan Patel",
    "role": "Member",
    "text": "BP today was 136/84.",
    "tags": ["bp"],
    "links": [],
    "initiated_by": "member"
  },
  {
    "id": 2,
    "ts": "2025-01-15 11:30",
    "sender": "Dr. Warren",
    "role": "Medical Strategist",
    "text": "Plan update: reduce salt intake and add one Zone2 session this week.",
    "tags": ["plan_update"],
    "links": [1],
    "initiated_by": "elyx"
  }
]

Guidelines:
- Use short, natural chat-like sentences.
- Ensure decisions (green cards) always have links to supporting messages (Why-traceability).
- Spread data across 8 months with realistic timestamps.
- Mix successful adherence and missed actions.
```

