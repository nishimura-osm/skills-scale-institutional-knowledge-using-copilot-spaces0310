# Retrospective Action Items Tracker

## Purpose
Record, assign, and track action items that come out of retrospectives. This ensures follow-through and closes the feedback loop between retrospectives and actual improvements.

## How to use
1. During the retro, agree on the **top 2–3 action items** (avoid overload).
2. For each item, copy the entry template below and fill it in.
3. After the retro, **create a GitHub Issue** for each action item:
   - Label it `retro-action` and assign it to the named owner.
   - Add it to the project board so it is visible alongside regular work.
4. Open the previous retro's action items section at the start of the next retro (the "Follow-up on previous action items" agenda item) and update their status.

## Cadence & Ownership
- **Frequency**: Retros are held after every sprint, major release, or significant incident.
- **Facilitator**: Rotating (default: PM schedules; any team member can facilitate).
- **Owner of follow-through**: PM tracks that all action-item issues are assigned and visible on the project board.
- **Review**: Action item status reviewed at every weekly PM sync until closed.

---

## Retro: _Sprint / Release Name_ — YYYY-MM-DD

### Attendees
_@mention, @mention, ..._

### What went well
- 
- 

### What could be improved
- 
- 

### Action Items

| # | Title | Description | Owner | Due Date | GitHub Issue | Status |
|---|---|---|---|---|---|---|
| 1 | | | @owner | YYYY-MM-DD | #issue | Open |
| 2 | | | @owner | YYYY-MM-DD | #issue | Open |
| 3 | | | @owner | YYYY-MM-DD | #issue | Open |

---

## Follow-up: Previous Action Items

_(Copy the table from the previous retro here and update statuses before the meeting.)_

| # | Title | Owner | Due Date | GitHub Issue | Status |
|---|---|---|---|---|---|
| | | | | | |

---

## Converting Action Items to GitHub Issues

When creating the GitHub Issue for an action item, use this body template:

```markdown
## Retro Action Item

**From retro**: [Sprint/Release name, YYYY-MM-DD]
**Owner**: @mention
**Due date**: YYYY-MM-DD

### Description
_What needs to happen?_

### Success Criteria
_How do we know this is done?_

### Notes
_Any context, links to retro notes, or related issues._
```

Label the issue `retro-action` and assign it to the owner.
