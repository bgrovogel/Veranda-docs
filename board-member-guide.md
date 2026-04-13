# Livenhood — Board Member Guide

> How to use Livenhood as a board member or board officer.

**Status:** Current | **Last verified:** 2026-04-05

---

## Quick Start

### Step 1: Accept Your Invitation or Self-Register

If you received an invitation email:

1. Click the link in the invitation email — it opens the Livenhood signup page
2. Enter your name and set a password (minimum 8 characters, uppercase + lowercase + digit)
3. A verification email is sent to your address — click the link to verify
4. You're redirected to your board dashboard

If you're setting up a new HOA on Livenhood:

1. Go to the Livenhood login page and click **"Setting up a new HOA? Start for free →"**
2. **Step 1 — Account:** Enter your name, email, and password; click **Continue**
3. **Step 2 — Verify:** Check your email for a 6-digit code and enter it
4. **Step 3 — Community:** Enter your HOA name, address, state, and timezone; click **Complete Setup**
5. You're redirected to your board dashboard as the **board officer**

### Step 2: Explore the Board Dashboard

After logging in you'll see the board dashboard at `/hoa/dashboard`. It shows:

- Open, in-progress, and resolved **violation counts**
- **Recent violations** list
- Quick navigation to all board features

The left sidebar (desktop) or bottom navigation (mobile) gives access to:
| Section | What it does |
| ----------------- | ------------------------------------- |
| **Violations** | Create, track, and resolve violations |
| **Units** | Your property directory |
| **Members** | Board member management |
| **Announcements** | Community-wide messages |
| **Documents** | CC&Rs, bylaws, meeting minutes |
| **Forms** | Fill out and generate PDF forms |
| **Payments** | Connect bank account, configure dues collection |
| **Settings** | Community profile |

### Step 3: Add Your Units

Before inviting homeowners, you need your unit directory set up.

**Option A: Add units one at a time**

1. Go to **Units** → click **Add Unit**
2. Enter the address, unit number, and optional lot size
3. Click **Save**

**Option B: Bulk import from CSV (recommended for 5+ units)**

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

See [importing-properties.md](../clients/importing-properties.md) for the full CSV format and field descriptions.

### Step 4: Invite Homeowners

**Invite from the Units page**

1. Go to **Units**
2. Click **Invite All Homeowners** for a bulk invite, or find a specific unit and click **Invite**
3. Homeowners receive an email with a signup link
4. They set a password and verify their email
5. Their account appears under the unit in your directory

**Invite an individual homeowner**

1. Go to **Units** → find the unit → click the row to open unit detail
2. Click **Invite Resident**
3. Enter their email, first name, and last name
4. Click **Send Invite**

**Track pending invitations**
The Units page shows a **Pending Invitations** section with all sent-but-not-accepted invites. From there you can **resend** or **revoke** invitations.

### Step 5: Invite Board Members

1. Go to **Members** → click **Invite Board Member**
2. Enter their email address
3. Choose their role:
   - **Board Member** — standard access
   - **Board Officer** — full access
4. Click **Send Invite**

> **Board Officers** can do everything including: deactivate users, change roles, waive violations, and manage community settings.

### Step 6: Configure Community Settings

Go to **Settings** to configure:

- Community **name, address, phone, and website**
- **Property label** (Unit, Lot, Home, or Property — shown throughout the app)
- **Default violation cure period** (how many days homeowners have to fix a violation)
- **Notification preferences**

### Common First-Day Questions

**A homeowner says they didn't receive their invite.**
→ Go to **Units → Pending Invitations** → find their name → click **Resend**.

**I imported units but the homeowner emails were wrong. How do I fix it?**
→ Re-import the CSV with corrected data. Existing units will be updated; a new invite will be sent to the corrected email.

**Can I have multiple board officers?**
→ Yes. Invite board members and set their role to **Board Officer**. You can have as many as needed.

**How do I remove someone's access?**
→ Go to **Members** → find the person → click **Deactivate**. They'll no longer be able to log in. Their history is preserved.

