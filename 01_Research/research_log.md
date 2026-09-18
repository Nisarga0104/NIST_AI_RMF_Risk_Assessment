# Research Log — NIST AI RMF Risk Assessment
Date: 2026-09-13

Covers: NIST AI RMF's own function structure, the RBI regulatory context, and the DPDP Act
commencement timeline. Verification status is inline with each finding rather than in a
separate file, since this is a framework-mapping project, not a research-report project.

## Search 1 — "NIST AI Risk Management Framework AI RMF 1.0 Govern Map Measure Manage functions"
Purpose: verify the framework's structure before using it to organize the assessment.
Result: Confirmed. AI RMF 1.0 (NIST AI 100-1), published January 26, 2023, is voluntary
guidance organized around four core functions — Govern, Map, Measure, Manage — with Govern
treated as the cross-cutting function that informs the other three. Multiple independent sources
converge on 19 categories and roughly 72 subcategories distributed across the four functions
(this subcategory count wasn't checked against the primary PDF line-by-line, but isn't
load-bearing for anything cited in the mapping). Your draft's characterization of Govern as
"cross-cutting" and its function-by-function structure matches the actual framework — no
correction needed to the framework description itself.
**Source:** National Institute of Standards and Technology (2023). AI Risk Management Framework
(AI RMF 1.0). NIST AI 100-1.

## Search 2 — "RBI guidelines NBFC IT governance outsourcing digital lending 2026"
Purpose: your draft cites "RBI guidance on outsourcing of IT services and digital lending"
generically, without naming specific regulations. Checked what an actual current, named
citation would be.
Result: Found three specific, current, named RBI instruments an Indian NBFC would actually be
assessed against right now — used to replace the generic reference in the final mapping:
1. **RBI (NBFC — Outsourcing of IT Services) Directions, 2025** — in effect from 28 November
   2025 for new IT outsourcing contracts; existing contracts must transition by 10 April 2026
   or at renewal, whichever is earlier. Requires board-approved IT outsourcing policy, a central
   register of material outsourcing arrangements, audit rights over vendors and sub-vendors, and
   cyber-incident reporting via vendors within a window short enough for the NBFC to meet RBI's
   own 6-hour reporting requirement.
2. **RBI (NBFC — Cybersecurity, Technology Risk, Resilience and Assurance) Directions, 2026** —
   repeals the earlier IT Governance framework for NBFCs; requires incident reporting on the
   DAKSH platform within 6 hours of detection, periodic reviews/audits, and governance
   responsibilities scaled to NBFC category.
3. **RBI Digital Lending Directions, 2025** (issued 8 May 2025) — consolidated framework
   replacing the 2022 digital lending guidelines; governs Lending Service Provider (LSP)
   relationships directly relevant to Northstar's third-party-LLM vendor dependency.

## Search 3 — "DPDP Act 2023 commencement status September 2026 Data Protection Board rules notified"
Purpose: verify the DPDP Act commencement timeline stated in the draft, since this is the
fastest-moving fact in the document.
Result: **Your draft was already accurate and did not need correction.** Confirmed: DPDP Rules,
2025 notified 13 November 2025 (G.S.R. 843(E)); Data Protection Board established same day;
staged three-phase commencement — machinery/Board provisions in force immediately, Consent
Manager provisions from 13 November 2026, and the Act's substantive consent/notice/breach-
notification obligations from 13 May 2027. One live/ongoing item worth flagging: a Supreme
Court challenge to the Act was pending as of August 2026 (notice issued, no interim stay, no
provision struck down) — doesn't change the stated dates, but added as a one-line caveat since
this specific fact moves fast.
**Source:** Ministry of Electronics and Information Technology, Government of India. Digital
Personal Data Protection Act, 2023, and DPDP Rules, 2025 (notified 13 November 2025).

## Net changes applied to the final mapping and full assessment
- RBI reference upgraded from generic description to the three named, dated regulations above.
- One-line DPDP Supreme Court caveat added.
- DPDP commencement dates and the NIST function structure required no changes — already accurate.
