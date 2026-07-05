# Label Configuration Proposal

> Map the scanned content to the four labels (Public / Internal / Confidential / Restricted)
> and the eight descriptors. Propose auto-labelling rules and Copilot scoping for go-live.
> Ground each choice in the provided deck.

## Label mapping

Label‑Configuration Proposal for Go‑Live

Legislative Assembly of British Columbia – Information Protection Program  

Prepared for: Director, Information Technology Division

Prepared by: Senior Data Strategist (Candidate)

Date: 5 July 2026



1\. Mapping the Scan Content to Assembly Labels \& Descriptors

The following table maps each site in your scan to the Assembly’s four labels (Public, Internal, Confidential, Restricted) and the eight descriptors (People, Proceedings, Legal, Commercial, Financial, Audit, Security, Member Support).

This mapping is grounded in the Information Protection deck’s principles:

Sensitivity first
Least privilege
Business function descriptors
BC Information Security Classification Standard

Site ID	Site Name	Label	Descriptor
S‑001	Corporate Communications	Public	People
S‑002	ITD Project Plans	Internal	Proceedings
S‑003	HR Benefits Enrolment	Confidential	People
S‑004	Finance Draft Budgets	Restricted	Financial
S‑005	Hansard – Broadcast Ops	Public	Proceedings
S‑006	Legal Opinions Library	Confidential	Legal
S‑007	Member Services Portal	Confidential	Member Support
S‑008	Vendor Contracts (active)	Confidential	Commercial
S‑009	IT Security Runbooks	Restricted	Security
S‑010	Committee Closed Sessions	Restricted	Proceedings
S‑011	General Staff Share	Internal	People
S‑012	Constituency Office Files	Confidential	Member Support
S‑013	ITD Project Plans	Internal	Proceedings
S‑014	Payroll Records	Restricted	Financial
S‑015	Public Job Postings	Public	People
S‑016	Audit and Review Findings	Restricted	Audit
S‑017	Leadership Briefing Notes	Confidential	Proceedings
S‑018	Training Materials	Internal	People
S‑019	Network Diagrams and Plans	Restricted	Security
S‑020	Personnel Reorg Planning	Confidential	People
S‑021	Expense Claims Archive	Confidential	Financial
S‑022	Old Records (pre‑2015)	Internal	Proceedings
S‑023	Media Releases Approved	Public	People
S‑024	Incident Response Active	Restricted	Security

2\. Auto‑Labelling Rules for Go‑Live

These rules follow the Information Protection deck’s guidance:

Content determines classification
Descriptors reflect business function
Labels reflect sensitivity and harm potential

2.1 Public – Auto‑Labelling Rules

Criteria: Approved for external release; disclosure poses no harm.
Triggers:
“media release”, “public job posting”, “Hansard”, “broadcast”, “public statement”, “approved for release”

Auto‑Label:  
Public + Descriptor: People or Proceedings
Deck grounding: Public = information intended for external audiences.

2.2 Internal – Auto‑Labelling Rules
Criteria: Routine operational information; low sensitivity.
Triggers:
“training”, “general staff”, “internal memo”, “project plan”, “draft planning”, “non‑sensitive operations”
Auto‑Label:  
Internal + Descriptor: People or Proceedings
Deck grounding: Internal = staff‑only, low‑risk information.

2.3 Confidential – Auto‑Labelling Rules
Criteria: Contains personal, member, legal, or commercial sensitivity.
Triggers:
“benefits enrolment”, “member services”, “constituency”, “contract”, “agreement”, “legal opinion”, “HR”, “reorg”, “expense claim”
Auto‑Label:  
Confidential + Descriptor: People, Legal, Commercial, Member Support, or Financial
Deck grounding: Confidential = information requiring controlled access due to personal, legal, or commercial sensitivity.

2.4 Restricted – Auto‑Labelling Rules
Criteria: Highest sensitivity; disclosure would cause significant harm.
Triggers:
“audit”, “risk”, “security runbook”, “network diagram”, “incident response”, “closed session”, “draft budget”, “payroll”
Auto‑Label:  
Restricted + Descriptor: Security, Audit, Financial, or Proceedings
Deck grounding: Restricted = information requiring strict controls due to security, audit, or financial sensitivity.

3\. Copilot Scoping Rules for Go‑Live
Copilot access must follow the deck’s least‑privilege and sensitivity‑based principles.

3.1 Public – Copilot Access
Copilot may:
Read, summarize, generate content
Use Public content in prompts and outputs
Deck grounding: No confidentiality risk.

3.2 Internal – Copilot Access
Copilot may:
Read and summarize
Generate internal documents
Copilot may not:
Surface Internal content externally
Combine Internal content with Public outputs
Deck grounding: Internal = staff‑only, low sensitivity.

3.3 Confidential – Copilot Access
Copilot may:
Summarize content for authorized users
Generate internal documents using Confidential inputs
Copilot may not:
Surface personal information
Combine Confidential content with Public outputs
Use Confidential content in general prompts
Deck grounding: Confidential = personal, legal, commercial sensitivity.

3.4 Restricted – Copilot Access
Copilot may:
Provide high‑level summaries only
Assist authorized users in drafting restricted documents
Operate in zero‑retention mode
Copilot may not:
Access raw Restricted content unless explicitly permitted
Generate detailed summaries of security, audit, or financial restricted data
Combine Restricted content with any other classification
Store or reuse Restricted content
Deck grounding: Restricted = highest sensitivity; strict controls required.

4\. Go‑Live Configuration Summary

Auto‑Labelling
Public → communications, broadcasts, job postings
Internal → training, general staff, non‑sensitive operations
Confidential → HR, member services, legal, commercial, financial personal data
Restricted → security, audit, incident response, payroll, draft budgets, closed proceedings
Copilot Scoping
Public → full access
Internal → controlled access
Confidential → limited access, no externalization
Restricted → high‑level only, zero‑retention, strict authorization
Deck Alignment
Every rule is grounded in:
BC Information Security Classification Standard
Assembly’s four‑label model
Descriptor taxonomy
Sensitivity‑first classification
Least‑privilege access control

## Auto-labelling rules

## Copilot and agent scoping

## Sample-document labels

|Document|Label|Descriptor|Reason|
|-|-|-|-|
|leadership\_pack\_draft.txt|Restricted|Proceedings|Five named individuals. Unpublished financial information. Confidential committee context. Sensitive personnel details.|
|procurement\_card\_review.txt|Internal|Financial|Internal review of financial date, possible update to confidential as it is not final and not shared. |
|media\_release\_approved.txt|Public|Proceedings|This is public information. Announced to public, approved, scheduled to post on website this afternoon. I selected Proceedings since it is an Assembly event.|