**What's the difference between Board Officer and Board Member?**
→ Board Members can create violations, send notices, invite homeowners, and post announcements. Board Officers can do all of that **plus**: waive violations, change user roles, deactivate users, and edit community settings.

---

## Quick Links

...existing code...

## Your Dashboard

The board dashboard shows at a glance:

- Open violation count — violations not yet resolved
- In-progress violation count — notices sent, cure period running
- Resolved violation count
- Recent violations list with unit address and status

The sidebar (desktop) or bottom navigation (mobile) gives access to all board features:

| Section       | What it does                          |
| ------------- | ------------------------------------- |
| Violations    | Create, track, and resolve violations |
| Units         | Your property directory               |
| Members       | Board member management               |
| Announcements | Community-wide messages               |
| Documents     | CC&Rs, bylaws, meeting minutes        |
| Forms         | Fill out and generate PDF forms       |
| Payments      | Connect bank account, configure dues  |
| Settings      | Community and profile settings        |

---

## Managing Violations

### Creating a violation

1. Go to **Violations** → click **New Violation**
2. Fill in:
   - **Unit** — search by address or unit number
   - **Category** — violation type (landscaping, parking, exterior, etc.)
   - **Description** — what you observed
   - **Photos** — attach 1–4 photos
   - **Rule cited** — the CC&R or rule section (optional but strongly recommended)
3. Click **Submit**

The violation is now `open`. The homeowner is not notified yet.

### Sending notices

**Send First Notice:**

1. Open the violation → click **Send First Notice**
2. Review the auto-generated PDF (includes your community letterhead, description, photos, cure deadline)
3. Click **Send**

What happens automatically:

- PDF is generated and stored
- Homeowner receives an email with the PDF attached
- Homeowner receives a push notification (if installed)
- Status changes to `first_notice_sent`
- Cure deadline timer starts

**Send Second Notice:**
If the cure deadline passes without resolution, open the violation and click **Send Second Notice**.

### Violation states

| Status               | Meaning                                  |
| -------------------- | ---------------------------------------- |
| `open`               | Violation recorded, no notice sent       |
| `first_notice_sent`  | First notice sent, cure timer running    |
| `second_notice_sent` | Second notice sent after deadline passed |
| `resolved`           | Homeowner corrected it, board confirmed  |
| `closed`             | Board closed it (any board member)       |
| `waived`             | Board waived it (board officer only)     |

### Confirming resolution

When a homeowner submits resolution photos:

1. You receive an in-app notification
2. Open the violation → review the submitted photos
3. Click **Mark Resolved** → add optional notes → **Confirm**

### Closing or waiving a violation

| Action | When to use                                          | Who                |
| ------ | ---------------------------------------------------- | ------------------ |
| Close  | Resolved informally, withdrawn, no longer applicable | Any board member   |
| Waive  | Board chooses not to enforce this specific violation | Board officer only |

Both actions are recorded in the audit trail with a timestamp and your name.

### Audit trail

Every action on a violation is logged permanently. To view: open a violation → **Audit Trail** tab.

The audit trail records: who created the violation, when each notice was sent, who confirmed resolution, who closed or waived it. This is your documentation if a homeowner dispute arises.

---

## Posting Announcements

Announcements reach all registered homeowners via email and push notification.

**Create an announcement:**

1. Go to **Announcements** → click **New Announcement**
2. Write a title and message body
3. Click **Publish**

All active homeowners receive an email and push notification immediately.

**Pinning an announcement:**

- Pinned announcements appear at the top of the announcements list for all homeowners
- Click the pin icon on any announcement to toggle it

**Archiving:**

- Archived announcements are hidden from the main list but remain accessible under the **Archive** tab
- You can restore an archived announcement at any time

---

## Managing Documents

The document library stores your community's governing documents, meeting minutes, forms, and notices.

**Uploading a document:**

1. Go to **Documents** → click **Upload**
2. Select the file (PDF, JPEG, PNG, or Word .docx — max 50MB)
3. Choose a category and set visibility (Public or Board Only)
4. Click **Save**

