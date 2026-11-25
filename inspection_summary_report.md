# Inspection Summary Report

## Inspection Identification

- **Project:** SNU Research Grants Management System (RGMS), Draft SRS for Inspection (package 3.zip)
- **Meeting Date:** 2026-11-23, online (Zoom), recorded

## Work Product Description

- Anonymized draft SRS received from the instructor on Nov 19, 2026 as 3.zip (folder "SNU-SRS-DRAFT-Draft-for-Inspection"), version 0.1, status "in progress".
- Markdown repository based on the course SRS template: Main.md; intro/ (1.1 to 1.3); overview/ (2.1 to 2.5); uc/ (3.0 overview and six use cases 3.1.1, 3.1.2, 3.2.1, 3.2.2, 3.3.1, 3.3.2); datareqs/4.3; ifaces/5.2; qualities/6.5; br/BusinessRules.md (BR-1 to BR-7); evidence/ (interview transcripts, stakeholder emails, Vision and Scope PDF).
- Inspected: the sections the instructor required for the draft (Sections 1 and 2, Section 3 up to and excluding adjudication, 4.3, 5.2, one quality attribute, Business Rules, Domain Evidence). Empty template files (4.1, 4.2, 5.1, 5.3, 5.4, 6.1 to 6.4, 6.6, glossary) were not inspected.

## Inspectors

| # | Role | Inspector | Preparation Time (hours) |
| --- | --- | --- | --- |
| 1 | Author | N/A (authoring group anonymous, not present) | - |
| 2 | Moderator | Mohammad Mustafaa Hameed | 2.0 |
| 3 | Recorder | Ayush Gupta | 2.0 |
| 4 | Reader | Mohammad Shahnaei | 3.0 |

## Inspection Data

| Metric | Value |
| --- | --- |
| Planned for Inspection | 11 pages (about 5,300 words of SRS; evidence appendix used for cross-checking) |
| Actually Inspected | 11 pages |
| Meeting Time | 2.0 hours |
| Total Planning Effort | 1.0 labor hours |
| Total Overview Effort | 0 labor hours (no separate overview meeting) |
| Total Preparation Effort | 7.0 labor hours |
| Actual Rework Effort | N/A (rework is done by the authors) |

## Inspection Process Description

- **Planning:** roles and meeting time were agreed in the group chat. Moderator: Mohammad Mustafaa Hameed. Reader: Mohammad Shahnaei. Recorder: Ayush Gupta. The Reader shared his written walkthrough (Main.md and every linked file) before the meeting.
- **Preparation:** each inspector read the full draft beforehand against a checklist of completeness, correctness, consistency, unambiguity, verifiability, feasibility, traceability and template conformance. The Recorder prepared the issue log template and a list of candidate defects, checked against the authors' evidence files.
- **Meeting:** held online on Zoom on Nov 23, 2026, and recorded. Each member introduced themselves and their role at the start.
- **Order:** the document was inspected in Main.md order: 1.1 to 1.3, 2.1 to 2.5, 3.0 and each use case, 4.3, 5.2, 6.5, Business Rules and evidence.
- **Turn taking:** for each section the Reader summarized the content, gave his interpretation and raised candidate defects. The Moderator then invited the other two members to agree, disagree or add new issues, one at a time. Discussion was kept to identifying defects, not fixing them. Points already raised were not repeated.
- **Recording:** the Recorder logged each agreed issue with type, severity and location, using the instructor's types (Incomplete, Invalid, Infeasible, Ambiguous, Unverifiable, Untraceable, Inconsistent) and severities (Major, Minor).
- **Close:** near the two-hour limit, the Recorder read back the first 20 issues for confirmation. The remaining 6 had been agreed during the walkthrough and were confirmed for the log. The group agreed on the recommendation.
- **Not covered:** nothing was skipped. Empty template files were out of scope for the draft.

## Summary of Issues

26 issues were logged: 13 Major and 13 Minor. The most important and recurring ones:

1. **Department Chair approval is inconsistent.** Section 2.2 says it is not confirmed, but use case 3.2.2 requires it. There is no Chair approval use case, and the Chair is not an actor (issues 15, 17).
2. **Required models are missing.** There is no use case diagram, and no system sequence diagrams or mock-ups in any use case (issues 9, 10).
3. **Traceability is weak throughout.** related-evidence is empty in every use case, no business rule cites a source, and evidence codes cannot be followed (issues 1, 11, 25, 26).
4. **Business rules are missing or conflicting.** The maximum request amounts are absent, and adding programs conflicts with BR-5 (issues 18, 19).
5. **Section 4.3 is hard to read.** It has fragmented rules, and DR-05 contradicts stakeholder evidence on grade revisions (issues 22, 23).
6. **Use cases are incomplete.** Several have missing return points, failure flows and contradictory postconditions, and there is no application-status use case (issues 12, 14, 16, 20, 21).

## Product Appraisal

**RECOMMENDATION**
- [ ] accepted as is
- [ ] conditionally accepted upon verification
- [x] reinspect following rework
- [ ] inspection not completed

**OTHER COMMENTS**

The draft follows the template structure, is concise, and its scope statement and exclusions are clear. The major issues are concentrated in traceability, missing models and the Department Chair approval workflow. Resolving these should make the next version much stronger.

----
*Copyright © 2001 by Karl E. Wiegers. Permission is granted to use, modify, and distribute this document.*
