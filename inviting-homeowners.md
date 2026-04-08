# Livenhood — Inviting Homeowners

> How to get residents and board members onto Livenhood — individually, in bulk, and what they see when they accept.

**Status:** Current | **Last verified:** 2026-04-02

---

## Quick Links

- [Invite a Single Homeowner](#invite-a-single-homeowner)
- [Bulk Invite with CSV Import](#bulk-invite-with-csv-import)
- [Resend an Invitation](#resend-an-invitation)
- [Revoke an Invitation](#revoke-an-invitation)
- [Invite a Board Member](#invite-a-board-member)
- [What the Homeowner Sees](#what-the-homeowner-sees)
- [Removing a Homeowner](#removing-a-homeowner)
- [Tips](#tips)

---

## Invite a Single Homeowner

1. Go to **Properties** in your board dashboard
2. Find the unit you want to invite the homeowner to
3. Click the unit to open its detail page
4. Click **Invite Homeowner**
5. Enter their email address, first name, and last name
6. Select their role: **Homeowner** or **Resident**
7. Click **Send Invite**

> The homeowner receives an email with a personalized invitation link. The link is **valid for 7 days** and can only be used **once**.

---

## Bulk Invite with CSV Import

If you're setting up a new community or inviting many homeowners at once, use the CSV import:

1. Go to **Properties** → click **Import CSV**
2. Upload your CSV file with `ownerEmail`, `ownerFirstName`, and `ownerLastName` columns filled in
3. After import completes, click **Send Bulk Invites**
4. Livenhood sends invitation emails to every homeowner included in the import

See [importing-properties.md](./importing-properties.md) for the CSV format.

---

## Resend an Invitation

If a homeowner hasn't accepted their invite (link expired or email missed):

1. Go to **Properties** → scroll to **Pending Invitations**
2. Find the homeowner and click **Resend**

> A new invitation link is sent to their email. The old link is **invalidated**.

---

## Revoke an Invitation

To cancel an invitation before it's accepted:

1. Go to **Properties** → scroll to **Pending Invitations**
2. Find the homeowner and click **Revoke**

---

## Invite a Board Member

1. Go to **Members** in your board dashboard
2. Click **Invite Board Member**
3. Enter their email address, first name, and last name
4. Select their role:

| Role              | Access Level                                                                                                              |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------- |
| **Board Officer** | Full control — can change other members' roles and deactivate users                                                       |
| **Board Member**  | Can create violations, manage documents and announcements, invite homeowners. Cannot change roles or deactivate accounts. |

5. Click **Send Invite**

---

## What the Homeowner Sees

When a homeowner clicks the invitation link:

1. They see a **welcome screen** confirming which community they're joining
2. They **set a password** for their account
3. They **verify their email** address (Cognito sends a 6-digit code)
4. They're taken to their **homeowner portal**

From the portal they can:

- See **violations** for their unit
- **View and download** community documents
- Receive **push notifications** (if they allow it on their device)
- Update their **profile** and notification preferences

---

## Removing a Homeowner

When a homeowner moves out or should no longer have access:

1. Go to **Members**
2. Find the homeowner
3. Click **Deactivate**

> Their account is deactivated immediately. They cannot log in, but their history (violations, etc.) is **preserved** for your records. You can then invite the new owner to the same unit.

---

## Tips

- **Invite early.** The sooner homeowners are on Livenhood, the sooner they receive violation notices electronically — which simplifies enforcement.
- **Use bulk invite after a successful CSV import.** It takes 30 seconds to invite 100 homeowners.
- **Check pending invitations regularly.** Some homeowners miss their invite email. A resend usually fixes it.
- **Set the right role.** A resident should get the Resident role, not Homeowner. This keeps ownership records accurate.

---

_Last updated: 2026-04-02_