**Categories:** CC&Rs, Bylaws, Meeting Minutes, Budget, Rules & Regulations, Forms, Notices, Other.

**Access levels:**

- **Public** — visible to all registered homeowners
- **Board Only** — visible to board members only

---

## Forms

The Forms section provides fillable templates for common HOA documents. Completed forms are generated as downloadable PDFs.

**Finding Forms in the sidebar:**

Forms appear in the **Content** section of the sidebar, between **Documents** and the next item. On mobile, look for **Forms** in the bottom navigation.

**Available templates:**

| Template                           | Who can access              | Purpose                                              |
| ---------------------------------- | --------------------------- | ---------------------------------------------------- |
| Board Authorization Form (BAF)     | board_officer, board_member | Required for HOA verification on the platform        |
| Architectural Change Request (ACR) | board_officer, board_member | Review submitted requests for exterior modifications |
| Violation Acknowledgment           | board_officer, board_member | Formal covenant violation notice                     |
| Variance Request                   | board_officer, board_member | Request to grant an exception to a CC&R rule         |

**Filling out a form:**

1. Go to **Forms** — the library shows all templates available to your role
2. Click a template card to open it
3. Fill in all required fields (marked with an asterisk)
4. The PDF preview on the right updates in real time as you type
5. Click **Generate PDF** to produce the final document
6. Click **Download** to save the PDF to your device

**Customizing templates (board_officer only):**

Board officers can customize any template and control homeowner access:

1. Open the template from the Forms library
2. Click **Customize** (top right of the form page)
3. **Homeowner Access toggle** — enable to allow homeowners to see and fill this template from their portal; disable to restrict it to board members only
4. Add or edit the instructions block — this text appears at the top of generated PDFs for your community
5. Override field labels and upload a community logo
6. Click **Save**

**Draft auto-save:** When filling out a form, field values are automatically saved every few seconds. Previously generated PDFs appear in a **Previously Generated** section at the bottom of the form page.

---

## Managing Members

### Inviting a board member

1. Go to **Members** → click **Invite Board Member**
2. Enter their email, first name, and last name
3. Select role:
   - **Board Member** — can create violations, invite homeowners, manage documents and announcements
   - **Board Officer** — all Board Member permissions plus: change roles, deactivate accounts, waive violations, edit community settings
4. Click **Send Invite**

### Inviting a homeowner

1. Go to **Units** → find the unit → click **Invite Resident**
2. Enter their email, first name, and last name
3. Select role: **Homeowner** or **Resident**
4. Click **Send Invite**

**Resending invitations:** Go to **Units** → scroll to **Pending Invitations** → click **Resend** next to the homeowner's name.

### Changing a member's role

Board officers can change roles:

1. Go to **Members** → find the person
2. Use the role dropdown to change their role
3. Change takes effect immediately

### Deactivating a member

Board officers can deactivate accounts:

1. Go to **Members** → find the person → click **Deactivate**
2. Confirm the action

The member loses access immediately. Their history (violations, actions) is preserved.

---

## Dues & Payments (board_officer only)

Go to **Payments** to set up online dues collection via Stripe Connect.

### Connecting your bank account

1. Go to **Payments** → click **Set Up Payments →**
2. You'll be redirected to Stripe's hosted onboarding flow
3. Enter your HOA's banking details (Stripe handles all compliance)
4. Complete identity verification as required by Stripe
5. You're redirected back to Livenhood when setup is complete

Once connected, homeowners can pay dues online via bank transfer (ACH) or credit/debit card. Your HOA receives payments directly — Livenhood never holds your funds.

If you leave the Stripe onboarding flow early, come back to **Payments** and click **Resume Setup →**.

### Fee configuration (after connecting)

Once your bank account is connected, you can configure how fees work:

**Who pays the Technology Fee ($2.95)**

