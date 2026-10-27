---
name: task-capture-clarify
description: "Collect commitments from email, chat, meetings, documents, calls and ideas into one inbox, then process each item with the Getting Things Done decisions: delete, do now under two minutes, delegate, defer to the calendar, create a project or file as reference, extracting actions, owners and dates from notes and threads. Use whenever someone wants a brain dump, to process their inbox or to-do list, to turn meeting notes, email threads or chat into tasks, or feels overwhelmed by loose commitments."
license: CC-BY-4.0
metadata:
  author: Afeez Adebayo
  author_url: https://afeezadebayo.com
  author_linkedin: https://www.linkedin.com/in/afeez-adebayo/
  author_x: https://x.com/za_icon
  source: https://afeezadebayo.com/skills-md/productivity/planning-tasks/task-capture-clarify/
  category: productivity
  subcategory: planning-tasks
  version: "1.0.0"
  created: "2026-10-10"
  updated: "2026-10-12"
---

# Task Capture and Clarify

Tasks arrive from everywhere: email, chat, meetings, calls, documents, voice notes and passing thoughts. When they are not captured, people rely on memory and things slip. When everything is captured but never clarified, lists fill with vague notes nobody wants to start. David Allen's Getting Things Done method separates these steps: capture everything in a few trusted inboxes, then clarify each item into a decision. [Reference, Getting Things Done]

This skill helps a person and their AI agent collect commitments from every source into one inbox, then process each item quickly: delete it, do it now, delegate it, defer it to a date, turn it into a project or file it as reference.

## Operating principles
1. **Capture fast, decide later.** Getting it out of the head is the first job.
2. **Few inboxes.** Two or three collection points the person checks, not ten.
3. **Every item gets a decision.** Nothing stays in the inbox after processing.
4. **Two-minute rule.** If it takes less than about two minutes, do it now.
5. **Next action or nothing.** Kept items become a clear action, a waiting item, a project or reference.

## Capture sources
| Source | How to capture |
|---|---|
| Email | Flag or forward actionable emails to the task inbox; the agent extracts actions |
| Chat (Slack, Teams, WhatsApp) | Save or forward messages with requests |
| Meetings | The agent extracts actions, owners and dates from notes |
| Documents and comments | Mentions and assigned comments go to the inbox |
| Calls and voice notes | Dictate a one-line note immediately |
| Ideas on the go | A quick-add note on the phone |

## When to use, and when not to
Use it for inbox processing, turning meeting notes or email threads into tasks, a brain dump when overwhelmed, or cleaning up a messy to-do list.

Don't use it to choose what to do today (`prioritisation`, `daily-planning`) or to triage email itself (the Email and Inbox skills).

## Workflow

### Step 1. Collect
Gather items from the agreed sources. For a brain dump, list everything on the person's mind without filtering: work, home, people, money, ideas.

### Step 2. Clarify each item
Ask two questions: what is it, and is it actionable?

```
Not actionable  -> delete, keep as reference, or add to Someday/Maybe
Actionable, < 2 min -> do it now
Actionable, someone else should do it -> delegate, add to Waiting for
Actionable, needs one step -> write the next action, add to the list
Actionable, needs several steps -> create a project with a first action
Has a fixed date or time -> calendar
```

### Step 3. Write the next action
Verb, object, and where helpful a person, place or tool: "Call the landlord about the leak", not "Flat".

### Step 4. Add context only where it helps
Due dates only when real, the person for waiting items, the source link, and a tag for the area.

### Step 5. Empty the inbox
Confirm every item has a home. Show counts: done, delegated, scheduled, added, projects, reference, deleted.

### Step 6. Set the habit
Process inboxes once or twice a day at set times, not continuously.

## Extracting actions from text
When given meeting notes, email threads or chat logs, the agent:
- Finds sentences that commit someone to do something ("I'll send", "can you", "we need to", "by Friday").
- Records the action, owner, due date and source.
- Marks the user's own actions for the task list and others' for Waiting for.
- Lists unclear items as questions rather than guessing owners or dates.

