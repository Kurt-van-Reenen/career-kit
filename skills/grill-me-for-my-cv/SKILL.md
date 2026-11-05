---
name: grill-me-for-my-cv
description: Interview the user in depth, in any profession or industry, to build or update their master CV, the complete record of their career that tailored CVs are cut from. Use when the user wants to create, rebuild or add to their base or master CV.
---

# Grill me for my CV

The goal is one file: `master-cv.md`, the single source of truth about the user's career. It is deliberately longer and more detailed than any CV that gets sent out. The `gen-me-a-cv` and `get-me-that-job` skills read from it, so always stick to the format at the bottom of this file.

This works for any profession: nurse, electrician, accountant, teacher, chef, sales rep, developer, graduate with no experience yet. Never assume the field. Find out, then adapt.

## Before starting

- Look for an existing master CV: an attached file, a project file, or `data/master-cv.md` / `master-cv.md` in the working folder.
- **Update mode** (one exists): read it, summarise what is there in a few lines, and ask what has changed or what feels thin. Only grill the gaps and the `## Open questions` section.
- **Build mode** (none exists): if the user has an old CV or a LinkedIn export, ask for it first and use it as the skeleton so they don't retype what already exists.

## First, understand their world

Before grilling roles, ask a short round of questions:

- What do you do, or want to do? (profession, field, level)
- Which country or countries are you applying in? (CV norms differ: length, photos, ID numbers, references)
- Is there anything your field always asks for? Examples: professional registration or licence numbers, trade certificates, security clearance, a portfolio, publications, client list, sales figures, case load.

Use the answers to adapt every later question. A chef gets asked about covers per service and kitchen brigade size; a teacher about class sizes, subjects and pass rates; a salesperson about targets and quota attainment. When unsure what matters in their field, ask them rather than guessing.

## How to grill

- Ask at most 3 questions at a time, grouped by topic. Never send a 20-question form.
- Work one role at a time, most recent first.
- Push past vague answers. "Helped customers" becomes: how many, what kind, what problems, what changed because of you, what would have gone wrong without you?
- Hunt for numbers, in whatever form fits the field: people managed or trained, customers or patients served, budgets handled, revenue or savings, volumes produced, targets hit, time saved, ratings or scores, deadlines met. If they don't know exact figures, accept honest estimates and mark them with `~`.
- For the best 3 to 5 achievements in each role, get the full story (Situation, Task, Action, Result). These feed interview prep later.
- Capture the tools, equipment, systems, methods and techniques used in each role, so it is clear how recent each skill is.
- Count everything that counts: volunteering, side work, freelancing, caring responsibilities, career breaks and study. Gaps are recorded honestly, with what was done during them.
- Never invent, inflate or assume. If something is unclear, ask. Mark anything unconfirmed with `[?]`.
- After each role, play back a short summary and ask "anything wrong or missing?" before moving on.
- Stopping halfway is fine. Save what exists and note where you left off under `## Open questions`.

## Finishing

- Save or deliver `master-cv.md`.
- List the weakest spots (roles with no numbers, skills with no evidence) as things to grill next time.
- Remind the user the file holds personal details, so it belongs somewhere private, never in a public repo.

## Output format (master-cv.md)

Leave out sections that don't apply to this person, and add any their field needs.

```markdown
# Master CV: {Full name}
_Last updated: {YYYY-MM-DD}_

## Profile
- Profession / field:
- Level:
- Target roles:
- Countries applying in:

## Contact
- Email:
- Phone:
- Location:
- Links: (LinkedIn, portfolio, professional profiles, website)

## Headline options
- {2 to 4 one-line positioning statements, each aimed at a different type of role}

## Summary bank
### {Angle, e.g. specialist, manager, career changer}
{3 to 4 line summary}

## Skills
| Skill, tool or method | Level (1-5) | Years | Last used | Evidence (role or project) |
|-----------------------|-------------|-------|-----------|----------------------------|

## Experience
### {Job title}, {Organisation} ({MM/YYYY} to {MM/YYYY})
- **Context:** what the organisation does, team size, setting
- **Responsibilities:**
- **Achievements:** (a number on each one where possible)
- **Tools, systems and methods:**
- **STAR stories:**
  - **{Short title}:** S: ... T: ... A: ... R: ...
- **Why I left:**

## Career breaks
## Projects, volunteering, freelance or side work
## Education
## Licences, registrations, certifications and memberships
## Publications, awards or portfolio items
## Languages
## Other (driver's licence, availability, references, interests worth mentioning)
## Preferences (role types, salary expectations, work setup, location, notice period, deal-breakers)
## Open questions
```
