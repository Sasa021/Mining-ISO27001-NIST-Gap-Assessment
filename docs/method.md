# Method

How to run this gap assessment on Amberkloof Mining Systems. The company is fictional. Read [company-profile/README.md](../company-profile/README.md) first.

This note tells you how to work. It does not contain ratings, findings, or scores. You produce those after you have notes.

The legal context for South Africa is written up in the report template. Use it when you judge privacy, breach notice, and what to do if someone commits an offence against the company. It is not legal advice.

## What you are assessing

You are comparing how Amberkloof manages cybersecurity risk with:

- ISO/IEC 27001:2022 Annex A, by control number
- NIST CSF 2.0, by subcategory and tier
- IEC 62443 ideas, at zone level, for the Red Dune plant

You are not issuing a certificate. You are not allowed to quote Annex A or IEC 62443 control sentences in place of your own judgement. Short titles are already in the sheet. Your words go in the evidence and gap cells.

## Solo interviews

There is no real staff to call. You play the interviewer and the interviewee.

Rules that keep the work honest:

1. Use the roles in the company profile. Do not add a security team that the profile does not have unless you write the addition into the profile and mark it as yours.
2. Ask one role at a time. Write the answer in that person's voice, in [evidence/](../evidence/README.md), and put the role name on the note.
3. If you invent a fact that the profile does not state, start the sentence with `Assumption:`.
4. Keep the story consistent. If the artisan says PLC changes are logged, the superintendent's note cannot quietly say the opposite unless you record the conflict and resolve it.
5. Do not copy the `EXAMPLE ONLY` rows. Those rows show column format. They are not facts about Amberkloof.
6. During the interview, write what people do. Do not write the gap rating in the same sentence. Score the next pass, from the notes.
7. If two roles disagree, keep both statements and look for a document that would settle it. If you never create that document, the rating stays weaker than `Met`.

Suggested length is 45 to 60 minutes per role. You do not need a transcript. You need facts you can point to later: who, what system, how often, where the record is, what happens when it fails.

## Who to speak to

| Order | Role | Why this conversation matters |
| --- | --- | --- |
| 1 | Managing Director | What the business will not risk, and who is allowed to accept a risk |
| 2 | IT Administrator | Identity, endpoints, backups, the network sketch, vendors |
| 3 | HR Manager | Joiners, leavers, training, employee and health information |
| 4 | Finance Manager | Ledgerpit, payments, PayMica |
| 5 | Workshop Manager | Workshop LAN, CCTV, test bench, contractors on the floor |
| 6 | Operations Superintendent | Red Dune contract, safety, OT ownership, client boundary |
| 7 | Control room artisan | How PitView and the PLCs are actually changed |
| 8 | Depot Supervisor | The small site that is easy to forget |
| 9 | DeskOrchard service lead | What the MSP can see and change |

Use the questions in [interview-questionnaire.md](interview-questionnaire.md). Add questions when an answer is vague. Stop when you can name the evidence, or when you can say the evidence does not exist.

Opening line you can reuse:

> This is a fictional assessment for a portfolio project. I am going to ask what you do today, who else is involved, and what record I could look at. I will write the rating after the interview, not during it.

Closing line:

> What should I have asked about your site that I did not ask? What broke the last time something failed?

## How to take notes

For each fact, try to capture five points:

1. The claim, in one sentence
2. The role who said it
3. The system or site
4. The evidence that would prove it, and whether you have it
5. The assumption, if you filled a hole yourself

File names and the evidence index are described in [evidence/README.md](../evidence/README.md).

Ask for these kinds of evidence when the answer is "yes, we do that":

- A policy or procedure, and the date someone approved it
- A list of users, assets, or vendors
- A ticket, a backup log, a training register, or a change note
- A contract clause, not only a verbal promise from a vendor
- A diagram that matches the cables and accounts, not only the sketch in the profile

If the evidence is "we would do that if asked", the practice is not in place.

## How to rate ISO/IEC 27001 Annex A

Sheet: [assessment/iso27001-annexA-gap.csv](../assessment/iso27001-annexA-gap.csv).

The control id and the short title are filled. Everything else is yours. Titles are paraphrases so the sheet can be shared without copying the standard. If your wording needs the official sentence, read your own licensed copy and keep that sentence out of the repository.

Use only these gap ratings:

| Gap rating | Use it when |
| --- | --- |
| Met | The practice exists, people use it, and you can point to evidence. It covers the sites where the control matters. |
| Partial | Something exists, but it is informal, out of date, unused at one of the sites, or missing evidence. |
| Not met | You found no practice that meets the control. |
| Not applicable | The control does not apply. Write the reason in the evidence cell. |

Current state is what happens now, in your words, one or two sentences. Target state is what you think Amberkloof should be able to show in the next year. Do not set every target to a perfect enterprise programme. A mid sized contractor needs controls it can actually run.

Priority is `High`, `Medium`, or `Low`. Set it only after the risk register has a first pass. A large paper gap on a low impact asset is not automatically high priority. A small gap on PitView or on health information might be.

Owner is a role from the profile, not a person's private name if you can avoid it. One owner per row. "IT and OT" is not an owner.

Leave `Not applicable` rare. Say why.

## How to rate NIST CSF 2.0

Sheet: [assessment/nist-csf-2-gap.csv](../assessment/nist-csf-2-gap.csv).

NIST CSF 2.0 is public. The subcategory sentences in the sheet follow NIST CSWP 29. A few commas were used where the NIST PDF uses a dash, so this repository stays in plain punctuation. The meaning is the NIST outcome.

