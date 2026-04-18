# AI orchestration

## Candidate models

- **Gemini Flash Live** (realtime voice-in / voice-out) — the likely spine of the interaction loop
- **Secondary LLM callouts** for slower reasoning, planning, memory, content moderation — open question which provider(s)
- **Vision** — does the camera feed go into a multimodal live model, into a cheaper classifier (e.g. "person detected", "costume guess"), or both?

## Orchestration pattern

_How do the pieces fit together?_

- Realtime voice loop vs. turn-based ("push-to-talk-equivalent" triggered by motion/vision)
- Where vision enters the loop (always-on context vs. snapshot on trigger)
- How movement/light cues get emitted — tool/function calls from the model? Separate control plane driven by audio envelope?
- Wake condition — motion sensor? Face detection? Always listening?

## Latency budget

_Target end-to-end response time. What feels "alive" vs. awkward on a porch interaction?_

-

## Persona / prompt

_System prompt drafts, voice style, named character, backstory, "things it will and won't say"._

-

## Memory

_Session-only? Remember across the night? Across years? Privacy implications._

-

## Safety and guardrails

- Kids at the door — content filters, topics to avoid
- Bystander privacy — are we recording? What's retained?
- Fail-safe behavior when models/network are unavailable (canned lines, offline mode?)

## Notes
