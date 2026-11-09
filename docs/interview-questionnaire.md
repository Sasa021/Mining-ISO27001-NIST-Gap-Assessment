# Interview questionnaire

Use this with [method.md](method.md) and the [company profile](../company-profile/README.md).

Write answers in the evidence folder, not in this file. Keep this questionnaire blank so the questions stay reusable.

For every answer, record the role, the site, whether the statement is from the profile or an `Assumption:`, and the evidence id if you create one.

Do not fill gap ratings in the interview note. Facts only.

## 1. Opening, for every role

1. What is your job, and which site do you spend most of your time on?
2. Which systems would stop your work this week if they were unavailable?
3. Who do you call when something on those systems looks wrong?
4. What were you told about this assessment, and what is out of scope for your team?

## 2. Governance and risk

Ask the Managing Director, then check the same topics with the IT administrator and the operations superintendent.

5. Who is accountable for cybersecurity risk? Is that written down anywhere?
6. Is there a written information security policy? Who approved it, and when was it last read by staff?
7. What risks has the company already agreed to accept? Where is that decision recorded?
8. How does a cyber risk get onto the same table as a safety or a money risk?
9. What would you refuse to let a client or a vendor do on your systems?
10. Is there a budget or a named person for security work this year? What is in or out of that budget?
11. When a project starts, such as a new pump skid or a new depot link, who asks the security questions?

## 3. Assets and data

12. Where is the list of laptops, servers, and network gear? When was it last updated?
13. Where is the list of PitView servers, HMIs, PLCs, and the engineering workstation?
14. Who owns the drawings and the PLC project files? Who is allowed to copy them onto a laptop?
15. What personal information does Amberkloof hold, and who is the responsible party for each set?
16. Does Stonehealth keep the health records, or does Amberkloof keep a copy?
17. Does TrackOre store driver names and locations? Who at Amberkloof can pull that history?
18. Where does the Microsoft 365 tenant sit, in South Africa or in another country?
19. What is on the workshop CCTV recorder, and how long is it kept?

## 4. Identity and access

20. How does a new employee get an account, and how fast is it removed when they leave?
21. Who has administrator rights in Active Directory, in Microsoft 365, in Ledgerpit, and on the firewalls?
22. How do people sign in? Is there a second factor for email, for remote access, and for the MSP?
23. How does the control room artisan sign in to PitView and to the engineering workstation? Is that account shared?
24. How does a vendor such as DeskOrchard, Bushlink, or Mothlight get access? Is the access closed after the job?
25. Can someone in Centurion reach a PLC, or only the jump host? Who approves that session?
26. What happens to accounts for contractors when the rotation ends?

## 5. Physical and people

27. Who can walk into the server corner in Centurion, the workshop electrical bay, and the Red Dune control room?
28. How are visitors and contractors inducted at Red Dune? Who keeps the record?
29. Are staff screened before they are hired into the control room or into payroll?
30. What security training have staff had in the last year? Is OT staff included, or only office staff?
31. What should a driver or an artisan do if they receive a strange email or a strange USB stick?
32. Is there a disciplinary path if someone misuses an account or a PLC password?

## 6. Suppliers, cloud, and the client boundary

33. Which suppliers can see Amberkloof data or connect to Amberkloof systems? Is there a list?
34. What does the DeskOrchard contract say they may do, and what must they report back?
35. What does the Highveld Cloud Backup contract say about where backups are stored and who may restore them?
36. What does PayMica have to tell Amberkloof if payroll data is exposed?
37. Does any contract require a supplier to tell Amberkloof about a security compromise?
38. Which paths, if any, exist between Amberkloof and the Red Dune Iron network?
39. Who at the client would Amberkloof phone if the water circuit had to stop for a security reason?

## 7. Operations, change, backup, and vulnerabilities

40. How are changes made to Ledgerpit, to firewalls, and to PLC logic? Is there a record?
41. Who is allowed to load a PLC project, and is there a second person?
42. What is backed up, how often, and when was a restore last tried?
43. How do laptops and servers get security updates? What about PitView, the HMIs, and the PLCs?
44. Is there a list of known vulnerabilities, or a person who reads vendor notices?
45. Is the panel test bench in eMalahleni on the workshop LAN? What can it reach?
46. How do you know a Shieldline alert was looked at?

## 8. Detection, incidents, and recovery

47. Who watches for a bad event after hours? Is that the MSP, the IT administrator, or nobody?
48. What counts as an incident, as opposed to a fault on the plant?
49. Is there a written incident process? Has anyone used it?
50. If payroll data or health data were copied out, who would tell the Information Regulator and the data subjects, and how fast?
51. If someone broke into email or changed a PLC, would anyone report it to the South African Police Service?
52. What would you restore first at Red Dune, and what would you restore first in Centurion?
53. How would you tell the client, the depot, and staff, without using the system that has failed?

## 9. OT, telematics, and remote sites

Ask the superintendent and the artisan. Then check the IT administrator's version of the same facts.

54. Walk through the Purdue sketch. Which lines on the drawing are real, and which are wishes?
55. Is the jump host in place today? Who can log on to it?
56. What happens to the pumps and sprays if PitView stops? Do they hold the last state, or is there a local mode?
57. How does the artisan reach the plant from home, if at all?
58. How do the water trucks talk to TrackOre? Could that path reach a PLC?
59. What would a wrong set point or a stopped spray mean for dust, water, and people on the pit?
60. Who is allowed to change a set point, and is the change visible the next day?
61. Lepelle Depot: who looks after the PCs when the supervisor is on leave?
62. Has anyone from a supplier connected a laptop to a panel on site in the last year? What was the rule?

## 10. Close, for every role

63. What is the one failure you hope I do not ignore?
64. Which document should I read next, and who can give it to me?
65. What did I misunderstand about your site?

## Evidence to ask for

Tick these in your evidence index as `Provided`, `Not provided`, or `Assumption`. Do not rate a control as `Met` on a verbal claim alone.

| Id to assign | Item |
| --- | --- |
| You choose | Information security policy, or a note that none was produced |
| You choose | List of users with administrator rights |
| You choose | Joiner and leaver record for the last few months |
| You choose | Asset list for IT, and a separate list for OT |
| You choose | The network sketch signed or corrected by the person who drew it |
| You choose | Backup job list and the last restore test |
| You choose | Vendor list and the DeskOrchard, PayMica, and Highveld contracts, or the clauses that exist |
| You choose | Incident or fault tickets that had a security angle |
| You choose | Training attendance |
| You choose | A sample PLC change record, or a note that none exists |
| You choose | Microsoft 365 tenant region |
| You choose | Who holds Stonehealth records, and the operator agreement if there is one |

When you write a fictional document to stand in for one of these, label it `Fictional evidence created for this exercise` on the first line.
