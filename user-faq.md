# Veranda — FAQ

> Common questions from board members and homeowners.

**Status:** Current | **Last verified:** 2026-04-02

---

## Quick Links

- [For Board Members](#for-board-members)
- [For Homeowners](#for-homeowners)
- [Technical Questions](#technical-questions)
- [Legal Questions](#legal-questions)

---

## For Board Members

**How do I add units to my community?**
Go to **Units** → click **Add Unit** to add one at a time. For 5 or more units, use **Import CSV** for bulk import. See [docs/clients/importing-properties.md](../../docs/clients/importing-properties.md) for the CSV format.

**How do I invite homeowners?**
Go to **Units** → find the unit → click **Invite Resident**. Enter their email and name, select their role (Homeowner or Tenant), and click **Send Invite**. For bulk invites, include owner email columns in your CSV import.

**A homeowner says they didn't receive their invite. What do I do?**
Go to **Units** → scroll to **Pending Invitations** → find their name → click **Resend**. A new invitation is sent and the old link is invalidated. Check that the email address on file is correct.

**How do I create a violation?**
Go to **Violations** → **New Violation**. Select the unit, category, write a description, attach photos, and optionally cite the rule. The homeowner is not notified until you send a formal notice.

**Can I edit a violation after it's created?**
You can add internal notes and photos at any time. The description and category can be edited while the violation is in `open` status. Once a notice is sent, the filed record is locked to preserve the legal record.

**What's the difference between Close and Waive?**
Any board member can close a violation (resolved informally, withdrawn, or no longer applicable). Only board admins can waive a violation (the board chooses not to enforce it). Both are recorded in the audit trail.

**Can I have multiple board admins?**
Yes. Invite board members and set their role to Board Admin. There is no limit to the number of board admins.

**How do I remove a board member or homeowner?**
Go to **Members** → find the person → click **Deactivate**. Only board admins can deactivate accounts. Their history is preserved; they lose access immediately. You cannot deactivate yourself.

**Can announcements be scheduled for later?**
Not currently. Announcements are published immediately when you click Publish.

**Who can see Board Only documents?**
Documents marked as Board Only are visible only to board members (board_admin and board_member roles). Homeowners and tenants cannot see them.

---

## For Homeowners

**How do I accept my invitation?**
Click the link in your invitation email, set a password, verify your email with the 6-digit code, and you're in. If the link has expired (links are valid for 7 days), ask your board admin to resend it.

**Where do I see my violations?**
Log in to Veranda → go to **Violations**. You'll see all violations filed for your unit, their status, and the cure deadline for each.

**I received a violation notice. What do I do?**
Read the notice carefully. It includes the rule cited, what was observed, and the cure deadline. Correct the issue before the deadline. Once fixed, you can submit resolution photos directly in Veranda through the violation detail page.

**How do I submit proof that I fixed a violation?**
Open the violation → click **Mark as Resolved** → write a description and attach photos → click **Submit**. Your board will review your submission and confirm the resolution.

**Can I download my violation notice?**
Yes. Open the violation → go to the **Notices** tab → click the PDF download link.

**How do I change my email address?**
Go to **Settings** → click **Change Email** → enter your new email and current password → click **Submit Request**. A board admin must approve the change. You'll be notified when it's approved.

**How do I change my password?**
Go to **Settings** → click **Change Password** → enter your current password and your new password → click **Update Password**.

**Why am I not receiving push notifications?**
Check that you have allowed notifications in your browser. On iOS, push notifications work in Safari with iOS 16.4 or later after adding Veranda to your Home Screen. Email is always the primary notification channel — check your email if you're not receiving push notifications.

**Can I see documents like CC&Rs and bylaws?**
Yes. Go to **Documents** to access all community documents marked as Public by your board.

---

## Technical Questions

**Do I need to download an app?**
No. Veranda is a Progressive Web App (PWA). Access it from any browser on your phone or computer. On Android (Chrome) and iOS (Safari), you can install it to your home screen for an app-like experience — no app store required.

**What browsers does Veranda support?**
Chrome, Safari, Firefox, and Edge — current and one version back. Chrome on Android is recommended for the best push notification experience on mobile.

**The app isn't loading. What should I try?**
Try a hard refresh (Ctrl+Shift+R on Windows, Cmd+Shift+R on Mac). Check your internet connection. If the problem persists, try logging out and logging back in.

**I'm logged out unexpectedly. Is this normal?**
Veranda sessions expire for security. Log back in with your email and password. If you're being logged out frequently, check that your browser is not clearing cookies or local storage on close.

**The notification bell shows a count but clicking it shows nothing. What's happening?**
Click **Mark all as read** to clear the badge. If notifications are missing, try refreshing the page.

**Can I use Veranda on a tablet?**
Yes. Veranda is responsive and works on tablets in both portrait and landscape orientation.

---

## Legal Questions

**Is Veranda a legal document service?**
No. Veranda is a software tool for managing HOA operations. It generates violation notices based on information you enter, but it does not provide legal advice, legal document drafting, or legal review.

**Are violation notices generated by Veranda legally valid?**
Notices generated by Veranda are formatted letters based on the information you provide (rule cited, description, photos, cure deadline). Whether a notice meets your state's or HOA's specific legal requirements depends on your governing documents and applicable law. Verify notice requirements with your HOA attorney before sending.

**Does Veranda enforce fines?**
Fine assessment is not available in the current version of Veranda. Fine processes involve legal and regulatory considerations that vary by state. Consult your HOA attorney before implementing a fine schedule.

**Can the audit trail be used as evidence in a dispute?**
The audit trail records all actions with timestamps and user attribution. Whether this record is admissible or useful in a specific dispute depends on the nature of the dispute and the applicable rules of evidence. Consult your HOA attorney.

**Does Veranda constitute legal service?**
No. Veranda is a software tool, not legal counsel. All enforcement settings are configured by your board based on your governing documents. Verify enforcement requirements with your HOA attorney.

**Who is responsible for HOA enforcement decisions?**
Your board. Veranda provides tools to help your board track and communicate about violations, but all enforcement decisions (whether to file a violation, send a notice, waive, or close) are made by your board in accordance with your governing documents. Veranda does not make enforcement decisions.

_Last updated: 2026-04-02_
