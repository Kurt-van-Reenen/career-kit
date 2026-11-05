---
name: gen-me-a-cv
description: Generate a CV tailored to one specific job ad, in any profession, cut from the user's master CV. Use when the user shares a job ad, link or role description and wants a CV (and optionally a cover letter) for it.
---

# Gen me a CV

Turn the master CV plus one job ad into a short, targeted CV for that job. Everything comes from the master CV. This skill selects, orders and rewords. It never adds experience that isn't there.

Works for any profession. Never assume the field from the skill's examples; take it from the master CV and the ad.

## Inputs

1. **Master CV.** Find `master-cv.md` (attached, in project files, or `data/master-cv.md`). If there isn't one, stop and suggest running `grill-me-for-my-cv` first.
2. **The job ad.** Pasted text, a link (fetch it), or a description. If the ad is thin, ask for the company name and any extra info the user has (recruiter notes, salary band).
3. **Anything missing for this field.** If the ad asks for something the master CV doesn't cover (a registration number, a portfolio link, references, a specific certificate), ask the user for it rather than guessing or leaving it out silently.

## Step 1: Break down the ad

Before writing anything, show the user a short breakdown:

- **Must-haves:** hard requirements (years, qualifications, licences, specific tools or methods).
- **Nice-to-haves.**
- **Keywords:** exact terms an applicant tracking system (ATS) will likely scan for, spelled the way the ad spells them.
- **What they actually care about:** the problem this hire solves, read between the lines.
- **Match score:** each must-have marked as strong, partial or gap, with the evidence from the master CV.

Flag real gaps honestly. Ask one question: any experience not in the master CV that covers a gap? If yes, note it so it can be added to the master CV later.

## Step 2: Write the CV

- **Follow the norms of the field and country.** Length, section names and what to include differ: an academic CV can run long with publications; a trade CV leads with tickets and certificates; a creative CV links a portfolio; some countries expect a photo or ID details and others avoid them. If unsure, ask the user what is normal where they apply. Default: 2 pages, no photo.
- **Recent and relevant first.** Recent and relevant roles get detail; old or unrelated roles shrink to one line or go under "Earlier experience".
- **Headline and summary:** pick the closest one from the master CV's banks and adapt it to this role. Use the ad's wording where it is true.
- **Skills:** relevant ones first, matching the ad's spelling. Leave out skills that are stale or unrelated.
- **Bullets:** choose the achievements that prove the must-haves. Lead with a strong verb, include the number, end with the impact. 3 to 6 bullets for the latest role, fewer for older ones.
- **Keywords:** work them in naturally. No keyword stuffing, no hidden text.
- **ATS-safe layout:** single column, standard headings, no tables, text boxes, icons or images, dates in one consistent format.
- **Honesty:** never claim a skill, title, number, date or qualification that isn't in the master CV or confirmed by the user in this conversation.
- Follow any writing-style rules the user has set (for example, no em dashes).

## Step 3: Deliver

- Make the CV as a document the user can edit and export to PDF or Word. Make a .docx or PDF file directly only if they ask for that format.
- File or document name: `CV - {Full name} - {Company} - {Role}`.
- After the CV, give a short list of:
  - which gaps remain and how to address them (cover letter, interview, a course, a quick piece of work to show),
  - anything to add to the master CV next time.
- Offer a cover letter. If they want one: under 300 words, specific to the company, opens with why this role, uses one achievement as proof, no generic filler.
- Suggest running `get-me-that-job` next to prepare for the interview.
