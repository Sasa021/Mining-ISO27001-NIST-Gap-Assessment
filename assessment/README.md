# Assessment workbooks

Fill these files yourself. The company and the questions are already in the repository. The judgements are not.

**Fictional.** Ratings you add are about Amberkloof Mining Systems only. Do not copy in a real assessment.

| File | What you fill |
| --- | --- |
| [iso27001-annexA-gap.csv](iso27001-annexA-gap.csv) | Current state, target state, gap rating, evidence, owner, priority for each Annex A control |
| [nist-csf-2-gap.csv](nist-csf-2-gap.csv) | Current tier, target tier, gap, and notes for each CSF 2.0 subcategory |
| [risk-register.csv](risk-register.csv) | The risks you choose, then likelihood, impact, score, treatment, and owner |
| [ot-iec62443.md](ot-iec62443.md) | Zone review and the seven IEC 62443 themes, at a high level |

## Example rows

Each CSV has one row whose id is `EXAMPLE`. That row shows how a finished line looks. It is not a finding about Amberkloof. Delete it before you share the work. The real rows underneath stay blank until you complete them.

`ot-iec62443.md` has one example row in each table for the same reason. Delete those rows too.

## Rules that keep the sheets usable

- Use the scales in [docs/method.md](../docs/method.md). Do not add a private numbering scheme.
- ISO titles are short paraphrases, not the text of the standard.
- NIST subcategory sentences follow NIST CSF 2.0 (CSWP 29). They are public. A comma is used where the NIST PDF uses a dash.
- Risk score must equal likelihood times impact.
- Point the evidence cell at an id in [evidence/README.md](../evidence/README.md).
- One owner per row. Use a role.
- If the workshop and Red Dune differ, say so in the cell. Do not average them into a single vague sentence.

Open the CSV files in a spreadsheet if that is easier. Keep the header row. Save as CSV again so the repository stays in plain text.
