---
name: task-system-setup
description: "Set up a plain-text task system a person and their AI agent share: a TASKS.md file with Today, This week, Waiting for, Later, Projects and Done, a MEMORY.md glossary that decodes shorthand, people and codenames, next-action rewrites, update rules and morning, after-meeting and weekly sync routines. Use whenever someone wants an AI agent to manage their to-do list, set up TASKS.md, consolidate scattered tasks, teach an agent their shorthand or sync tasks from meetings, email and chat."
license: CC-BY-4.0
metadata:
  author: Afeez Adebayo
  author_url: https://afeezadebayo.com
  author_linkedin: https://www.linkedin.com/in/afeez-adebayo/
  author_x: https://x.com/za_icon
  source: https://afeezadebayo.com/skills-md/productivity/planning-tasks/task-system-setup/
  category: productivity
  subcategory: planning-tasks
  version: "1.0.0"
  created: "2026-10-10"
  updated: "2026-10-12"
---

# Task System Setup (Agent-Maintained Task List)

AI agents are good at keeping lists tidy, but only if they know where the list lives, how it is structured and what the user's shorthand means. Without that, every session starts from zero: the agent asks the same questions, misreads "send PSR to Todd re Phoenix", and tasks drift between chats. Anthropic's open-source productivity plugin tackles this with a plain task file and a working-memory file that decodes the user's own terms, people and projects. [Reported, anthropics/knowledge-work-plugins]

This skill sets up and maintains a simple, plain-text task system that a person and their AI agent share: a `TASKS.md` file with clear sections, a glossary that decodes shorthand, rules for adding, updating and closing tasks, and routines for syncing tasks from meetings, email and chat.

## Operating principles
1. **Plain text, one file.** A Markdown task file works in any agent and any editor.
2. **Next actions, not topics.** Every open task starts with a verb and is small enough to do.
3. **Decode once, remember always.** Shorthand, nicknames and codenames go into a glossary the agent reads first.
4. **The user owns priorities.** The agent proposes; the user decides what matters.
5. **Keep it light.** If maintenance takes more than a few minutes a day, simplify.

## The files
**`TASKS.md`**
```
# Tasks
## Today
- [ ] Draft Q4 budget email to Sam (due Tue) #finance
## This week
- [ ] Review launch brief from Maya #launch
## Waiting for
- [ ] Contract signature from Acme (asked 3 Oct) #legal
## Later
- [ ] Research new CRM options #ops
## Projects
- Launch: next action "Book review with design" (see projects/launch.md)
## Done (this week)
- [x] Send invoice to Northwind (2 Oct)
```

**`MEMORY.md` (working memory and glossary)**
```
## People
Sam: finance lead, approves budgets
## Terms and codenames
PSR: product status report, weekly, sent Fridays
Phoenix: the website redesign project
## Preferences
Due dates in day-month format; British English
```

Larger projects can have their own file under `projects/` with goal, milestones and next actions.

## When to use, and when not to
Use it when setting up an AI-assisted task list, moving from scattered lists to one file, teaching an agent the user's shorthand, or syncing tasks from notes, email and chat.

Don't use it when a team must use a shared project tool such as Asana, Jira or Linear; in that case mirror only personal tasks, or connect the agent to the shared tool.

## Workflow

### Step 1. Find the existing tasks
Ask where tasks live now. Import them into `TASKS.md`, grouped by section.

### Step 2. Decode shorthand
For each task, find abbreviations, nicknames, project codenames and unclear references. Ask only about terms not yet decoded, and add each answer to `MEMORY.md`.

### Step 3. Rewrite as next actions
Turn vague items into verb-led actions with a clear finish: "Website" becomes "Send homepage copy to design for review".

### Step 4. Add useful metadata
Due dates only where real, a person for waiting items, tags for areas, and links to source messages.

### Step 5. Agree the rules
| Event | Agent action |
|---|---|
| New request in a message or meeting | Add to Today, This week or Later with source and date |
| Task done | Tick it and move to Done with date |
| Someone else owes an action | Move to Waiting for with person and date asked |
| Task untouched for 3 weeks | Flag at the weekly review: do, schedule, delegate or delete |
| Unknown term | Ask once, then add to the glossary |