Tiers describe how rigorous the practice is. Use the tier number and the name.

| Tier | Name | Plain meaning |
| --- | --- | --- |
| Tier 1 | Partial | Ad hoc. The practice depends on one person and is not repeatable. |
| Tier 2 | Risk Informed | People know the main risks. Practices exist but are not yet consistent everywhere. |
| Tier 3 | Repeatable | The practice is a defined process, used across the sites in scope, and checked. |
| Tier 4 | Adaptive | The practice changes from lessons and current risk, and it is reviewed on purpose. |

Current tier is today. Target tier is the tier that fits Amberkloof's risk, not automatically Tier 4. Many outcomes at a company this size are well aimed at Tier 2 or Tier 3.

Gap is the target tier number minus the current tier number. Example of the arithmetic only: a current Tier 1 and a target Tier 3 produce a gap of 2. That arithmetic is not a score for any Amberkloof row until you choose the tiers.

The notes cell is for scope limits, conflicts between interviews, and links to evidence ids. It is not a second rating scale.

Govern comes first in the sheet because CSF 2.0 uses Govern to set how the other functions are prioritised. You may still fill Identify and Protect before you finish Govern if that is the evidence you have. Come back and check that the target tiers match what the Managing Director would actually fund.

## How to score the risk register

Sheet: [assessment/risk-register.csv](../assessment/risk-register.csv).

One row is one risk, not one control. Write it as: a threat exploits a vulnerability on an asset, with a consequence you can explain.

Likelihood:

| Score | Word | When to use it |
| --- | --- | --- |
| 1 | Rare | You would not expect this in the next few years without a big change |
| 2 | Unlikely | Possible, but not a normal year |
| 3 | Possible | Could happen this year if nothing changes |
| 4 | Likely | You would be surprised if it did not happen |
| 5 | Almost certain | It is already happening, or it will happen without a change |

Impact:

| Score | Word | When to use it |
| --- | --- | --- |
| 1 | Insignificant | Short inconvenience, no safety, legal, or client consequence |
| 2 | Minor | Local disruption, a day of rework, small cost |
| 3 | Moderate | One site down for days, or a reportable privacy issue you can contain |
| 4 | Major | Contract, safety, or regulatory trouble that reaches the Managing Director |
| 5 | Severe | People harmed, a long plant stoppage, or personal information exposed at scale |

Score equals likelihood times impact. Do the multiplication yourself. Do not type a score that does not match the two inputs.

Use the bands only to sort the register, after the scores exist:

| Score | Band |
| --- | --- |
| 1 to 6 | Low |
| 8 to 12 | Medium |
| 15 to 25 | High |

There is no 7, 11, 13, or 14, because those products do not occur on a 1 to 5 times 1 to 5 grid. Do not force a row into a band by editing the score.

Treatment is one of: `Avoid`, `Mitigate`, `Transfer`, `Accept`.

- Avoid: stop the activity
- Mitigate: put a control in place and name it
- Transfer: a contract or insurance carries part of the consequence. You still own the relationship
- Accept: the Managing Director, or the role you name, accepts the score. Write that the acceptance is an assumption unless you have a note from that role

A treatment without an owner is unfinished.

Cover IT, OT, vendors, and personal information. A register that only lists malware on laptops is too narrow for this company. The sheets do not list the risks for you. Choose them from your interview notes.

Suggested minimum once you are done: 12 risks, with at least three that involve Red Dune OT or telematics, and at least two that involve personal information. That minimum is about coverage, not about which risks are worst.

## OT and IEC 62443

Read [assessment/ot-iec62443.md](../assessment/ot-iec62443.md) before you rate network and OT rows.

Work at zone level. Do not invent component security levels for every PLC. For each zone, decide a target security level only after you have written the consequence of a compromise. Leave the level blank if you cannot justify it.

Do not ask anyone to plug a laptop into a PLC, to scan the plant, or to test a bypass. This assessment uses interviews and documents. Say so in the report.

When a control exists in both ISO 27001 and the OT section, rate both, and say in the notes if the workshop practice and the Red Dune practice differ.

## From sheets to the report

Fill the sheets first. Then write the report from [report-template.md](report-template.md).

The executive summary is not a tour of every control. It answers:

1. What did you assess, and what did you leave out?
2. What are the few gaps that change safety, the Red Dune contract, or personal information?
3. What should happen in 30, 60, and 90 days, and who owns it?
4. What did you not see, so management should not treat the result as an audit certificate?

The roadmap is yours. A useful shape, which you still have to fill with your own actions:

- By day 30: name owners, confirm the top risks, and start the one exposure you are not willing to leave as it is
- By day 60: turn that response into a written practice the next shift can follow
- By day 90: show that the practice happened more than once, and set the next review date

If your evidence does not support an action, do not put it on the roadmap to look busy.

## Quality checks before you show the work

- Every `EXAMPLE ONLY` row is deleted
- No gap rating, tier, or score is filled without a note or an evidence id
- High priority items appear in the risk register and on the roadmap
- OT rows and IT rows are not copied from each other without a reason
- The report mentions POPIA where personal information is at risk, and the Cybercrimes Act where the scenario is an offence
- The fictional notice is still at the top of the README
- Nothing from a real employer, a real mine, or a real person has been added

## What you should not do

- Do not present this as a certified ISO 27001 audit or an IEC 62443 certification
- Do not paste the text of those standards into the repo
- Do not scan, exploit, or socially engineer a real network as "practice" for this project
- Do not use real identity numbers, real health records, or real credentials in the evidence folder