```
| Action | Owner | Due | Source | Goes to |
| Send revised budget | Me | Fri 18 Oct | Finance sync notes | This week |
| Approve copy | Maya | Wed | Launch thread | Waiting for |
```

## The five lists after processing
| List | Holds | Reviewed |
|---|---|---|
| Next actions | Single steps the person will do | Daily |
| Waiting for | Actions owed by others, with person and date | Weekly, or sooner if urgent |
| Projects | Outcomes needing more than one step, each with a next action | Weekly |
| Calendar | Time-specific actions and appointments | Daily |
| Someday/Maybe | Ideas and options not committed to | Monthly |

## Delegating well
A delegated item needs four things: who, what done looks like, by when, and how they will confirm. The agent drafts the delegation message and adds the item to Waiting for with the date sent, so follow-up happens at the weekly review rather than relying on memory.

## Reference and Someday/Maybe
Reference material, such as documents, links and information, goes to the notes system, not the task list, so tasks stay short. Someday/Maybe holds ideas worth keeping but not committing to now; reviewing it monthly turns good ideas into projects at the right time.

## Brain dump prompts
When someone feels overwhelmed, prompts help empty the mind: projects started but not finished, promises made to people, calls and emails to return, things to buy, bills and admin, home repairs, health appointments, learning goals, and anything causing worry. Every item is captured first, then clarified one by one.

## Daily processing rhythm
Two short sessions work for most people: one mid-morning after the first focus block and one late afternoon. Each takes 10 to 20 minutes and ends with an empty inbox. Between sessions, capture only; do not process continuously.

## Common capture tools
Any tool works if it is always within reach: a notes app on the phone, an email address that forwards to the task inbox, a chat message to the agent, or a paper notebook processed daily. Pick the fewest that cover every place commitments arrive.

## Edge cases and judgement calls
| Situation | What to do |
|---|---|
| Huge backlog (hundreds of items) | Process the newest 50; move older items to a dated archive for later |
| Items that are worries, not tasks | Write one next step or move to Someday/Maybe; suggest talking it through if distress is high |
| Requests with no deadline | Ask the requester or set a review date |
| Shared inbox | Agree owners for each item type |
| Personal and work mixed | One system with area tags, or two lists with a shared review |

## Handoffs to related skills
- Where tasks live: `task-system-setup`
- Choosing priorities: `prioritisation`
- Breaking down projects: `project-breakdown`
- Weekly clean-up: `weekly-review`
- Email triage: the Email and Inbox skills
- Meeting notes to actions: the Meetings and Calendar skills

## Worked example
A founder returned from a week of travel with 140 unread emails, two pages of meeting notes and a full head. The agent extracted 38 actions from the notes and flagged emails, the founder did 11 two-minute items immediately, delegated 7 to the team with dates, turned 4 into projects with first steps, put 3 fixed appointments in the calendar, filed 6 as reference and deleted 7. The task list gained 13 clear next actions, and the inbox was empty in under an hour.

## Output format
```
1. Captured items (count by source)
2. Decisions table: item | decision | next action | owner | date
3. New tasks for the task list
4. Waiting for items
5. New projects with first actions
6. Questions about unclear items
```

## Common mistakes
- Capturing without ever processing.
- Writing topics instead of next actions.
- Too many inboxes to check.
- Inventing owners or due dates.
- Processing continuously instead of at set times.

## Self-check before you answer
- Does every item have a decision?
- Is every kept task a clear next action?
- Are unclear owners and dates listed as questions?
- Is the inbox empty?

---
Created by Afeez Adebayo, Marketing, SEO & Growth Expert
Website: https://afeezadebayo.com
LinkedIn: https://www.linkedin.com/in/afeez-adebayo/
X: https://x.com/za_icon
Source: https://afeezadebayo.com/skills-md/productivity/planning-tasks/task-capture-clarify/

Licence: CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/). You may copy, share and adapt this skill, including for commercial use, as long as you credit Afeez Adebayo and link to the source URL above. Keep this notice in any copy or adapted version.
