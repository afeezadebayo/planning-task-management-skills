---
name: weekly-review
description: "Run a 30 to 45-minute weekly review with an AI agent: an agent-prepared brief, empty inboxes, last week's results, stale task decisions, chased waiting items, a next action for every project, the next two weeks of calendar, a goals check, three to five priorities, focus blocks and a weekly lesson log. Use whenever someone wants to do a weekly review, plan next week, clean up an out-of-control task list, restart after a holiday or keep their productivity system trusted."
license: CC-BY-4.0
metadata:
  author: Afeez Adebayo
  author_url: https://afeezadebayo.com
  author_linkedin: https://www.linkedin.com/in/afeez-adebayo/
  author_x: https://x.com/za_icon
  source: https://afeezadebayo.com/skills-md/productivity/planning-tasks/weekly-review/
  category: productivity
  subcategory: planning-tasks
  version: "1.0.0"
  created: "2026-10-10"
  updated: "2026-10-13"
---

# Weekly Review

Every task system decays without a review. Lists fill with stale items, waiting-for items are never chased, projects lose their next actions, and the calendar for next week arrives as a surprise. Once a list stops being trusted, people go back to keeping things in their heads. David Allen's Getting Things Done method calls the weekly review the habit that keeps the whole system working: get clear, get current, get creative. [Reference, Getting Things Done]

This skill runs a structured weekly review with a person and their AI agent in 30 to 45 minutes. It empties inboxes, reviews last week's results, cleans the task list, chases waiting items, checks every project has a next action, looks at the coming two weeks of calendar, reconnects the week to goals and ends with three to five priorities for next week.

## Operating principles
1. **Same time every week.** A fixed slot, such as Friday afternoon or Monday morning, makes it a habit.
2. **Short and complete.** Cover every list briefly rather than one list deeply.
3. **Results before tasks.** Start with what happened, then plan what is next.
4. **The agent does the admin.** It prepares the summary; the person makes decisions.
5. **End with a plan.** The review is done when next week's priorities and first blocks exist.

## Inputs
- Task list (`TASKS.md` or task app), including Waiting for and Projects.
- Calendar for last week and the next two weeks.
- Goals for the quarter (`goals.md` or OKRs).
- Notes from the week: meeting notes, journal, completed work.
- Any inboxes not yet processed.

## When to use, and when not to
Use it weekly, after holidays or busy periods, when the task list feels out of control, or before planning a new week with a manager.

Don't use it for daily plans (`daily-planning`) or quarterly strategy (`quarterly-planning-review`), though it feeds both.

## Workflow (30 to 45 minutes)

### Part 1. Get clear (10 minutes)
1. **Empty inboxes:** email flags, chat saves, notes, paper and downloads go through `task-capture-clarify`.
2. **Brain dump:** anything on the person's mind that is not captured.

### Part 2. Get current (15 minutes)
3. **Last week's results:** what got done, what slipped and why. The agent prepares a list from completed tasks and calendar.
4. **Task list:** tick done items, delete what no longer matters, rewrite vague items, and decide on anything untouched for three weeks: do, schedule, delegate or delete.
5. **Waiting for:** chase anything overdue; the agent drafts the follow-ups.
6. **Projects:** every active project has one clear next action; pause projects with no capacity.
7. **Calendar:** last week for missed follow-ups; the next two weeks for preparation, travel and deadlines.

### Part 3. Get creative and plan (10 to 15 minutes)
8. **Goals check:** progress on each quarterly goal; one action per goal for next week.
9. **Someday/Maybe:** promote anything now worth doing; delete what has gone stale.
10. **Next week's priorities:** three to five outcomes, checked against free hours.
11. **Block time:** put the first focus blocks for those priorities in the calendar.

## Agent preparation (before the review starts)
The agent builds a one-page brief:
```
Week of <date>
Done: 18 tasks (top: launch brief approved, hiring post live)
Slipped: 3 (budget email, design review, invoice)
Waiting for overdue: 2 (contract from Acme, copy from Maya)
Stale tasks (21+ days): 5
Projects without next action: 1 (CRM migration)
Next week: 11 hours of meetings, 2 deadlines (Wed, Fri)
Goals: Q4 launch on track; hiring behind by one interview
```

## Review questions
- What were the three most important things I finished?
- What slipped, and is it still important?
- What am I waiting on, and who needs a nudge?
- What does next week's calendar demand?
- Which goal needs attention next week?
- What will make next week a success?

