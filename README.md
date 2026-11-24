# ISO 27001 and NIST CSF gap assessment

**All company data in this repository is fictional.** Amberkloof Mining Systems (Pty) Ltd is an invented mid sized South African mining equipment and operations company. It is not a real business. It is not based on any employer, client, or mine. Do not add real company names, real employee data, or real network details.

This repository is a scaffold. Gap ratings, findings, and risk scores are blank on purpose. Mosa Mofokeng completes the assessment herself. Each workbook has one row marked `EXAMPLE ONLY` to show the format. Delete that row before you treat the sheet as your work.

## Overview

Amberkloof designs and builds surface materials handling equipment, and it runs a contract for pit water and dust suppression at one remote site. The company has a small IT team, a workshop, a spares depot, and an operational technology (OT) environment with SCADA, PLCs, and fleet telematics.

The exercise is a gap assessment against:

- ISO/IEC 27001:2022 Annex A, using control numbers and short paraphrased titles only
- NIST Cybersecurity Framework (CSF) 2.0, which is a public NIST publication
- IEC 62443 at a high level, for the OT zones
- South African context from the Protection of Personal Information Act 4 of 2013 (POPIA) and the Cybercrimes Act 19 of 2020

You interview the fictional roles, record evidence, then fill the sheets and the executive report. The method is in [docs/method.md](docs/method.md).

## What this proves

Completed work in this repository shows that you can:

- Scope governance, risk, and compliance for a company that has both IT and OT
- Compare current practice with ISO/IEC 27001 Annex A and NIST CSF 2.0, and explain the gap in plain language
- Keep a risk register with a stated scoring method, an owner, and a treatment
- Describe OT zones using the Purdue model, and point to IEC 62443 without pretending to certify a zone
- Write an executive gap report and a 30/60/90 day roadmap
- Place the result in South African law, including POPIA and the Cybercrimes Act
- Separate evidence from opinion, and leave a clear owner on each action

Employers should see your judgement in the sheets and the report. The scaffold only supplies the company, the questions, and the empty tables.

## Frameworks used

| Framework | How it is used here |
| --- | --- |
| ISO/IEC 27001:2022 Annex A | Control numbers and short paraphrased titles. This repo does not copy the standard. |
| NIST CSF 2.0 | Functions, categories, subcategories, and tiers. Wording follows NIST CSWP 29. |
| IEC 62443 | High level only: zones, conduits, security levels, and the seven requirement themes. |
| POPIA and the Cybercrimes Act | Legal context for privacy, security safeguards, breach notice, and cyber offences. Not a legal opinion. |

ISO/IEC 27001 and IEC 62443 are paid standards. Buy or borrow them if you need the official sentences. NIST CSF 2.0 is free from NIST.

## Method

Do the work in this order.

1. Read [company-profile/README.md](company-profile/README.md) and the network sketch.
2. Read [docs/method.md](docs/method.md). Use the rating scales there. Do not invent a second scale in the sheets.
3. Run the interviews with [docs/interview-questionnaire.md](docs/interview-questionnaire.md). The company is fictional, so you play both sides. Write the answers yourself and label anything you assume.
4. File notes and invented documents in [evidence/](evidence/README.md).
5. Fill [assessment/iso27001-annexA-gap.csv](assessment/iso27001-annexA-gap.csv), [assessment/nist-csf-2-gap.csv](assessment/nist-csf-2-gap.csv), and [assessment/risk-register.csv](assessment/risk-register.csv).
6. Complete the OT tables in [assessment/ot-iec62443.md](assessment/ot-iec62443.md).
7. Draft the report from [docs/report-template.md](docs/report-template.md).
8. Replace the Results and Lessons Learned sections below with your own words.
9. Capture the screenshots in [docs/screenshot-checklist.md](docs/screenshot-checklist.md).

Rating rules, in short:

- ISO gap rating: `Met`, `Partial`, `Not met`, or `Not applicable`
- NIST tiers: Tier 1 Partial, Tier 2 Risk Informed, Tier 3 Repeatable, Tier 4 Adaptive
- Risk score: likelihood (1 to 5) times impact (1 to 5)

Full definitions are in the method. Leave a cell blank until you have a reason you can point to.

## Repo structure

```text
.
├── README.md
├── LICENSE
├── .gitignore
├── company-profile/
│   └── README.md
├── assessment/
│   ├── README.md
│   ├── iso27001-annexA-gap.csv
│   ├── nist-csf-2-gap.csv
│   ├── risk-register.csv
│   └── ot-iec62443.md
├── docs/
│   ├── method.md
│   ├── interview-questionnaire.md
│   ├── report-template.md
│   └── screenshot-checklist.md
└── evidence/
    └── README.md
```

## Results

To be completed by Mosa after the assessment.

Replace this paragraph with the outcome in your own words. State the largest gaps, the highest risks, and whether you would treat OT or corporate IT first. Point to the sheets. Do not leave any `EXAMPLE ONLY` row in the result you show an employer.

## Lessons learned

To be completed by Mosa after the assessment.

Replace this paragraph with what you learned. Say which answers were hard to evidence, what you would ask differently next time, and what you would refuse to claim without a document.

## About me

Rewrite this section in your own words before you share the repository.

- Name: Mosa Mofokeng
- Location: Cape Town, South Africa
- Credentials to mention once you are ready: ISC2 CC, Microsoft SC-200
- LinkedIn: paste your profile URL here (start from [linkedin.com](https://www.linkedin.com/))
- GitHub: [github.com/Sasa021](https://github.com/Sasa021)

Suggested shape, once you rewrite it: four to six lines on the kind of security work you want, then the two links. Keep the fictional company notice at the top of this README.
