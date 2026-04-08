# Livenhood — FAQ

> Common questions from board officers, board members, and homeowners.

**Status:** Current | **Last verified:** 2026-04-05

---

## Quick Links

- [Getting Started](#getting-started)
- [Properties and Units](#properties-and-units)
- [Violations](#violations)
- [Announcements](#announcements)
- [Documents](#documents)
- [Members and Roles](#members-and-roles)
- [Notifications](#notifications)
- [Technical Questions](#technical-questions)
- [Legal Questions](#legal-questions)

---

## Getting Started

**How do I set up my community on Livenhood?**
Go to the Livenhood sign-up page and click **"Set up a new HOA."** You'll create your account, verify your email, and enter your community details (name, address, state). Once your account is created, you'll land on your board dashboard and can start adding units and inviting homeowners.

**How do I add units to my community?**
Go to **Units** → click **Add Unit** to add one at a time. For 5 or more units, use **Import CSV** for bulk import. See [importing-properties.md](../clients/importing-properties.md) for the CSV format and examples. Up to 500 properties per import.

**How do I invite homeowners?**
Go to **Units** → find the unit → click **Invite Resident**. Enter their email and name, select their role (Homeowner or Resident), and click **Send Invite**. For bulk invites, include owner email columns in your CSV import.

**How do I add board members?**
Go to **Members** in your board dashboard and click **Invite Board Member**. Enter their email address and select their role (Board Officer or Board Member). They'll receive an invitation email with a link to create their account.

**What roles are available?**

| Role              | Permissions                                                                                                        |
| ----------------- | ------------------------------------------------------------------------------------------------------------------ |
| **Board Officer** | Everything — create violations, change member roles, deactivate users, manage settings                             |
| **Board Member**  | Create violations, invite homeowners, manage documents and announcements. Cannot change roles or deactivate users. |
| **Homeowner**     | View their own violations, submit resolutions, view community documents and announcements                          |
| **Resident**      | Same as Homeowner                                                                                                  |

---

## Properties and Units

**Can I import all my properties at once?**
Yes — use the **Import CSV** button on the Properties page. See [importing-properties.md](../clients/importing-properties.md) for the required format and examples. Up to 500 properties per import.

**What if I have a unit that is rented (not owner-occupied)?**
Set the `role` column to `resident` in your CSV, or select **"Resident"** when inviting someone to a unit. Residents see the same homeowner portal as owners.

**Can I update a unit after it's created?**
Yes — click the unit in the Properties list and use the **Edit** button. You can update the address, lot number, and lot size.

**What happens when a property changes hands?**
Deactivate the previous owner from the Members page, then invite the new owner to that unit.

**How do I resend an invitation a homeowner missed?**
Go to **Properties** → scroll to **Pending Invitations** → find their name → click **Resend**. A new invitation link is sent and the old link is invalidated.

---

## Violations

**How does the violation process work?**

1. Board member **creates** a violation (unit, category, description, photo)
2. Board **sends First Notice** — Livenhood generates a PDF letter and emails the homeowner
3. A **cure period timer** starts automatically (typically 14–30 days)
4. If **resolved**: homeowner submits photos; board confirms resolution
5. If **not resolved**: board sends Second Notice
6. Board can **waive or close** the violation at any time

> Livenhood is a software tool, not legal counsel. Verify enforcement requirements with your HOA attorney.

**Do homeowners get notified automatically?**
Yes — when a notice is sent, the homeowner receives an **email** and a **push notification** (if they've installed the PWA on their phone).

**Can homeowners see their violations?**
Yes — homeowners see all violations for their unit when they log into their portal. They can submit resolution photos directly.

**How do I waive a violation?**
Open the violation and click **Waive**. Only board officers can waive violations. The audit trail records who waived it and when.

**Can I print a violation notice?**
Yes — violation notices are generated as PDF documents. Download them from the violation detail page under the **Notices** tab.

**Is fine assessment available?**
Fine assessment is coming in Phase 2 and is not available in the current version of Livenhood. Contact your HOA attorney regarding your community's fine policy and enforcement procedures.

**Can I edit a violation after it's created?**
You can add internal notes and photos at any time. The description and category can be edited while the violation is in `open` status. Once a notice is sent, the filed record is locked to preserve the legal record.

**What's the difference between Close and Waive?**
Any board member can close a violation (resolved informally, withdrawn, or no longer applicable). Only board officers can waive a violation (the board chooses not to enforce it). Both are recorded in the audit trail.

---

## Announcements

**How do I send a community-wide announcement?**
Go to **Announcements**, click **New Announcement**, write your message, and click **Publish**. All registered homeowners receive an email and push notification.

**Do all homeowners see announcements even if they haven't signed up for Livenhood?**
No — announcements are delivered to users with active Livenhood accounts. This is another reason to get all homeowners set up in the system.

**Can I schedule an announcement for later?**
Not in the current version. Announcements are published immediately when you click Publish.

**Can announcements be pinned or archived?**
Yes. Pinned announcements appear at the top of the list. Archived announcements are hidden from the main list but remain accessible under the Archive tab.

---

## Documents

**Who can see Board Only documents?**
Documents marked as Board Only are visible only to board members (board_officer and board_member roles). Homeowners and residents cannot see them.

**Can I see documents like CC&Rs and bylaws?**
Yes. Go to **Documents** to access all community documents marked as Public by your board.

**How do I upload a document?**
Go to **Documents** → click **Upload**. Select the file, choose a category, set visibility, and click Save.

---

## Members and Roles

**How do I add board members?**
Go to **Members** → click **Invite Board Member**. Enter their email address, select their role, and send the invite.

**How do I remove a board member or homeowner?**
Go to **Members** → find the person → click **Deactivate**. Only board officers can deactivate accounts. Their history is preserved; they lose access immediately. You cannot deactivate yourself.

**How do I change a member's role?**
Board officers can change roles: Go to **Members** → find the person → use the role dropdown to change their role. Change takes effect immediately.

**How do I resend an invitation?**
Go to **Units** → scroll to **Pending Invitations** → click **Resend** next to the homeowner's name.

---

## Notifications

**What notifications will I receive?**
You receive notifications for: homeowner submits resolution photos, email change requests, and other key events. The notification bell in the top navigation shows your unread count.

**How do I manage notification preferences?**
Go to **Settings** → Notifications to enable or disable email and push notifications for specific events.

**Why am I not receiving push notifications?**
Check that you have allowed notifications in your browser. On iOS, push notifications work in Safari with iOS 16.4 or later after adding Livenhood to your Home Screen. Email is always the primary notification channel — check your email if you're not receiving push notifications.

**Can I use Livenhood on a tablet?**
Yes. Livenhood is responsive and works on tablets in both portrait and landscape orientation.

---

## Technical Questions

**Do I need to download an app?**
No. Livenhood is a Progressive Web App (PWA). Access it from any browser on your phone or computer. On Android (Chrome) and iOS (Safari), you can install it to your home screen for an app-like experience — no app store required.

**What browsers does Livenhood support?**
Chrome, Safari, Firefox, and Edge — current and one version back. Chrome on Android is recommended for the best push notification experience on mobile.

**The app isn't loading. What should I try?**
Try a hard refresh (Ctrl+Shift+R on Windows, Cmd+Shift+R on Mac). Check your internet connection. If the problem persists, try logging out and logging back in.

**I'm logged out unexpectedly. Is this normal?**
Livenhood sessions expire for security. Log back in with your email and password. If you're being logged out frequently, check that your browser is not clearing cookies or local storage on close.

**The notification bell shows a count but clicking it shows nothing. What's happening?**
Click **Mark all as read** to clear the badge. If notifications are missing, try refreshing the page.

---

## Legal Questions

**Is Livenhood a legal document service?**
No. Livenhood is a software tool for managing HOA operations. It generates violation notices based on information you enter, but it does not provide legal advice, legal document drafting, or legal review.

**Are violation notices generated by Livenhood legally valid?**
Notices generated by Livenhood are formatted letters based on the information you provide (rule cited, description, photos, cure deadline). Whether a notice meets your state's or HOA's specific legal requirements depends on your governing documents and applicable law. Verify notice requirements with your HOA attorney before sending.

**Does Livenhood enforce fines?**
Fine assessment is not available in the current version of Livenhood. Fine processes involve legal and regulatory considerations that vary by state. Consult your HOA attorney before implementing a fine schedule.

**Can the audit trail be used as evidence in a dispute?**
The audit trail records all actions with timestamps and user attribution. Whether this record is admissible or useful in a specific dispute depends on the nature of the dispute and the applicable rules of evidence. Consult your HOA attorney.

**Does Livenhood constitute legal service?**
No. Livenhood is a software tool, not legal counsel. All enforcement settings are configured by your board based on your governing documents. Verify enforcement requirements with your HOA attorney.

**Who is responsible for HOA enforcement decisions?**
Your board. Livenhood provides tools to help your board track and communicate about violations, but all enforcement decisions (whether to file a violation, send a notice, waive, or close) are made by your board in accordance with your governing documents. Livenhood does not make enforcement decisions.

_Last updated: 2026-04-05_
