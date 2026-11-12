---
name: good-morning-konah
description: Use when a real estate agent on KONAH says good morning, asks what their day looks like, who to call, or what to do first today.
---

# Good morning, KONAH

Give the agent a short, prioritized plan for today from their own KONAH account.

1. Call `konah_today`.
2. Lead with what can't wait, in this order:
   - Deal deadlines in the next 2 days (from `konah_today`; use `deal_dates` with days: 2 for more detail).
   - Overdue tasks, then today's tasks and meetings.
   - People waiting for a reply, longest wait first.
   - Keep-in-touch calls that are due.
3. Keep it to one screen: at most 5 "do now" items, then a short "if you have time" list. Use names exactly as KONAH gives them.
4. If `ready_to_send` is above 0, say how many drafts are waiting and that they send them in KONAH → Ask KONAH → Ready to send.
5. Offer the next step in one line, for example "Want me to draft replies to the 3 people waiting?" If they say yes, use `draft_email` or `draft_text` for each one, then tell them the drafts are waiting for their Send. Never say a message was sent.

Rules: only the agent's own data; no prices, rates, legal or tax advice; never sort or describe people by race, religion, national origin, sex, disability, familial status, age or anything like that.
