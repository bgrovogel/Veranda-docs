# Veranda — Client FAQ

> Common questions from board administrators and homeowners.

**Status:** Current | **Last verified:** 2026-04-02

---

## Quick Links

- [Getting Started](#getting-started)
- [Properties and Units](#properties-and-units)
- [Violations](#violations)
- [Announcements](#announcements)
- [Documents](#documents)
- [Notifications](#notifications)
- [Account and Security](#account-and-security)
- [Technical](#technical)

---

## Getting Started

**How do I set up my community on Veranda?**
Go to the Veranda sign-up page and click **"Set up a new HOA."** You'll create your account, verify your email, and enter your community details (name, address, state). Once your account is created, you'll land on your board dashboard and can start adding units and inviting homeowners.

**How do I add board members?**
Go to **Members** in your board dashboard and click **Invite Board Member**. Enter their email address and select their role (Board Admin or Board Member). They'll receive an invitation email with a link to create their account.

**What roles are available?**

| Role             | Permissions                                                                                                        |
| ---------------- | ------------------------------------------------------------------------------------------------------------------ |
| **Board Admin**  | Everything — create violations, change member roles, deactivate users, manage settings                             |
| **Board Member** | Create violations, invite homeowners, manage documents and announcements. Cannot change roles or deactivate users. |
| **Homeowner**    | View their own violations, submit resolutions, view community documents and announcements                          |
| **Tenant**       | Same as Homeowner                                                                                                  |

---

## Properties and Units

**Can I import all my properties at once?**
Yes — use the **Import CSV** button on the Properties page. See [importing-properties.md](./importing-properties.md) for the required format and examples. Up to 500 properties per import.

**What if I have a unit that is rented (not owner-occupied)?**
Set the `role` column to `tenant` in your CSV, or select **"Tenant"** when inviting someone to a unit. Tenants see the same homeowner portal as owners.

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
2. Board **sends First Notice** — Veranda generates a PDF letter and emails the homeowner
3. A **cure period timer** starts automatically (typically 14–30 days)
4. If **resolved**: homeowner submits photos; board confirms resolution
5. If **not resolved**: board sends Second Notice
6. Board can **waive or close** the violation at any time

> Veranda is a software tool, not legal counsel. Verify enforcement requirements with your HOA attorney.

**Do homeowners get notified automatically?**
Yes — when a notice is sent, the homeowner receives an **email** and a **push notification** (if they've installed the PWA on their phone).

**Can homeowners see their violations?**
Yes — homeowners see all violations for their unit when they log into their portal. They can submit resolution photos directly.

**How do I waive a violation?**
Open the violation and click **Waive**. Only board admins can waive violations. The audit trail records who waived it and when.

**Can I print a violation notice?**
Yes — violation notices are generated as PDF documents. Download them from the violation detail page under the **Notices** tab.

**Is fine assessment available?**
Fine assessment is coming in Phase 2 and is not available in the current version of Veranda. Contact your HOA attorney regarding your community's fine policy and enforcement procedures.

---

## Announcements

**How do I send a community-wide announcement?**
Go to **Announcements**, click **New Announcement**, write your message, and click **Publish**. All registered homeowners receive an email and push notification.

**Do all homeowners see announcements even if they haven't signed up for Veranda?**
No — announcements are delivered to users with active Veranda accounts. This is another reason to get all homeowners set up in the system.

**Can I schedule an announcement for later?**
Not in the current version. Announcements are published immediately when you click Publish.

**Can I pin an announcement?**
Yes. Pinned announcements appear at the top of the list for all homeowners. Click the pin icon on any announcement to toggle it.

---

## Documents

**What documents should I upload?**
At minimum: **CC&Rs**, **bylaws**, and **meeting minutes**. You can also upload budget documents, reserve studies, architectural guidelines, and any community rules.

**Who can see documents?**
All registered homeowners can view documents marked as **"Public."** Board-only documents are visible only to board members.

**What file formats are supported?**
PDF, JPEG, PNG, and Word documents (`.docx`). Maximum file size is **50MB per file**.

**How long are documents stored?**
Indefinitely while your subscription is active.

---

## Notifications

**What notifications does Veranda send?**

| Event                      | Email          | Push Notification |
| -------------------------- | -------------- | ----------------- |
| Violation notice sent      | Homeowner      | Homeowner         |
| Cure deadline approaching  | Homeowner      | Homeowner         |
| Violation resolved/closed  | Homeowner      | Homeowner         |
| New announcement published | All homeowners | All homeowners    |
| Invitation to join Veranda | Invitee        | —                 |

**How do homeowners get push notifications on their phone?**
When a homeowner visits the Veranda portal for the first time, their browser will ask for notification permission. On Android (Chrome), they can also install Veranda to their home screen as a PWA. On iOS Safari, they can use "Add to Home Screen."

> iPhone users: Push notification reliability on iOS varies by browser and iOS version. Email is always the **primary delivery channel** for legally significant notices (violations, cure deadlines). Encourage homeowners to check their email as the backup.

---

## Account and Security

**How do I reset my password?**
On the login page, click **Forgot password?**, enter your email, and follow the link in the reset email.

**How do I change my email address?**
Submit an email change request from your **Settings** page. A board admin must approve the change before it takes effect. This protects against unauthorized account changes.

**Can I remove a board member?**
Yes — go to **Members**, find the person, and click **Deactivate**. Only board admins can deactivate accounts. You cannot deactivate yourself.

**Is my community's data visible to other communities?**
No. Every community's data is completely isolated. Veranda enforces row-level security at the database layer — it is architecturally impossible for one community to see another's violations, units, members, or documents.

---

## Technical

**Do homeowners need to download an app?**
No. Veranda is a **Progressive Web App (PWA)**. Homeowners access it from any browser on their phone or computer. On Android and iOS, they can optionally install it to their home screen for an app-like experience — no app store required.

**What browsers are supported?**
Chrome, Safari, Firefox, and Edge — current and one version back. **Chrome on Android** is recommended for the best push notification experience.

**Is there a native mobile app?**
Not currently. Veranda is a PWA that works in mobile browsers and can be installed to the home screen. A native app may be considered in a future phase if PWA push notification delivery does not meet requirements.

**Is there an API?**
Yes — Veranda has a REST API. Contact Veranda support if you need to integrate with other systems.

---

_Last updated: 2026-04-02_
