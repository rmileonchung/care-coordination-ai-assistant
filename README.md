# Care Coordination AI Assistant
### A prompt engineering project by Rachel Mileon-Chung

## What This Is
A lightweight AI tool that takes a Medicaid case manager's daily caseload data
and generates a prioritized work plan — flagging overdue items, compliance risks,
and recommended actions in plain language.

## The Problem It Solves
Care managers in Medicaid managed care programs manage 60+ active members simultaneously.
Daily prioritization is manual and reactive. This tool uses AI to triage the
caseload automatically, so case managers spend less time figuring out what to do
first and more time doing it.

## How It Works
1. Input: structured caseload data (member ID, risk level, visit dates, outstanding items)
2. AI prompt: instructs Claude to assess urgency and generate a ranked action plan
3. Output: prioritized daily work list + supervisor summary + compliance escalation flags

## Files In This Project
- mock-caseload-data.txt — sample caseload input (8 members, fictional data)
- ai-output-sample.txt — 1. Prioritized daily work plan — June 2, 2026
1.	M-004 — Critical: Complete escalation outreach today for the missed overdue visit, document all call attempts, contact emergency/alternate contacts if available, and escalate to a supervisor because the member has dementia, is unresponsive, and has no legal representative on file.
Risk if not addressed: Potential member safety issue, missed required monitoring, and compliance exposure due to overdue visit/note and lack of representative.
2.	M-007 — Critical: Complete and document Transition of Care follow-up today, confirm discharge status/services/medications, and prioritize the note since the visit was due 06/01 and the note is due 06/03.
Risk if not addressed: Hospital discharge gaps, medication/service interruptions, avoidable readmission, and late documentation.
3.	M-001 — High: Submit the overdue fall report today, verify member status after the fall, and begin POA/legal representative follow-up.
Risk if not addressed: Unreported falls may raise safety, quality, and compliance concerns; missing POAs may delay consent and care coordination.
4.	M-005 — Medium: Follow up today on the pending ALF placement change and obtain/confirm the updated address.
Risk if not addressed: An incorrect address can lead to missed visits, service disruptions, and inaccurate member records.
5.	M-002 — Medium: Start the care plan renewal today since it is due 06/15, and confirm whether any new needs or service changes are required.
Risk if not addressed: Care plan may fall behind, causing service planning delays and possible compliance issues.
6.	M-008 — Medium: Complete the monthly call today or send a self-check-in text since the member is competent and eligible.
Risk if not addressed: Missed monthly contact may affect the timeliness of monitoring and documentation.
7.	M-006 — Low: Confirm whether the welcome package was received and document the response.
Risk if not addressed: Minor onboarding gap; member may miss important plan/contact information.
8.	M-003 — Low: No urgent action needed today; continue routine monitoring and keep next visit/note dates on tracker.
Risk if not addressed: Low today, but missed tracking could lead to late documentation in the future.
2. Supervisor-ready summary
Today’s highest priorities are M-004, M-007, and M-001 due to overdue visits/notes, safety concerns, hospitalization follow-up, fall reporting, and missing legal representative documentation. M-004 requires immediate escalation because the member has dementia, is unresponsive, and has no legal rep on file. After addressing those urgent cases, the next focus should be ALF address confirmation for M-005, preparation of the care plan renewal for M-002, and monthly contact for M-008.
3. Compliance flags to escalate today
•	M-004: Overdue visit, overdue note, missed visit, unresponsive member, dementia, and no legal representative on file.
•	M-007: Hospitalization last week with Transition of Care not documented; visit due 06/01 and note due 06/03.
•	M-001: Overdue note, fall report not submitted, and no POA on file.
•	M-005: Pending ALF placement changes with no updated address, which may affect service delivery and visit compliance.

- README.md — this file

## Why I Built This
I have managed 60+ Medicaid members simultaneously at Florida Community Care.
Prioritization was always manual. This is the tool I wish existed.

## Tools Used
- Claude.ai (prompt engineering)
- GitHub (documentation and hosting)

## About
Built as part of a Health IT AI portfolio project.
Rachel Mileon-Chung | mileonrachel@outlook.com
linkedin.com/in/rachelmileon-chung
