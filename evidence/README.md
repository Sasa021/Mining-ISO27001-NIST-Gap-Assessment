# Evidence

Store the notes and fictional documents you create while you assess Amberkloof. The sheets should point here by evidence id. A rating of `Met` needs a file in this folder, or a clear statement that the evidence was not provided and the rating is not `Met`.

**Fictional exercise.** Do not put real employer data, real identity numbers, real health information, real credentials, scans of a real network, or malware in this folder.

## What to keep

- Interview notes, one file per role
- Assumption log, if a fact is not in the company profile
- Short fictional policies or registers you write so a control has something to point at
- Exports you invent, clearly marked as fictional, such as a user list with made up names
- A copy of the corrected network sketch, if you change the one in the profile

## What to leave out

- Passwords, keys, tokens, and connection strings
- Identity numbers, bank account numbers, and health records, even invented ones that look real. Use obvious fakes such as `ID-EXAMPLE-01` if a field is required
- Output from a scanner, exploit, or test against any real address
- Copyrighted text from ISO/IEC 27001 or IEC 62443

## File names

Use an evidence id, then a short name:

```text
EV-001-interview-it-administrator.md
EV-002-assumption-log.md
EV-003-fictional-asset-list.csv
```

Start at `EV-001`. Do not reuse an id.

First line of every file:

```text
Fictional evidence created for this exercise. Amberkloof Mining Systems is not a real company.
```

## Index

Fill this table as you go. The ids in the assessment sheets must match this index.

| Evidence id | File | What it supports | Provided, not provided, or assumption |
| --- | --- | --- | --- |
| | | | |

## Interview note shape

```text
Fictional evidence created for this exercise. Amberkloof Mining Systems is not a real company.

Role:
Site:
Date of the fictional interview:

Facts
- 

Assumptions
- 

Conflicts with another role
- 

Evidence still missing
- 
```

Write facts as things the role does or does not do. Do not put `Partial` or a risk score in the note. Score later, in the CSV, from these notes.
