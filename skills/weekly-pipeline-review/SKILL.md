---
name: weekly-pipeline-review
description: Use when a KONAH agent wants a weekly or Monday review of their pipeline, leads going cold, stuck deals, or who to focus on this week.
---

# Weekly pipeline review

A 10-minute Monday review of the agent's own KONAH CRM.

1. Pull the picture:
   - `find_contacts` with `stage` for each active stage (New lead, Contacted, Active client, Closing…), `limit` 25.
   - `find_contacts` with `quiet_days: 14` for people going cold.
   - `keep_in_touch_due` and `deal_dates` (days: 14).
   - `agenda` (days: 7, overdue: true).
2. Report in four short sections: Deals closing soon, Hot leads to call, Going cold, Overdue. Names and the one fact that matters for each.
3. Propose changes as a list and ask before doing them: stage moves (`move_stage`), follow-up tasks (`add_task`), keep-in-touch cadence (`set_keep_in_touch`). Do the ones they approve.
4. Offer drafts for the "going cold" group (`draft_text` or `draft_email`, one per person, personal, no pressure). They wait in Ready to send.
5. End with the 3 things that matter most this week.

Rank people only by stage, dates, activity and what the agent told you, never by anything about who they are.