| Option         | What it means                                                                                     |
| -------------- | ------------------------------------------------------------------------------------------------- |
| Homeowner Pays | The $2.95 Technology Fee and any card/ACH processing costs are shown to the homeowner at checkout |
| HOA Absorbs    | Processing costs are deducted from the collected amount — homeowners see no fees                  |

**Accepted payment methods**

- **Bank Transfer (ACH)** — always enabled (legally required baseline option)
- **Credit & Debit Cards** — enabled by default; you can turn this off if your board prefers ACH-only

**Check mailing address**

Enter the address homeowners should mail paper checks to. This is shown on every checkout screen as the fee-free payment option.

After changing any settings, click **Save Fee Settings**.

### Disconnecting

To disconnect your Stripe account, go to **Payments → Stripe Connection → Disconnect**. You'll be asked to confirm. After disconnecting, online payments stop until you reconnect.

> **Dues collection detail and transaction history** are coming in the next update.

---

## Community Settings (board_officer only)

Go to **Settings** to configure:

- Community **name, address, phone, and website**
- **Property label** — how properties are labeled throughout the app (Unit, Lot, Home, or Property)
- **Default cure period** — how many days homeowners have to resolve a violation (typically 14–30 days)
- **Violation categories** — add, edit, or reorder the violation types available in your community

---

## Notifications

You receive notifications for:

- Homeowner submits resolution photos on a violation
- Email change request submitted by a community member (requires board officer approval)

**Notification bell:** The bell icon in the top navigation shows your unread notification count. Click it to see recent notifications and mark them as read.

**Your notification preferences:** Go to **Settings** → Notifications to enable or disable email and push notifications for specific events.

**Push notifications on mobile:** When you first visit Livenhood, your browser will ask for notification permission. On Android (Chrome), you can install Livenhood to your home screen as a PWA for an app-like experience. On iOS Safari, use "Add to Home Screen."

---

## Two-Factor Authentication

Board members and officers are strongly encouraged to enable MFA. Go to **Settings → Security → Two-Factor Authentication** and click **Set up →**. Scan the QR code with an authenticator app (Google Authenticator, Authy, 1Password), enter the 6-digit code to verify, and save your recovery codes somewhere safe — they won't be shown again.

---

## Privacy & Data

As a community member, you have rights over your personal data under GDPR and CCPA — independent of your role as a board member. Go to **Settings** → **Privacy & Data** to submit and track your requests.

### Request types

| Request Type          | What it does                                                           |
| --------------------- | ---------------------------------------------------------------------- |
| Request My Data       | Access or portability — receive a ZIP export of all your personal data |
| Request Data Deletion | Erasure — request that your personal data be removed from Livenhood    |

### Submitting a request

1. Go to **Settings** → **Privacy & Data**
2. Click the request type you want to submit
3. Choose your regulation: **GDPR** (30-day SLA) or **CCPA** (45-day SLA)
4. Re-enter your password to confirm your identity
5. Click **Submit Request**

You can only have one active request per type at a time.

### Tracking your request

After submitting, the status tracker shows where your request is in the process:

| Status            | What it means                                                      |
| ----------------- | ------------------------------------------------------------------ |
| Received          | Your request has been logged and is awaiting platform admin review |
| Identity Verified | Your identity has been confirmed by the platform team              |
| Processing        | Your export is being generated or your erasure is being processed  |
| Completed         | The request is done — download your export or review the outcome   |
| Denied            | The request was denied — the reason is displayed on the page       |

### Downloading your export

When a data access or portability request is completed, a **Download Export** button appears. The download link expires in 7 days.

**Note:** Board members can view and manage their own data requests. The DSAR admin review queue at `/platform/dsar` is platform admin only — community boards do not have access to review other users' DSAR requests.

> Livenhood is a software tool, not legal counsel. Verify your data rights and any applicable requirements with your HOA attorney.

---

## Legal Notice

Livenhood is a software tool, not legal counsel. All enforcement settings are configured by your board based on your governing documents. Verify enforcement requirements with your HOA attorney.

_Last updated: 2026-04-08_
