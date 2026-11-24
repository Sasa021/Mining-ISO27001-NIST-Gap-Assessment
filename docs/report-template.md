# Gap assessment report template

Copy this file to `docs/amberkloof-gap-report.md` when you start writing. Fill the sections marked `To be completed by Mosa`. Leave the fictional notice and the South African context note in place. The context note is background, not a finding. The section under it, on what the law means for your results, is yours.

Do not paste ISO/IEC 27001 or IEC 62443 text into the report. Refer to control numbers, CSF subcategories, and your own evidence ids.

---

# Information security gap assessment

## Amberkloof Mining Systems (Pty) Ltd

**Fictional assessment.** Amberkloof is not a real company. This report is a portfolio exercise. It is not a certificate, not an audit opinion, and not legal advice.

| Field | Entry |
| --- | --- |
| Author | Mosa Mofokeng |
| Version | To be completed by Mosa |
| Date | To be completed by Mosa |
| Scope | Amberkloof IT and OT, as described in the company profile, unless you narrowed it |
| Status | Draft until the example rows are gone and the sheets match this report |

## 1. Executive summary

To be completed by Mosa.

Write one page or less. Use short paragraphs.

Cover only:

- What you assessed, including the four sites and the Red Dune OT plant
- What you left out of scope
- The few gaps that matter to safety, the operations contract, or personal information
- The highest risks, by the scores in your register, not by how worrying they sound
- What you want done in 30, 60, and 90 days
- What you could not evidence, so a reader does not treat this as a certification audit

## 2. Company and scope

To be completed by Mosa.

Summarise Amberkloof in your own words. Do not copy the whole profile. State the in scope systems and the client boundary with Red Dune Iron.

## 3. Method

To be completed by Mosa.

State that you used interviews against the fictional roles, the Annex A sheet, the NIST CSF 2.0 sheet, the risk register, and a high level IEC 62443 zone review. Name the rating scales you actually used. Say which roles you "interviewed" and which evidence you did not get.

## 4. ISO/IEC 27001 Annex A

To be completed by Mosa.

Do not paste all 93 rows into the report. Summarise by theme (A.5, A.6, A.7, A.8): how many controls you rated in each gap category, then discuss the ones that drive risk.

| Theme | Met | Partial | Not met | Not applicable |
| --- | --- | --- | --- | --- |
| A.5 Organisational | | | | |
| A.6 People | | | | |
| A.7 Physical | | | | |
| A.8 Technological | | | | |

The counts must match the CSV. If they do not, fix the CSV or the table before you publish.

### Gaps you want management to see

To be completed by Mosa.

For each gap you promote into this section, give the control id, the current state in one sentence, the evidence id, the owner, and the priority.

## 5. NIST CSF 2.0

To be completed by Mosa.

Describe the current and target profile by function: Govern, Identify, Protect, Detect, Respond, Recover. You can give a typical tier per function if you also mention the outliers. Do not average tiers into a false precision. A function can be Tier 2 in the office and Tier 1 at Red Dune. Say so.

| Function | What you observed | Current picture | Target picture |
| --- | --- | --- | --- |
| Govern (GV) | | | |
| Identify (ID) | | | |
| Protect (PR) | | | |
| Detect (DE) | | | |
| Respond (RS) | | | |
| Recover (RC) | | | |

Name the subcategories where the numeric gap is largest, and say whether that gap is also a high risk. A large tier gap on a minor outcome is not automatically a 30 day action.

## 6. Operational technology and IEC 62443

To be completed by Mosa.

Explain the zones you used and the Purdue reading from the company profile. For each zone, give the target security level you chose, or say you did not choose one and why.

State clearly that this is not an IEC 62443 certification. You used the ideas of zones, conduits, security levels, and the seven requirement themes to structure the OT review.

Call out anything that differs between the IT administrator's story and the artisan's story.

If a compromise of PitView, a PLC, or TrackOre could affect dust, water, or people, say that in plain language. That is a reason to prioritise, not a reason to hide the detail from the Managing Director.

## 7. Risk register

To be completed by Mosa.

Show the high band risks in full. Mention medium risks only if one of them is on the roadmap.

| Risk id | Asset | Score | Treatment | Owner |
| --- | --- | --- | --- | --- |
| | | | | |

The scores in this table must be the same numbers as in `assessment/risk-register.csv`.

## 8. South African context

This section is background for the exercise. It is not legal advice. Law changes by amendment and by commencement proclamations. Before you publish, check the latest text of the Acts and the Information Regulator's guidance. Then write section 8.3 yourself, from your findings.

### 8.1 POPIA

The Protection of Personal Information Act 4 of 2013 (POPIA) applies to the processing of personal information. Amberkloof, if it were real, would hold employee files, payroll data, occupational health records, CCTV, and driver identity in the telematics platform. Health information is special personal information. The company would need a lawful basis to process it, not only a security control.

