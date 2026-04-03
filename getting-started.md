# Veranda — Getting Started

> New board admin guide: first login, community setup, and inviting homeowners.

**Status:** Current | **Last verified:** 2026-04-02

---

## Quick Links

- [Step 1 — Accept Invitation or Self-Register](#step-1-accept-your-invitation-or-self-register)
- [Step 2 — Explore the Board Dashboard](#step-2-explore-the-board-dashboard)
- [Step 3 — Add Your Units](#step-3-add-your-units)
- [Step 4 — Invite Homeowners](#step-4-invite-homeowners)
- [Step 5 — Invite Board Members](#step-5-invite-board-members)
- [Step 6 — Configure Community Settings](#step-6-configure-community-settings)
- [Common First-Day Questions](#common-first-day-questions)

---

## Step 1: Accept Your Invitation or Self-Register

### If you received an invitation email

1. Click the link in the invitation email — it opens the Veranda signup page
2. Enter your name and set a password _(minimum 8 characters, uppercase + lowercase + digit)_
3. A verification email is sent to your address — click the link to verify
4. You're redirected to your board dashboard

### If you're setting up a new HOA on Veranda

1. Go to the Veranda login page and click **"Setting up a new HOA? Start for free →"**
2. **Step 1 — Account:** Enter your name, email, and password; click **Continue**
3. **Step 2 — Verify:** Check your email for a 6-digit code and enter it
4. **Step 3 — Community:** Enter your HOA name, address, state, and timezone; click **Complete Setup**
5. You're redirected to your board dashboard as the **board admin**

---

## Step 2: Explore the Board Dashboard

After logging in you'll see the board dashboard at `/board/dashboard`. It shows:

- Open, in-progress, and resolved **violation counts**
- **Recent violations** list
- Quick navigation to all board features

The left sidebar (desktop) or bottom navigation (mobile) gives access to:

| Section           | What it does                          |
| ----------------- | ------------------------------------- |
| **Violations**    | Create, track, and resolve violations |
| **Units**         | Your property directory               |
| **Members**       | Board member management               |
| **Announcements** | Community-wide messages               |
| **Documents**     | CC&Rs, bylaws, meeting minutes        |
| **Settings**      | Community profile                     |

---

## Step 3: Add Your Units

> Before inviting homeowners, you need your unit directory set up.

### Option A: Add units one at a time

1. Go to **Units** → click **Add Unit**
2. Enter the address, unit number, and optional lot size
3. Click **Save**

### Option B: Bulk import from CSV _(recommended for 5+ units)_

1. Go to **Units** → click **Bulk Import**
2. Download the sample CSV template
3. Fill in your units (address, unit number, owner email, first/last name)
4. Upload the CSV — up to **500 units** per import
5. Review the results — successful rows show green ✅, errors show red ❌ with the reason

**Sample CSV format:**

```csv
address,unitNumber,ownerEmail,ownerFirstName,ownerLastName,role
123 Oak Lane,101,jane@example.com,Jane,Smith,homeowner
456 Elm Street,102,bob@example.com,Bob,Jones,homeowner
```

See [importing-properties.md](./importing-properties.md) for the full CSV format and field descriptions.

---

## Step 4: Invite Homeowners

### Invite from the Units page

1. Go to **Units**
2. Click **Invite All Homeowners** for a bulk invite, or find a specific unit and click **Invite**
3. Homeowners receive an email with a signup link
4. They set a password and verify their email
5. Their account appears under the unit in your directory

### Invite an individual homeowner

1. Go to **Units** → find the unit → click the row to open unit detail
2. Click **Invite Resident**
3. Enter their email, first name, and last name
4. Click **Send Invite**

### Track pending invitations

The Units page shows a **Pending Invitations** section with all sent-but-not-accepted invites. From there you can **resend** or **revoke** invitations.

---

## Step 5: Invite Board Members

1. Go to **Members** → click **Invite Board Member**
2. Enter their email address
3. Choose their role:
   - **Board Member** — standard access
   - **Board Admin** — full access
4. Click **Send Invite**

> **Board Admins** can do everything including: deactivate users, change roles, waive violations, and manage community settings.

---

## Step 6: Configure Community Settings

Go to **Settings** to configure:

- Community **name, address, phone, and website**
- **Property label** (Unit, Lot, Home, or Property — shown throughout the app)
- **Default violation cure period** (how many days homeowners have to fix a violation)
- **Notification preferences**

---

## Common First-Day Questions

**Q: A homeowner says they didn't receive their invite.**
→ Go to **Units → Pending Invitations** → find their name → click **Resend**.

**Q: I imported units but the homeowner emails were wrong. How do I fix it?**
→ Re-import the CSV with corrected data. Existing units will be updated; a new invite will be sent to the corrected email.

**Q: Can I have multiple board admins?**
→ Yes. Invite board members and set their role to **Board Admin**. You can have as many as needed.

**Q: How do I remove someone's access?**
→ Go to **Members** → find the person → click **Deactivate**. They'll no longer be able to log in. Their history is preserved.

**Q: What's the difference between Board Admin and Board Member?**
→ Board Members can create violations, send notices, invite homeowners, and post announcements. Board Admins can do all of that **plus**: waive violations, change user roles, deactivate users, and edit community settings.

---

## Next Steps

- [violation-workflow.md](./violation-workflow.md) — full step-by-step violation lifecycle
- [faq.md](./faq.md) — additional common questions

---

_Last updated: 2026-04-02_
