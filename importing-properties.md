# Livenhood — Importing Properties

> Bulk-import all of your community's properties at once using a CSV spreadsheet file. You can include owner contact information so Livenhood automatically sends invitation emails during the import.

**Status:** Current | **Last verified:** 2026-04-02

---

## Quick Links

- [Who Can Use This Feature](#who-can-use-this-feature)
- [Preparing Your CSV File](#preparing-your-csv-file)
- [Examples by Property Type](#examples-by-property-type)
- [Step-by-Step Import](#step-by-step-import)
- [Tips and Limits](#tips-and-limits)
- [Downloading a Template](#downloading-a-template)

---

## Who Can Use This Feature

Any **board admin** or **board member** can import properties. You will find the **Import CSV** button at the top of the **Properties** (or Units / Lots / Homes) page.

---

## Preparing Your CSV File

A CSV file is a plain text spreadsheet that any spreadsheet app can export. Open your spreadsheet software (Excel, Google Sheets, Numbers) and set up the following columns:

| Column           | Required? | Description                                                                             |
| ---------------- | --------- | --------------------------------------------------------------------------------------- |
| `address`        | ✅ Yes    | Street address only, e.g. `123 Oak Lane` or `100 Main Street Unit 1A`                   |
| `lotNumber`      | No        | Your own identifier, e.g. `Lot 14` or `4B`. If blank, Livenhood uses the street number. |
| `city`           | No        | City, e.g. `Austin`                                                                     |
| `state`          | No        | Two-letter state code, e.g. `TX`                                                        |
| `zip`            | No        | ZIP code, e.g. `78701`                                                                  |
| `ownerEmail`     | No        | Homeowner or tenant email. When provided, an invitation is sent automatically.          |
| `ownerFirstName` | No        | Owner's first name                                                                      |
| `ownerLastName`  | No        | Owner's last name                                                                       |
| `role`           | No        | `homeowner` or `tenant`. Defaults to `homeowner`.                                       |
| `lotSizeSqft`    | No        | Lot size as a whole number, e.g. `7200`                                                 |

> **Column names are case-insensitive** — `Address`, `ADDRESS`, and `address` all work. You can also omit the header row and Livenhood will assume the columns are in this order: `address`, `lotNumber`, `city`, `state`, `zip`, `ownerEmail`, `ownerFirstName`, `ownerLastName`, `role`, `lotSizeSqft`.

---

## Examples by Property Type

### Single-family homes (subdivision)

Most common setup. The address is the full identifier; lot number is optional.

```csv
address,ownerEmail,ownerFirstName,ownerLastName,lotSizeSqft
123 Oak Lane,jsmith@email.com,Jane,Smith,8500
456 Maple Drive,bjones@email.com,Bob,Jones,7200
789 Birch Road,,,,
```

> The third row has no owner yet — the property is created and an invite can be sent later.

### Lots (land subdivision / HOA with vacant lots)

```csv
address,lotNumber,ownerEmail,role
14 Lakeview Terrace,Lot 14,owner@email.com,homeowner
22 Lakeview Terrace,Lot 22,,
31 Lakeview Terrace,Lot 31,tenant@email.com,tenant
```

### Apartments / condos / townhomes

Unit numbers work as lot numbers.

```csv
address,lotNumber,ownerEmail,ownerFirstName,ownerLastName
100 Main Street,1A,alice@email.com,Alice,Nguyen
100 Main Street,1B,bob@email.com,Bob,Kim
100 Main Street,2A,,,
```

---

## Step-by-Step Import

1. Go to **Properties** in the board portal
2. Click **Import CSV** in the top-right corner
3. Click the file drop zone and choose your `.csv` file
4. Livenhood shows a **preview of the first 10 rows** and the total count — review it
5. If there are any errors (shown in red), fix them in your spreadsheet and re-upload
6. Click **Import N properties** to start the import
7. Once complete, you'll see a summary:
   - How many properties were **created**
   - How many **invitation emails** were sent
   - Any rows that were **skipped** (duplicates) or **failed** with the reason

---

## Tips and Limits

- **Maximum 500 rows** per import. Split larger lists into multiple files.
- **Duplicate addresses** are skipped automatically — re-running the same file is safe.
- **Invitation emails** are sent immediately for rows with an `ownerEmail`. If an email fails to send, the property is still created — you can resend the invite from the **Pending Invitations** section.
- **Addresses with commas** (e.g. `123 Main St, Apt 4`) must be wrapped in double quotes: `"123 Main St, Apt 4"`. Most spreadsheet apps do this automatically when you export as CSV.
- The import does **not** overwrite existing properties. It only creates new ones.

---

## Downloading a Template

Copy the appropriate template below into a new spreadsheet, fill in your data, then export as CSV.

**Single-family homes:**

```
address,lotNumber,city,state,zip,ownerEmail,ownerFirstName,ownerLastName,role,lotSizeSqft
123 Oak Lane,,Austin,TX,78701,jsmith@email.com,Jane,Smith,homeowner,8500
456 Maple Drive,,Austin,TX,78701,bjones@email.com,Bob,Jones,homeowner,7200
```

**Apartments / condos:**

```
address,lotNumber,city,state,zip,ownerEmail,ownerFirstName,ownerLastName,role
100 Main Street,1A,Austin,TX,78701,alice@email.com,Alice,Nguyen,homeowner
100 Main Street,1B,Austin,TX,78701,bob@email.com,Bob,Kim,homeowner
```

**Lots:**

```
address,lotNumber,city,state,zip,ownerEmail,ownerFirstName,ownerLastName,role,lotSizeSqft
14 Lakeview Terrace,Lot 14,Austin,TX,78701,owner@email.com,John,Doe,homeowner,12000
```

---

> **Need help?** Contact your Livenhood administrator or reach out to support. Do not include sensitive financial or legal information in the CSV — this file is only for property and contact data.

---

_Last updated: 2026-04-02_