In plain language, POPIA expects a responsible party to:

- Decide who is accountable for personal information
- Collect only what is needed, for a clear purpose
- Keep it accurate
- Tell people what is being done with it
- Protect it with reasonable technical and organisational measures
- Let people ask for access and correction
- Use operators (suppliers who process personal information for you) under a written arrangement

Security safeguards sit in section 19. The duty is to take appropriate, reasonable technical and organisational measures against loss, damage, and unauthorised access, and to identify reasonably foreseeable risks.

Suppliers such as PayMica, Stonehealth, Highveld Cloud Backup, TrackOre, and Microsoft may be operators for some of this information. Section 21 requires a written contract and requires the operator to tell the responsible party at once if there are reasonable grounds to believe personal information was accessed or acquired by an unauthorised person.

Section 22 deals with a compromise. Where there are reasonable grounds to believe personal information was accessed or acquired by an unauthorised person, the responsible party must notify the Information Regulator and the data subject as soon as reasonably possible. POPIA does not set a fixed number of hours. Notification can be delayed if a public body responsible for crime prevention, or the Regulator, decides that telling the data subject would impede a criminal investigation. The Act lists what the notice must cover, including what happened, what measures are being taken, and a recommendation of what the person can do.

Section 72 covers sending personal information outside South Africa. You need to know where Microsoft 365 and any other cloud service actually store the data before you can say whether a cross border condition is met. The company profile leaves the tenant region unknown on purpose.

Useful official source: the Information Regulator, [inforegulator.org.za](https://inforegulator.org.za/).

### 8.2 Cybercrimes Act

The Cybercrimes Act 19 of 2020 creates criminal offences for cyber conduct. The parts that create the main offences came into force on 1 December 2021. They include unlawful access, unlawful interception, unlawful interference with data or a computer system, unlawful acts involving passwords or software tools, cyber fraud, cyber forgery, cyber extortion, and certain harmful data messages.

If Amberkloof were a victim, for example if someone broke into email or interfered with a PLC, the practical step is to preserve logs and report the crime to the South African Police Service so there is a case number. Preserving evidence supports Annex A control themes on evidence collection and the NIST Respond outcomes. It is also how a company helps a criminal investigation.

Section 54 would place a reporting duty on electronic communications service providers and financial institutions. It tells those organisations to report certain offences on their own service or network to the South African Police Service without undue delay and, where feasible, within 72 hours, and to preserve information that may help the investigation. Failure would be an offence with a fine not exceeding R50 000. Section 54 was excluded from the commencement fixed for 1 December 2021 in the proclamation published in Government Gazette 45562. Public guidance still described it as not in force during 2026. Check the Gazette before you rely on it. Even when it is in force, Amberkloof is not, on the facts in this profile, an electronic communications service provider or a financial institution. Bushlink might be, for its own network. Do not give Amberkloof a section 54 duty it does not have. Do not ignore a crime because section 54 does not apply. A victim can still report.

POPIA and the Cybercrimes Act do different jobs. POPIA is about lawful processing and telling people when their information is compromised. The Cybercrimes Act is about offences. One incident can trigger both.

The Mine Health and Safety Act 29 of 1996 still matters as context. A cyber event that stops dust suppression or changes a pump can be a safety event on a mine. Your report should say how Amberkloof would warn its own people and the client. Do not invent a section number you have not read.

### 8.3 What this means for your results

To be completed by Mosa.

Tie the law to your own rows. For example, name which risks involve employee or health information, whether an operator agreement showed up in evidence, and whether the incident process tells someone to notify the Regulator and to preserve logs for the police. If you did not see those practices, say that. Do not claim Amberkloof complies with POPIA.

## 9. Roadmap, 30, 60, and 90 days

To be completed by Mosa.

Actions must come from your high priority gaps and your high band risks. Each action needs one owner and something you could look at afterwards to see that it happened.

| Window | Outcome you want | Actions | Owner | How you will know it happened |
| --- | --- | --- | --- | --- |
| Day 1 to day 30 | | | | |
| Day 31 to day 60 | | | | |
| Day 61 to day 90 | | | | |

Add rows if you need them. Do not add actions that have no link to a risk id or a control id.

## 10. Limitations

To be completed by Mosa.

State that the interviews were a solo exercise on a fictional company, that you did not test technical controls, and that you did not certify any zone. List the evidence you wanted and did not have.

## 11. Conclusion

To be completed by Mosa.

Four to eight sentences. What should the Managing Director do first, and what are you not claiming?

## Document history

| Version | Date | Author | What changed |
| --- | --- | --- | --- |
| 0.1 | | Mosa Mofokeng | First draft from the scaffold template |
