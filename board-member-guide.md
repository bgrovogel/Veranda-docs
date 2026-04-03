# Veranda — Board Member Guide

> How to use Veranda as a board member or board administrator.

**Status:** Current | **Last verified:** 2026-04-02

---

## Quick Links

- [Getting Started](#getting-started)
- [Your Dashboard](#your-dashboard)
- [Managing Violations](#managing-violations)
- [Posting Announcements](#posting-announcements)
- [Managing Documents](#managing-documents)
- [Managing Members](#managing-members)
- [Community Settings (board_admin only)](#community-settings-board_admin-only)
- [Notifications](#notifications)
- [Legal Notice](#legal-notice)

---

## Getting Started

You'll receive an email invitation from your community's board admin. The link is valid for 7 days.

**Accepting your invitation:**

1. Click the link in the invitation email
2. Enter your name and create a password (minimum 8 characters, uppercase + lowercase + digit)
3. Verify your email address with the 6-digit code sent to you
4. You're taken to the board dashboard

**Logging in after setup:**

- Go to your community's Veranda login page
- Enter your email and password
- You'll land on `/board/dashboard`

**Forgot your password?** Click "Forgot password?" on the login page and follow the reset link sent to your email.

---

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
| `waived`             | Board waived it (board admin only)       |

### Confirming resolution

When a homeowner submits resolution photos:

1. You receive an in-app notification
2. Open the violation → review the submitted photos
3. Click **Mark Resolved** → add optional notes → **Confirm**

### Closing or waiving a violation

| Action | When to use                                          | Who              |
| ------ | ---------------------------------------------------- | ---------------- |
| Close  | Resolved informally, withdrawn, no longer applicable | Any board member |
| Waive  | Board chooses not to enforce this specific violation | Board admin only |

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

## Managing Members

### Inviting a board member

1. Go to **Members** → click **Invite Board Member**
2. Enter their email, first name, and last name
3. Select role:
   - **Board Member** — can create violations, invite homeowners, manage documents and announcements
   - **Board Admin** — all Board Member permissions plus: change roles, deactivate accounts, waive violations, edit community settings
4. Click **Send Invite**

### Inviting a homeowner

1. Go to **Units** → find the unit → click **Invite Resident**
2. Enter their email, first name, and last name
3. Select role: **Homeowner** or **Tenant**
4. Click **Send Invite**

**Resending invitations:** Go to **Units** → scroll to **Pending Invitations** → click **Resend** next to the homeowner's name.

### Changing a member's role

Board admins can change roles:

1. Go to **Members** → find the person
2. Use the role dropdown to change their role
3. Change takes effect immediately

### Deactivating a member

Board admins can deactivate accounts:

1. Go to **Members** → find the person → click **Deactivate**
2. Confirm the action

The member loses access immediately. Their history (violations, actions) is preserved.

---

## Community Settings (board_admin only)

Go to **Settings** to configure:

- Community **name, address, phone, and website**
- **Property label** — how properties are labeled throughout the app (Unit, Lot, Home, or Property)
- **Default cure period** — how many days homeowners have to resolve a violation (typically 14–30 days)
- **Violation categories** — add, edit, or reorder the violation types available in your community

---

## Notifications

You receive notifications for:

- Homeowner submits resolution photos on a violation
- Email change request submitted by a community member (requires board admin approval)

**Notification bell:** The bell icon in the top navigation shows your unread notification count. Click it to see recent notifications and mark them as read.

**Your notification preferences:** Go to **Settings** → Notifications to enable or disable email and push notifications for specific events.

**Push notifications on mobile:** When you first visit Veranda, your browser will ask for notification permission. On Android (Chrome), you can install Veranda to your home screen as a PWA for an app-like experience. On iOS Safari, use "Add to Home Screen."

---

## Legal Notice

Veranda is a software tool, not legal counsel. All enforcement settings are configured by your board based on your governing documents. Verify enforcement requirements with your HOA attorney.

_Last updated: 2026-04-02_