## Output format
```
1. Weekly brief (prepared by the agent)
2. Decisions on stale and slipped tasks
3. Follow-up messages drafted
4. Projects with next actions
5. Next week's 3 to 5 priorities linked to goals
6. Focus blocks added to the calendar
7. One lesson or change for next week
```

## Personal and life areas
A work-only review misses half the open loops. Add a two-minute scan of personal areas: health appointments, family commitments, money and bills, home admin, learning and relationships. Capture anything that needs action into the same list with an area tag, so nothing personal depends on memory.

## Checklist the agent follows
- [ ] Inboxes processed to zero
- [ ] Brain dump captured
- [ ] Done list summarised; slipped items decided
- [ ] Stale tasks (21+ days) decided
- [ ] Waiting for chased where overdue
- [ ] Every project has a next action
- [ ] Last week and next two weeks of calendar checked
- [ ] Quarterly goals checked; one action per goal
- [ ] Someday/Maybe skimmed
- [ ] Next week's priorities set and blocked
- [ ] One lesson logged

## Monthly add-on
Once a month, add 15 minutes: review the Someday/Maybe list in full, check progress on each quarterly goal against the plan, archive finished projects and look at the lesson log for patterns. This keeps the quarterly review short because most of the thinking has already happened.

## Where to keep the review
Store each brief and decision list in a dated file, such as `reviews/2026-10-11.md`, so the agent can compare weeks and spot trends.

## Edge cases and judgement calls
| Situation | What to do |
|---|---|
| Missed several weeks | Do a longer reset: archive old items, then resume the weekly slot |
| Only 15 minutes available | Do Part 2 steps 4 to 6 and Part 3 step 10 |
| Very heavy week ahead | Pick one priority; cancel or move low-value meetings |
| Team weekly review | Shared priorities, blockers and owners in 30 minutes; personal review separately |
| Review keeps getting skipped | Move it to a time with fewer interruptions; shorten it |

## Handoffs to related skills
- Processing inboxes: `task-capture-clarify`
- Task list structure: `task-system-setup`
- Choosing priorities: `prioritisation`
- Scheduling blocks: `time-blocking`
- Goals and quarterly planning: `goal-setting-okrs`, `quarterly-planning-review`

## Worked example
A consultant reviews on Friday at 4pm. The agent's brief shows 22 tasks done, 4 slipped, 3 overdue client replies and a project with no next action. In 35 minutes the consultant deletes 6 stale tasks, sends three follow-ups the agent drafted, adds a next action to the stalled proposal, notices a client workshop on Wednesday that needs preparation, and sets next week's priorities: finish the proposal, prepare the workshop, and invoice two clients. Two focus blocks go into Monday and Tuesday mornings.

## Common mistakes
- Skipping the review when busy, which is when it matters most.
- Reviewing only tasks and ignoring the calendar.
- Letting stale tasks linger for months.
- Ending without priorities or time blocks.
- Turning the review into a two-hour planning session.

## Making the habit stick
- Book a recurring calendar slot and treat it like a meeting.
- Use the same checklist every week.
- Let the agent send a reminder with the prepared brief.
- Keep a short log of weekly lessons; patterns appear within a month.
- If a week is missed, do a 15-minute version rather than skipping.

## Weekly lesson log
```
| Week | Biggest win | What slipped | Why | Change for next week |
| 7 Oct | Launch brief approved | Budget email | No focus time | Block Monday 9 to 11 |
```
After four to six weeks, the log shows recurring causes, such as meeting overload or late inputs from others, that are worth fixing at the root.

## Self-check before you answer
- Were inboxes emptied and stale tasks decided?
- Are overdue waiting items chased?
- Does every active project have a next action?
- Are next week's priorities linked to goals and blocked in the calendar?

---
Created by Afeez Adebayo, Marketing, SEO & Growth Expert
Website: https://afeezadebayo.com
LinkedIn: https://www.linkedin.com/in/afeez-adebayo/
X: https://x.com/za_icon
Source: https://afeezadebayo.com/skills-md/productivity/planning-tasks/weekly-review/

Licence: CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/). You may copy, share and adapt this skill, including for commercial use, as long as you credit Afeez Adebayo and link to the source URL above. Keep this notice in any copy or adapted version.
