# Inspection Issue Log

**Project:** SNU Research Grants Management System (RGMS), Draft SRS for Inspection (package 3.zip)
**Meeting Date:** 2026-11-23
**Recorder:** Ayush Gupta

- **Type:**
	- For individual requirements: **Incomplete** (missing parts), **Invalid** (does not follow from stakeholder needs), **Infeasible**, **Ambiguous**, **Unverifiable**, **Untraceable**.
	- For sets (e.g. the entire feature): **Incomplete**, **Inconsistent**, **Untraceable**
- **Severity:** **Major**, **Minor**
- **Location:** Offer section and page number.

## Issues

| # | Type | Severity | Location | Description |
| --- | --- | --- | --- | --- |
| 1 | Ambiguous | Minor | intro/1.2.Convention.md | Requirement numbering (e.g. 3.1.2.1) does not distinguish section, use case and requirement identifiers. Evidence codes E1 to E7 cannot be found in the evidence appendix. "N/A" does not distinguish "not applicable" from "not yet specified". |
| 2 | Ambiguous | Minor | intro/1.3.ProjectScope.md | Scope describes the complete lifecycle (review, grading, ranking) while the main file says this draft excludes them. It is not stated which scope applies. |
| 3 | Inconsistent | Minor | Main.md, Appendices | The link to "Vision and Scope.pdf" is broken. The file is in the evidence folder under a different name. |
| 4 | Inconsistent | Minor | overview/2.1.ProductPerspective.md | The release timeline cites Vision and Scope section 4.2, but the roadmap is in section 2.3. The February 2028 release date is not supported by the Vision and Scope document. |
| 5 | Ambiguous | Minor | overview/2.2.UserClasses.md, population column | Populations are marked "TBD" while numbers are given beside them (312 faculty members, 17 departments). |
| 6 | Ambiguous | Minor | overview/2.3.OperationalEnvironment.md | "Standard web browser" is not defined (browsers, versions). Remote versus on-campus access and hosting are not specified. |
| 7 | Incomplete | Minor | overview/2.4.DesignImplementation.md | The development team is not described; only the course deadline is given. "Protected even if the database is breached" has no testable criterion. |
| 8 | Incomplete | Minor | overview/2.5.AssumptionAndDependency.md | The assumption that Keycloak supplies role information is not supported by evidence. No behaviour is defined when the HR system or the Student Information System is unavailable. |
| 9 | Incomplete | Major | uc/3.0.Overview.md, section C | The use case diagram is missing (marked N/A). |
| 10 | Incomplete | Major | All six use case files, sections C and D | System sequence diagrams or activity diagrams and mock-ups are marked N/A in every use case. |
| 11 | Untraceable | Major | All six use case files, YAML header | The related-evidence field is empty and no use case has an Evidence section, so no use case traces to the stakeholder evidence. |
| 12 | Incomplete | Major | uc/3.1.1.AuthenticeUser.md | The actor list omits CoR Member, CoR Chair and Dean. There is no flow for a user reported inactive by HR or the Student Information System, or for those services being unavailable. |
| 13 | Inconsistent | Minor | uc/3.1.2.ManageRoleBasedAccess.md | Quality requirements are copied from 3.1.1 and concern sign-in, not role management. Alternative Flow 1 assigns roles automatically, which conflicts with BR-2 (roles assigned by IT only). "HR/SRS" should read SIS. |
| 14 | Incomplete | Minor | uc/3.2.1.ManageApplicationDraft.md | Postconditions are inconsistent with the delete flow. Eligibility failure and save failure have no defined outcome. Create, view, edit and delete are combined in one use case. |
| 15 | Inconsistent | Major | overview/2.2.UserClasses.md; uc/3.2.2.SubmitApplication.md, step 3 | Section 2.2 says Department Chair approval is not confirmed, but use case 3.2.2 checks it as a required step. Most of the evidence (Research Officer email, applicant email, Dean interview 2) says the Chair must sign; the conflict with Dean interview 1 is not resolved. |
| 16 | Ambiguous | Minor | uc/3.2.2.SubmitApplication.md, Alternative Flows 1 and 2, Exception 2, Quality Requirements | Alternative flows do not state where they return to the main flow. "Chair not responding" has no time limit. "Deadline-day peaks" and "immediately" are not measurable. |
| 17 | Incomplete | Major | uc/3.2.2.SubmitApplication.md | The maximum request amount is not checked at submission. The Department Chair signs in Alternative Flow 1 but is not listed as an actor, and there is no Department Chair approval use case. |
| 18 | Inconsistent | Major | uc/3.3.1.ManageGrantPrograms.md, step 3; br/BusinessRules.md BR-5 | The use case lets the Research Officer add programs, while BR-5 allows only the four existing programs. |
| 19 | Incomplete | Major | uc/3.3.1.ManageGrantPrograms.md; br/BusinessRules.md | The maximum request amounts ($15,000 for DF and SRG, $5,000 for MRG and JF) are missing from program setup and from the business rules. |
| 20 | Incomplete | Major | uc/3.3.2.OrganizeSubmittedApplications.md | Postconditions for success and return contradict each other. Returned applications have no resubmission flow. |
| 21 | Incomplete | Major | Section 3 (feature list) | There is no use case for applicants to view the status of their application, although the applicant evidence identifies missing status visibility as a main problem. |
| 22 | Inconsistent | Major | datareqs/4.3, DR-05 | DR-05 states that grade corrections are not permitted, while the CoR Chair email states that members revise grades during the meeting. |
| 23 | Ambiguous | Major | datareqs/4.3 (DR-03, DR-05, DR-06, DR-12) | Several data rules are fragmented and unclear. The file contains unusual punctuation characters and has no YAML header. |
| 24 | Incomplete | Minor | ifaces/5.2.Software-Interfaces.md | Role provisioning and notification failure handling are left open. No sequence diagrams or data formats are given for the interfaces. |
| 25 | Untraceable | Minor | qualities/6.5.Security.md, SEC-01 | Only one requirement; its supporting evidence is marked as still to be checked. The YAML header lacks author and related fields. |
| 26 | Untraceable | Major | br/BusinessRules.md | No rule cites a source. BR-2, BR-4, BR-5 and BR-7 are unclear or conflict with use cases. Use case YAML links do not match the rule headings (e.g. "BR-2 - Roles assigne by IT only", "BR-3 - Applicants can only see their own applications"). |

**Totals:** 26 issues (13 Major, 13 Minor)

---
*Copyright © 2001 by Karl E. Wiegers. Permission is granted to use, modify, and distribute this document.*
