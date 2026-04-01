---
description: Pull full CRM
  pipeline and flag what
  needs attention
---

# /pipeline-report

**Usage:** `/pipeline-report` — no arguments needed

**What it does:** Pulls the full pipeline from CRM, analyses where
every lead and deal stands, calculates key numbers, flags what needs
attention, and recommends specific actions for this week.

---

## Instructions

### Step 1 — Pull all data from CRM

Retrieve every open lead and deal with:
- Name and company
- Stage (New / Contacted / Demo Booked / Demo Done /
  Platform Signup / Financing Conversation / Won / Lost)
- Source (waitlist / referral / email / LinkedIn / other)
- Last activity date
- Next action and due date
- Acquisition target details if known
- Financing value if in financing stage

Also pull:
- Total waitlist count
- New signups in the last 7 days
- Demos booked this week
- Platform signups this week

### Step 2 — Analyse the pipeline

Calculate:
- Total leads by stage
- Number of hot leads (score 12+ or live deal in progress)
- Leads with no activity in 7 or more days — stalled
- Leads with overdue next actions
- Demos scheduled this week
- Total financing value in pipeline (Stage: Financing Conversation)

### Step 3 — Produce the report

---
BIZZED — PIPELINE REPORT
[Date]

HEADLINE NUMBERS
New waitlist signups (last 7 days): [X]
Active leads in pipeline: [X]
Demos booked this week: [X]
Platform signups this week: [X]
Total financing value in progress: £[X]

PIPELINE BY STAGE
New / Uncontacted:        [X] leads
Contacted:                [X] leads
Demo Booked:              [X] leads
Demo Done:                [X] leads
Platform Signup:          [X] leads
Financing Conversation:   [X] leads — £[X] total value

NEEDS ATTENTION
[Name] — [Stage] — Last activity [X] days ago — [Recommended action]
[Name] — [Stage] — Next action overdue by [X] days
[Name] — Hot lead — not yet contacted today

HOT LEADS THIS WEEK
[Name] — [Target business] — [Stage] — [Next step]

RECOMMENDED ACTIONS THIS WEEK
1. [Specific action on specific lead]
2. [Specific action on specific lead]
3. [Specific action on specific lead]
---

### Step 4 — Offer to act
"Would you like me to send follow-ups on any stalled leads,
draft outreach for the uncontacted waitlist signups,
or book demos for any of the hot leads above?"