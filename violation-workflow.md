# Livenhood — Violation Workflow

> Step-by-step guide for board administrators managing the full violation lifecycle in Livenhood.

**Status:** Current | **Last verified:** 2026-04-02

---

## Quick Links

- [Violation States](#violation-states)
- [Step 1 — Create a Violation](#step-1-create-a-violation)
- [Step 2 — Send the First Notice](#step-2-send-the-first-notice)
- [Step 3 — Monitor the Cure Period](#step-3-monitor-the-cure-period)
- [Step 4a — Confirm Resolution](#step-4a-confirm-resolution-violation-cured)
- [Step 4b — Send Second Notice](#step-4b-send-second-notice-not-cured)
- [Step 4c — Close or Waive](#step-4c-close-or-waive)
- [Audit Trail](#audit-trail)
- [Notice Delivery Tracking](#notice-delivery-tracking)
- [Tips for Compliance](#tips-for-compliance)
- [Configuring Violation Categories](#configuring-violation-categories)

---

## Violation States

```
open → first_notice_sent → second_notice_sent → resolved / closed / waived
```

| Status               | Meaning                                                      |
| -------------------- | ------------------------------------------------------------ |
| `open`               | Violation recorded; no notice sent yet                       |
| `first_notice_sent`  | First formal notice emailed to homeowner; cure timer running |
| `second_notice_sent` | Second notice sent after cure period expired                 |
| `resolved`           | Homeowner corrected the violation; board confirmed           |
| `closed`             | Board closed the violation (no resolution required)          |
| `waived`             | Board waived the violation _(board admin only)_              |

---

## Step 1: Create a Violation

1. Go to **Violations** in your board dashboard
2. Click **New Violation** (or tap **Inspect** to start from an inspection view)
3. Fill in:
   - **Unit** — search by address or unit number
   - **Category** — select from your community's violation types (e.g., landscaping, parking, exterior maintenance)
   - **Description** — describe what you observed
   - **Photos** — attach 1–4 photos from your phone or computer
   - **Rule violated** — cite the specific CC&R or rule section _(optional but recommended)_
4. Click **Submit**

> The violation is now `open`. The homeowner is **not notified yet** — only when you send a formal notice.

---

## Step 2: Send the First Notice

When you're ready to send formal notice to the homeowner:

1. Open the violation
2. Click **Send First Notice**
3. Review the notice preview — Livenhood generates a formatted PDF with:
   - Your community letterhead
   - The violation description and photos
   - The rule cited
   - The cure deadline _(typically 30 days — configurable in Settings)_
4. Click **Send**

**What happens automatically:**

- PDF is generated and stored
- Homeowner receives an **email** with the PDF attached
- Homeowner receives a **push notification** (if they have the app)
- Violation status changes to `first_notice_sent`
- Cure deadline **timer starts** in the background

---

## Step 3: Monitor the Cure Period

During the cure period:

- The violation detail page shows a **countdown timer**
- If the homeowner submits resolution photos, you'll receive an **in-app notification**
- You can add **internal notes** to the violation at any time

> **The homeowner's view:** They can see the violation in their portal, download the notice PDF, and submit resolution photos with a description.

---

## Step 4a: Confirm Resolution (Violation Cured)

When the homeowner has corrected the violation:

1. Open the violation
2. Review any **resolution photos** the homeowner submitted
3. If satisfied, click **Mark Resolved**
4. Add optional resolution notes
5. Click **Confirm**

> The violation status changes to `resolved`. Both you and the homeowner will see it marked as closed in your respective portals.

---

## Step 4b: Send Second Notice (Not Cured)

If the cure deadline passes without resolution:

1. Open the violation
2. Review the situation
3. Click **Send Second Notice** to escalate

> Fine assessment is coming in Phase 2. It is not available in the current version.

---

## Step 4c: Close or Waive

| Action    | When to use                                                       | Who can do it     |
| --------- | ----------------------------------------------------------------- | ----------------- |
| **Close** | Violation resolved informally, withdrawn, or no longer applicable | Any board member  |
| **Waive** | Board chooses not to enforce this specific violation              | Board admins only |

> Waived violations are recorded in the **audit trail** with the reason.

---

## Audit Trail

Every action on a violation is logged with a **timestamp** and the **name of the board member** who took the action. This includes:

- When the violation was created
- When each notice was sent
- Who confirmed resolution
- Who waived or closed it

To view: Open a violation → **Audit Trail** tab.

> This record is **immutable** and is your legal documentation if a dispute arises.

---

## Notice Delivery Tracking

Livenhood tracks whether the homeowner **opened** the violation notice email (via a tracking pixel).

To view: Open a violation → **Notices** tab → See delivery status and open timestamp for each notice sent.

> If the homeowner claims they never received the notice, you have **documented proof** of delivery and open time.

---

## Tips for Compliance

1. **Always cite the rule.** Including the specific CC&R or rule section strengthens your position if a homeowner disputes the violation.
2. **Take photos before and after.** Courts and arbitrators want to see the problem and its resolution.
3. **Send notices promptly.** Delays between observation and notice can weaken your enforcement position.
4. **Enforce consistently.** Enforce the same rules the same way for every homeowner. Selective enforcement is a common HOA legal liability.
5. **Keep the cure period reasonable.**

| Violation Type   | Recommended Cure Period |
| ---------------- | ----------------------- |
| Minor violations | 14–30 days              |
| Safety hazards   | 7 days                  |
| Major repairs    | 60+ days                |

---

## Configuring Violation Categories

To customize the violation types available in your community:

1. Go to **Settings** in your board dashboard
2. Select **Violation Categories**
3. Add, edit, or reorder categories

**Common categories:** Landscaping · Parking · Exterior Paint · Fence/Gate · Trash Cans · Noise · Pets · Short-Term Rental · Exterior Storage

---

_Last updated: 2026-04-02_
