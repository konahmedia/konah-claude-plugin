---
name: after-showing
description: Use when a KONAH agent describes a showing, call, or meeting they just had (often a voice note) and wants it logged, followed up, or turned into next steps.
---

# After a showing or call

Turn what the agent just said into CRM updates in one go.

1. Find the person with `find_contacts` (name, phone or address). If there are two matches, ask which one. If there are none, offer `add_contact`.
2. `add_note` with the facts in plain words: what they saw, what they liked or didn't, timeline, next step. No guesses, nothing they didn't say.
3. If a next step has a day ("call Friday", "send listings tomorrow"), `add_task` with that due day. If no day was said, suggest one and ask.
4. If the stage clearly changed ("they want to write an offer"), offer `move_stage` and say from what to what.
5. Offer a thank-you or follow-up: `draft_text` (under 300 characters) or `draft_email`, in the agent's voice. It waits in Ready to send for their Send.
6. Confirm back in 2-3 lines: note logged, task set for <day>, draft waiting.

Never write anything about the buyer's protected characteristics in notes or drafts.