### Step 6. Set the sync routines
- **Morning:** read `TASKS.md`, suggest Today's top three, flag overdue items.
- **After meetings:** add actions from notes, with owners and dates.
- **Weekly:** clean Done, review Waiting for, archive stale items, update projects.

### Step 7. Keep memory current
Add new people, terms and projects as they appear. Keep `MEMORY.md` short, ideally under 100 lines, with detail in separate files.

## Writing good next actions
| Vague | Next action |
|---|---|
| Budget | Email Sam the three cost options for Q4 budget |
| Website | Send homepage copy to design for review |
| Hiring | Write the job description draft for the analyst role |
| Taxes | Collect last year's invoices into one folder |
A good next action names a verb, an object and, where it helps, a person and a finish line. If the action takes more than about two hours, it is probably a project; give it a file and a first step.

## Tags and areas
Keep tags few and stable, such as #finance, #launch, #hiring and #personal. Areas help the weekly review spot neglected parts of life or work. Avoid tags for priority; the Today and This week sections already do that job.

## Privacy
Task files often contain names, client details and personal matters. Store them in a private folder or repository, avoid sharing the glossary publicly, and keep anything sensitive out of files that sync to shared tools.

## Working with calendars
Dated tasks and appointments belong in the calendar; the task file holds actions. When a task gets a time block, note the date beside it so the morning plan can see what is already scheduled.

## Recurring tasks
List recurring work, such as a weekly report or monthly invoices, in a short Recurring section with the rhythm and next due date. Each morning the agent copies due items into Today, so routine work never depends on memory.

## Setting up in different agents
In Claude Code or Codex, keep `TASKS.md` and `MEMORY.md` in the project or home folder the agent opens. In chat apps without file access, paste the files at the start of a session or store them in a connected drive. The structure stays the same everywhere, which keeps the system portable.

## When to simplify
If the files grow faster than the user can review them, cut sections, merge tags and archive old projects. A smaller list that is trusted beats a complete one that is ignored.

## Edge cases and judgement calls
| Situation | What to do |
|---|---|
| Hundreds of old tasks | Move anything older than 60 days to an archive; review later |
| Sensitive tasks or names | Keep them out of shared files; use initials if needed |
| Several agents or devices | One file in a synced folder or repository |
| Team tool required | Mirror personal tasks only; link to the team tool |
| User dislikes Markdown | Use the same structure in their notes app |

## Handoffs to related skills
- Audit first: `productivity-system-audit`
- Capturing from many sources: `task-capture-clarify`
- Choosing Today's tasks: `prioritisation`, `daily-planning`
- Weekly clean-up: `weekly-review`
- Notes and knowledge files: the Knowledge Management skills

## Worked example
An operations lead kept tasks in chat threads and sticky notes. The agent imported 46 items into `TASKS.md`, decoded 9 terms (including two project codenames and a recurring report acronym) into `MEMORY.md`, rewrote 18 vague items as next actions, moved 7 items to Waiting for with names and dates, and archived 11 stale ones. Each morning the agent proposes three priorities; after each meeting it adds actions from the notes. The lead reports spending five minutes a day on the list instead of chasing messages.

## Output format
```
1. TASKS.md (complete, ready to save)
2. MEMORY.md additions (people, terms, preferences)
3. Rules the agent will follow
4. Daily and weekly sync routines
5. Questions for terms still unknown
```

## Common mistakes
- Topics instead of next actions.
- Tasks in several files and apps.
- The agent changing priorities without asking.
- A glossary that grows into a diary.
- No weekly clean-up.

## Self-check before you answer
- Does every open task start with a verb?
- Is all shorthand decoded or asked about?
- Are the update rules clear?
- Is the system light enough to keep up daily?

---
Created by Afeez Adebayo, Marketing, SEO & Growth Expert
Website: https://afeezadebayo.com
LinkedIn: https://www.linkedin.com/in/afeez-adebayo/
X: https://x.com/za_icon
Source: https://afeezadebayo.com/skills-md/productivity/planning-tasks/task-system-setup/

Licence: CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/). You may copy, share and adapt this skill, including for commercial use, as long as you credit Afeez Adebayo and link to the source URL above. Keep this notice in any copy or adapted version.
