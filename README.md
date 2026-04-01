# 🤖 Bizzed AI Employee

An AI coworker for Bizzed built on Claude CoWork. Qualifies leads, books meetings, drafts proposals, and manages your sales pipeline — connected to Gmail, Google Calendar, and Notion.

---

## Installation

1. Download as zip file or clone this plugin folder
2. Open **Claude CoWork** and go to **Customize → Personal Plugins**
3. Click **Add Plugin → Create Plugin → Upload Plugin** and select the `AI-Employee` zip file
4. Connect the required integrations (see below)

### Required Integrations

| Integration | Purpose |
|---|---|
| Gmail | Read emails, send messages |
| Google Calendar | Check availability, create events |
| Notion | Read and update leads/deals in Notion |

Go to **Settings → Integrations** in CoWork and connect all three.

---

## Commands

### `/morning-brief`
Scans your emails, calendar, and CRM. Gives you a prioritised daily brief in 90 seconds.

```
/morning-brief
```

---

### `/qualify-lead`
Scores a lead out of 15 using Budget, Authority, Need, Timeline, and Fit. Tells you exactly what to do next.

```
/qualify-lead Sarah Jones
/qualify-lead [paste their email here]
/qualify-lead                          ← grabs latest unqualified lead from Notion
```

**Score guide:** 12–15 = Hot · 8–11 = Warm · 4–7 = Cold · 0–3 = Poor fit

---

### `/book-meeting`
Checks real calendar availability, proposes 3 time slots, drafts the email, and sends on your approval. Creates the calendar event and updates CRM automatically.

```
/book-meeting Sarah Jones discovery call
/book-meeting James from Acme demo this week
```

**Meeting types:** Discovery call (20 min) · Product demo (30 min) · Financing consultation (45 min) · Partnership call (30 min)

---

### `/follow-up`
Writes a follow-up that doesn't sound like a follow-up. Checks CRM history and picks the right approach based on which follow-up number this is.

```
/follow-up Sarah Jones
/follow-up James extra context: raised budget concerns last time
```

**Follow-up types:** #1 (3 days) adds value · #2 (7 days) asks one yes/no · #3 (14+ days) closes the loop gracefully

---

### `/draft-proposal`
Writes a personalised deal-specific follow-up proposal after a demo or discovery call.

```
/draft-proposal Sarah Jones
/draft-proposal James [paste discovery call notes]
```

---

### `/summarise-thread`
Reads a full email thread and extracts what was discussed, what was agreed, what's unresolved, and what needs to happen next.

```
/summarise-thread Sarah Jones
/summarise-thread [paste the email thread here]
```

---

### `/pipeline-report`
Pulls the full Notion pipeline. Flags hot leads, stalled deals, and overdue actions. Recommends 3 specific actions for the week.

```
/pipeline-report
```

---

## Skills (Knowledge Bases)

The plugin comes with 5 built-in knowledge bases that inform every command.

| Skill | What it contains |
|---|---|
| `company-context` | What Bizzed does, pricing model, traction, ideal customers, rules the AI must never break |
| `lead-qualification` | The 5-factor scoring framework (Budget, Authority, Need, Timeline, Fit) |
| `sales-process` | Step-by-step from first contact → discovery → demo → financing conversion |
| `scheduling` | Working hours, meeting durations, buffer rules, how to propose times |
| `tone-of-voice` | British English, short paragraphs, no jargon, always reference the prospect's specific deal |

---

## How it works

- Every command **shows you a draft before doing anything** — nothing is sent or updated without your approval
- If a contact is already in Notion, just use their name — the plugin pulls the rest automatically
- All actions (emails sent, meetings booked, follow-ups logged) are recorded in Notion automatically

---

## Typical daily workflow

```
Morning   → /morning-brief          See what needs attention
New lead  → /qualify-lead [name]    Score them, decide next step
Hot lead  → /book-meeting [name]    Get them booked in
Post-call → /draft-proposal [name]  Send a personalised follow-up
No reply  → /follow-up [name]       Chase at the right time
Weekly    → /pipeline-report        Review the full picture
```

---

## Author

Built by **Subash Sunuwar** 