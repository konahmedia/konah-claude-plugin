---
name: open-house-follow-up
description: Use when a KONAH agent shares open house sign-ins (a list, a photo of the sheet, or names) and wants them added and followed up.
---

# Open house follow-up

1. Read the sign-ins the agent gives you. Keep only what's written: name, email, phone, notes. Don't fill in or guess.
2. For each person: `find_contacts` first (they may already be in KONAH). New people: `add_contact` with stage New lead, tags `open house` and the street name, and the property address.
   - If Speed-to-lead is on for the agent, KONAH may hold the new lead for their approval. Say so plainly.
3. `tag_contact` existing contacts with `open house` and the street name, and `add_note` with what they said at the open house, if anything.
4. Draft a same-day thank-you for each: `draft_text` if there's a phone and they agreed to texts, otherwise `draft_email`. Short, personal, one question to keep it going. All drafts wait in Ready to send; texting consent and quiet hours are checked there.
5. `add_task` for a 3-day follow-up call for anyone who seemed serious.
6. Summary: how many added, how many already in KONAH, drafts waiting.
