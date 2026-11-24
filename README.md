# ArchiveReports

# PROJECT 09 — DIGITAL FOOTPRINT ASSESSMENT
**External Exposure & Open-Source Intelligence Research**

**Project ID:** DFRA-2026-009  
**Project type:** OSINT / Cybersecurity Research / Exposure Assessment  
**Team size:** 2 researchers  
**Difficulty:** Beginner  
**Duration:** 10 working days  
**Estimated effort:** 15–25 hours per researcher  
**Budget:** €0  
**Target:** An owned or explicitly authorized domain/organization  
**Distribution:** Private working report; separate sanitized public edition  
**Status:** Project planning — not yet assessed

---

## 1. Executive Project Overview

### 1.1 Project Description

The Digital Footprint Assessment project investigates what information about an organization, website, or digital service is publicly visible on the internet.

The research team will collect and analyze open-source information to understand the subject's digital presence, discover publicly associated internet assets, document potential information exposures, and propose practical security improvements.

The assessment focuses on passive reconnaissance, public information analysis, evidence validation, risk evaluation, and professional reporting.

**Primary research question:**

*What can an external observer discover about the selected organization through publicly accessible information, and which verified exposures may create cybersecurity or privacy risks?*

### 1.2 Learning Objectives

By completing the project, both researchers should be able to:

1. Explain digital footprint analysis and external attack surface management.
2. Define and document an authorized research scope.
3. Perform structured OSINT investigations.
4. Identify publicly associated domains, subdomains, services, and digital assets.
5. Research DNS records and certificate transparency data.
6. Investigate public websites, repositories, and archived content.
7. Recognize potential information disclosure risks.
8. Validate observations and distinguish facts from assumptions.
9. Prioritize confirmed findings using a documented risk methodology.
10. Produce an evidence-based professional cybersecurity report.

### 1.3 Expected Outcomes

The project should produce:

- A documented inventory of observed digital assets.
- A structured evidence register with verified sources.
- An analysis of public information exposure.
- A timeline of relevant historical observations where available.
- A risk register containing confirmed findings and potential concerns.
- An actionable remediation plan.
- A professional technical report and public portfolio summary.

There is no requirement to discover a vulnerability. A well-supported conclusion that no significant exposure was identified within the assessment scope is a legitimate research outcome.

---

## 2. Research Scope and Rules

### 2.1 Selecting a Research Target

**Recommended options:**

- A personal domain owned by either researcher.
- A website or online project managed by the team.
- A small business whose owner provides explicit permission.
- A fictional organization with synthetic records.
- An educational environment prepared specifically for this assessment.

**Best beginner option:** Assess a website/domain you control, along with its associated public GitHub repositories and deliberately published test documents.

If no suitable real target exists, create a fictional company called *Northstar Digital* using synthetic assets and sample data. In that case, the final product must be labeled a simulated digital footprint assessment.

### 2.2 Included Activities

- Search engine research.
- Passive DNS and registration data lookups.
- Public certificate transparency research.
- Public website content review.
- Historical website archive analysis.
- Public GitHub repository review.
- Publicly posted document metadata analysis.
- Examination of organization-owned social media pages.
- Correlation and validation of observed information.
- Basic DNS and HTTP configuration checks on authorized assets.

### 2.3 Excluded Activities

- Port scanning or vulnerability scanning without separate authorization.
- Password attacks and credential testing.
- Attempted account access or authentication bypass.
- Social engineering or contacting employees under false pretenses.
- Accessing restricted documents, databases, or systems.
- Downloading exposed credentials or private datasets.
- Intrusive subdomain enumeration.
- Unapproved testing of third-party infrastructure.

The discovery of a third-party service associated with the organization does not automatically authorize testing that service.

### 2.4 Scope Record

Before beginning, complete the following:

| Scope field | Required entry |
|---|---|
| Organization / project | Approved target name |
| Primary domain | Authorized domain |
| Approved subdomains | Listed explicitly or defined by owner |
| Approved GitHub accounts | Usernames or organizations |
| Other public assets | Websites and channels |
| Assessment dates | Start and end dates |
| Research methods | Passive OSINT, plus specifically approved checks |
| Authorization | Owner approval reference |
| Restrictions | Exclusions and sensitive-data rules |
| Reporting contact | Authorized recipient |

**Gate:** No target-specific investigation begins until authorization and scope have been documented.

---

## 3. Research Team and Responsibilities

### Researcher A — OSINT & Asset Discovery Lead

**Primary mission:** Discover, document, and map the target's publicly visible digital presence.

Responsibilities:

- Coordinate scope approval.
- Research the organization's public identity.
- Discover publicly associated domains and subdomains.
- Review DNS and registration data.
- Research certificate transparency records.
- Examine public repositories and document references.
- Build the asset inventory.
- Prepare the infrastructure and exposure map.
- Draft the asset discovery and methodology sections.

**Assigned deliverables:**

- Asset inventory.
- OSINT search log.
- Domain and DNS observations.
- Certificate transparency review.
- Asset relationship diagram.
- Initial evidence collection.

### Researcher B — Exposure & Risk Analysis Lead

**Primary mission:** Evaluate the verified observations and document their cybersecurity implications.

Responsibilities:

- Review public website disclosures.
- Analyze authorized public documents and metadata.
- Inspect public repository configuration information.
- Evaluate findings supplied by Researcher A.
- Identify and prioritize possible security weaknesses.
- Build the risk register.
- Research mitigation guidance.
- Draft the risk assessment and recommendations.
- Integrate the final report.

**Assigned deliverables:**

- Exposure assessment.
- Risk register.
- Finding validation notes.
- Recommendations and remediation plan.
- Executive summary.
- Final report assembly.

### Shared Responsibilities

Both researchers must:

- Participate in research planning.
- Validate each other's significant findings.
- Maintain evidence provenance.
- Review all high-severity claims.
- Confirm the final report contains no secrets or personal data.
- Approve the final publication version.

Neither researcher should independently approve their own high-severity finding for publication.

---

## 4. Investigation Modules

The investigation contains seven practical modules.

### Module 01 — Organization & Public Identity Research

**Lead:** Researcher A  
**Support:** Researcher B

Investigate the organization's publicly disclosed identity and online presence.

**Research tasks:**

1. Identify the official website.
2. Identify the verified public social media profiles.
3. Identify official public GitHub repositories.
4. Record public contact channels.
5. Identify relevant brands and project names.
6. Establish which discovered properties are actually associated with the target.

**Questions to answer:**

- What digital channels does the organization operate?
- Which online profiles are confirmed as official?
- Is the public identity consistent across platforms?
- Are obsolete or duplicate channels still visible?

**Evidence:** Official links, public profile references, publication dates, screenshots, and URLs.

### Module 02 — Domain & DNS Footprint

**Lead:** Researcher A  
**Reviewer:** Researcher B

Investigate public DNS records and registration metadata.

**Research tasks:**

1. Retrieve available RDAP registration information.
2. Inspect DNS A and AAAA records.
3. Identify MX records.
4. Identify nameservers.
5. Review publicly visible TXT records, including SPF and DMARC where applicable.
6. Search public certificate transparency records.
7. Identify historical subdomain names from certificate data.
8. Distinguish current DNS observations from historical records.

**Questions to answer:**

- Which internet-facing assets can be associated with the authorized domain?
- Which services can be inferred from published DNS records?
- What historical hostnames appear in certificate records?
- Are there potential configuration concerns requiring owner verification?

**Important:** A hostname appearing in a certificate log is not proof that the host is still active. A missing DNS record or security policy must be interpreted in context, not automatically labeled a vulnerability.

### Module 03 — Public Website Information Exposure

**Lead:** Researcher B  
**Reviewer:** Researcher A

Review information intentionally or unintentionally disclosed by the authorized public website.

**Research tasks:**

1. Review accessible informational pages.
2. Examine publicly linked documents and resources.
3. Identify unnecessary technical details disclosed in page content.
4. Review public contact information for excess disclosure.
5. Check whether outdated public pages remain indexed.
6. Review security headers only on specifically authorized sites.
7. Document observed information that might support unwanted reconnaissance.

**Questions to answer:**

- Does the website unnecessarily expose sensitive operational details?
- Are old public documents still accessible?
- Is published configuration information appropriate for public access?
- Can findings be reduced without disrupting legitimate operations?

**Evidence:** Page title, URL, observation date, relevant excerpt, redacted screenshot, and risk explanation.

### Module 04 — Public Code Repository Exposure

**Lead:** Researcher A  
**Reviewer:** Researcher B

Review the team's or organization's explicitly authorized public repositories.

**Research tasks:**

1. Inventory public repositories.
2. Inspect README files and public documentation.
3. Identify published configuration examples.
4. Review whether sample environment files contain realistic values.
5. Check for unnecessary infrastructure descriptions.
6. Document public references to inactive applications or services.

**Questions to answer:**

- What infrastructure or technology information is published?
- Is any configuration information more detailed than intended?
- Do public repositories reveal unnecessary internal architecture?
- Are demonstration values distinguishable from real credentials?

Do not verify suspected exposed credentials against services. If a genuine secret is encountered, minimize access, record only safe metadata, and use the authorized reporting channel.

### Module 05 — Historical Digital Footprint

**Lead:** Researcher A  
**Reviewer:** Researcher B

Use public archives to identify changes in the organization's online presence.

**Research tasks:**

1. Search archived website versions.
2. Identify historical page titles and URLs.
3. Compare old and current public contact information.
4. Identify obsolete project references.
5. Record public changes in site structure.
6. Correlate historical observations with the current asset inventory.

**Questions to answer:**

- What information remains discoverable in historical archives?
- Are obsolete assets still referenced publicly?
- Do public records indicate changes in online infrastructure?

**Evidence:** Archive URL, capture date, description of observed change, and verification status.

### Module 06 — Exposure Verification & Risk Assessment

**Lead:** Researcher B  
**Reviewer:** Researcher A

Evaluate the security significance of findings.

Every observation should be assigned one of these statuses:

- **Verified finding:** Supported by direct, reproducible evidence.
- **Potential concern:** Plausible but needs additional confirmation.
- **Informational:** Useful contextual information without established security impact.
- **Not substantiated:** Insufficient or conflicting evidence.
- **Out of scope:** Outside the authorized research boundary.

Assess plausible consequences for:

- Confidentiality.
- Integrity.
- Availability.
- Privacy.
- Organizational reputation.
- Facilitation of further reconnaissance.

Avoid stating that a system is vulnerable solely because it appears in DNS, certificate logs, an archive, or a search result.

### Module 07 — Recommendations & Final Assessment

**Lead:** Researcher B  
**Reviewer:** Researcher A

Translate confirmed observations into practical action.

For each verified finding:

1. Describe the observed condition.
2. Identify the affected asset.
3. Explain the plausible risk.
4. Define an appropriate corrective action.
5. Assign a suggested priority.
6. Describe a nonintrusive method of validating the fix.

Recommendations should be specific, feasible, and linked directly to evidence.

---

## 5. Free Research Tools and Resources

| Resource | Purpose | Cost |
|---|---|---|
| Google / Bing | Public indexing and asset discovery | Free |
| ICANN Lookup / RDAP | Domain registration information | Free |
| `dig` / `nslookup` | DNS records | Free |
| crt.sh | Certificate transparency searches | Free |
| Internet Archive Wayback Machine | Historical website content | Free |
| GitHub Code Search | Public code and configuration references | Free account |
| Google Safe Browsing | Public website safety signals | Free |
| Wireshark | Network analysis, optional for later projects | Free |
| draw.io | Infrastructure and relationship diagrams | Free |
| LibreOffice | Report and spreadsheet authoring | Free |
| Git / GitHub | Version control and team collaboration | Free tiers |
| Zotero | References and source management | Free |

**Optional:** Have I Been Pwned domain search, only for a domain whose control can be verified. Availability of free domain results depends on current service conditions and domain size.

A second optional resource is OWASP Amass for more advanced asset discovery. For this beginner project, manual passive research is sufficient. Any automation must remain within approved methods and scope.

### Practice Datasets

**Dataset A — Owned project**

The preferred dataset is the team's own website, domain, and public repositories.

**Dataset B — Synthetic company**

Create a fictional organization containing:

- One fictional domain name ending in `.invalid`.
- A synthetic DNS-record inventory.
- Five fictitious public assets.
- Three sample public documents.
- Two simulated repository descriptions.
- A handful of historical observations.
- Two or three deliberately introduced, non-sensitive exposure scenarios.

Use synthetic data only; do not register or scan the fictional `.invalid` domain.

**Dataset C — Published training material**

Use the OWASP Web Security Testing Guide, official documentation, and public educational examples to practice interpreting evidence. Clearly distinguish training observations from findings about real organizations.

---

## 6. Practical Research Techniques

### 6.1 Search Engine Queries

Replace `YOURDOMAIN` with an authorized domain.

- `site:YOURDOMAIN`
- `site:YOURDOMAIN filetype:pdf`
- `"YOURDOMAIN" "documentation"`
- `"YOURDOMAIN" "contact"`
- `"YOURDOMAIN" site:github.com`

Use the results to find public references. Search snippets may be stale, so findings require corroboration.

### 6.2 Basic DNS Commands

For a domain you are authorized to assess:

- `dig YOURDOMAIN A`
- `dig YOURDOMAIN AAAA`
- `dig YOURDOMAIN MX`
- `dig YOURDOMAIN NS`
- `dig YOURDOMAIN TXT`
- `dig _dmarc.YOURDOMAIN TXT`

Record the observation time and resolver, as results may vary. These queries provide configuration observations, not comprehensive assurance about email security.

### 6.3 Certificate Transparency

Visit `https://crt.sh/` and search for the approved domain.

Record:

- Certificate subject names.
- Relevant certificate dates.
- Potential subdomain names.
- Duplicate or historical entries.
- Whether a candidate hostname is independently corroborated.

### 6.4 Public Repository Review

Use GitHub's web interface to review authorized public repositories.

Focus on:

- Documentation.
- Readme files.
- Public configuration examples.
- Published environment templates.
- References to external services.
- Outdated architecture descriptions.

Do not copy suspected credentials into the report or public repository.

### 6.5 Historical Website Research

Visit `https://web.archive.org/` and search for the approved website.

Select several available snapshots and record:

- Capture dates.
- Relevant changes.
- Historical public assets.
- Whether those references appear current.

An archived page is historical evidence, not proof of a present-day exposure.

---

## 7. Evidence Collection Standard

Each significant observation must be reproducible or clearly described as a secondary-source claim.

### Evidence Register

| Field | Description |
|---|---|
| Evidence ID | Unique reference, e.g. EVD-001 |
| Finding ID | Related finding, if applicable |
| Asset | Affected domain, page, file, or repository |
| Source | URL, lookup source, or data file |
| Collected at | UTC date and time |
| Method | Query or inspection procedure |
| Observation | Exact relevant fact |
| Evidence file | Local screenshot or export path |
| SHA-256 | Hash of retained evidence file |
| Analyst | Researcher A or B |
| Reviewer | Other researcher |
| Confidence | High, Moderate, Low |
| Sensitivity | Public, Restricted, Sensitive |
| Limitations | Relevant caveats |

### Confidence Definitions

**High:** Supported by direct observation and reliable corroboration.

**Moderate:** Credible supporting evidence exists, but an important detail remains uncertain.

**Low:** A preliminary indication requiring further confirmation.

### Evidence Handling Rules

- Preserve original source URLs.
- Record collection times in UTC.
- Save only material needed to support the conclusion.
- Do not alter the retained original evidence.
- Calculate SHA-256 hashes for retained evidence files.
- Redact personal or sensitive data in publication copies.
- Reference the exact evidence ID in every material finding.
- Document conflicting sources.
- Avoid retaining real passwords, tokens, or unnecessary personal data.
- Maintain a clear separation between internal evidence and public artifacts.

SHA-256 helps detect evidence file changes; it does not independently establish where the evidence came from or that a claim is true.

---

## 8. Risk Assessment Methodology

Use a simple **4 × 4 qualitative risk matrix** for teaching purposes. This is a project-specific scoring method, not an official CVSS or NIST scoring system.

### Likelihood

1 — Unlikely under the documented conditions  
2 — Possible  
3 — Likely  
4 — Highly likely

### Impact

1 — Minimal  
2 — Limited  
3 — Significant  
4 — Severe

**Risk score = Likelihood × Impact**

| Score | Risk level |
|---|---|
| 1–3 | Low |
| 4–6 | Moderate |
| 8–9 | High |
| 12–16 | Critical |

Scores must be justified. Where likelihood cannot be reasonably estimated from passive evidence, use **Not Rated** and explain the missing information instead of inventing a score.

### Finding Template

**Finding ID:** F-001  
**Title:** Short descriptive finding name  
**Affected asset:** Relevant authorized asset  
**Observation:** What was actually identified  
**Evidence:** EVD-001, EVD-002  
**Security relevance:** Why the observation matters  
**Impact:** What might happen under specified conditions  
**Likelihood:** Justified rating or Not Rated  
**Overall risk:** Provisional or confirmed rating  
**Confidence:** High / Moderate / Low  
**Recommendation:** Concrete corrective action  
**Verification method:** How the owner can verify remediation  
**Status:** Open / Accepted / Resolved / Informational

### Illustrative Training Example

**Finding:** An obsolete public project page remains indexed.

**Evidence:** A public search result and a matching authorized website page.

**Observation:** The page references an application that the owner confirms is retired.

**Potential risk:** Unnecessary disclosure of historical project information.

**Recommendation:** Review whether the page should remain public and whether search indexing should be updated.

**Confidence:** High for the page's existence; security impact remains context-dependent.

This is a fictional example, not a finding about any real organization.

---

## 9. Full Report Outline

**Recommended length: 15–25 pages**, excluding extensive evidence attachments.

### Cover Page
Project title, authors, date, version, authorized target, and distribution marking.

### 1. Executive Summary (1 page)
Purpose, scope, key confirmed observations, overall assessment, and top recommendations.

### 2. Introduction (1 page)
Background, objectives, and research questions.

### 3. Scope & Limitations (1 page)
Authorized assets, methodologies, exclusions, and constraints.

### 4. Methodology (1–2 pages)
Research process, tools, evidence requirements, confidence levels, and validation.

### 5. Target Digital Footprint Overview (1–2 pages)
Observed web presence, domain relationships, repositories, and public channels.

### 6. DNS & Infrastructure Findings (2 pages)
Relevant DNS records, registration observations, certificates, and historical domains.

### 7. Website & Public Information Findings (2 pages)
Publicly visible information, documents, archived pages, and relevant disclosures.

### 8. Public Repository Findings (1–2 pages)
Published configuration references, documentation, and information exposure concerns.

### 9. Risk Assessment (2 pages)
Risk matrix, verified findings, confidence, and limitations.

### 10. Recommendations (1–2 pages)
Prioritized remediation measures and owner verification actions.

### 11. Conclusions (1 page)
Answers to research questions and overall assessment.

### 12. References (1 page)
All significant public sources and methodology references.

### Appendices
Evidence index, additional screenshots, research queries, asset inventory, and diagrams.

**Report writing rule:** The executive summary must be understandable to a nontechnical reader, while the technical sections should let another researcher reproduce the important observations.

---

## 10. Ten-Day Research Timeline

| Day | Researcher A | Researcher B | Milestone |
|---|---|---|---|
| 1 | Scope, target ownership, asset list | Scope review, risk criteria | Approved project scope |
| 2 | Public identity research | Source reliability research | Initial source register |
| 3 | DNS and RDAP review | Website content review | First evidence batch |
| 4 | Certificate transparency | Document exposure review | Infrastructure inventory |
| 5 | Public repository review | Exposure screening | Midpoint review |
| 6 | Historical archives | Validate potential findings | Updated evidence register |
| 7 | Asset diagram | Risk register and ratings | Findings review |
| 8 | Draft methodology and technical sections | Draft findings and recommendations | Draft report |
| 9 | Review risk claims and evidence | Compile and edit report | QA candidate |
| 10 | Final evidence audit | Publication redaction and formatting | Final deliverables |

**Daily working rhythm:**

- 10–15 minutes: Agree on tasks and blockers.
- 60–90 minutes: Individual assigned research.
- 20–30 minutes: Joint review and evidence synchronization.
- 10 minutes: Record progress and next actions.

**Midpoint gate (Day 5):** The team should have a usable asset inventory and source register. If evidence is sparse, narrow the research questions instead of inventing findings.

**Final gate (Day 10):** Every material claim must have evidence, and the public report must pass the sensitive-information review.

---

## 11. Collaboration & Project Organization

### Suggested GitHub Repository

**Repository:** `digital-footprint-assessment`

Recommended structure:

- `README.md` — Project overview and research scope.
- `docs/` — Methodology, scope, report outline, and contributor guidelines.
- `research/researcher-a/` — OSINT and asset discovery notes.
- `research/researcher-b/` — Exposure and risk analysis notes.
- `data/` — Synthetic or sanitized working datasets.
- `evidence/` — Evidence index and redacted publication-safe materials only.
- `findings/` — Approved finding records.
- `diagrams/` — Asset relationships and research workflow.
- `reports/` — Drafts and final public report.
- `references/` — Source bibliography.
- `templates/` — Evidence, finding, and risk templates.

**Important:** Use a private repository for internal research. Publish only a separate sanitized portfolio version. Do not put unredacted private evidence into Git history.

### Task Tracking

Create GitHub Issues for each research module.

Suggested labels:

- `research`
- `osint`
- `dns`
- `evidence`
- `finding`
- `validation`
- `report`
- `quality-assurance`
- `completed`

Each issue should include a clear objective, assigned researcher, expected deliverable, and completion criteria.

### Collaboration Rules

1. Assign one primary owner and one reviewer to each task.
2. Maintain one canonical evidence register.
3. Use separate branches for substantial report changes.
4. Review findings before merging them.
5. Keep internal and public evidence separate.
6. Record unresolved questions rather than hiding them.
7. Require both researchers to approve the publication release.

---

## 12. Final Deliverables

### Deliverable A — Technical Research Report

**Suggested filename:** `DFRA-2026-009_Technical_Report.pdf`

A complete report containing the assessment methodology, technical observations, validated findings, and mitigation recommendations.

### Deliverable B — Executive Brief

**Suggested filename:** `DFRA-2026-009_Executive_Brief.pdf`

A 1–2 page nontechnical summary with the main conclusions and recommended priorities.

### Deliverable C — Asset Inventory

**Suggested filename:** `asset_inventory.csv`

A structured inventory with asset type, identifier, source, observation time, validation status, and relevant notes.

### Deliverable D — Evidence Register

**Suggested filename:** `evidence_register.csv`

A structured index of collected evidence with supporting references and review status.

### Deliverable E — Risk Register

**Suggested filename:** `risk_register.csv`

A table containing verified findings, provisional ratings, affected assets, recommendations, and confidence.

### Deliverable F — Infrastructure Diagram

**Suggested filename:** `digital_footprint_map.png`

A diagram representing verified relationships among the assessed domain, public assets, and associated services.

### Deliverable G — Public GitHub Portfolio

Include:

- A clear README.
- The project's objectives.
- Both researchers' contributions.
- Research methodology.
- Sanitized diagrams.
- Public report.
- Key learning outcomes.
- Relevant links and references.

### Deliverable H — Lessons Learned

**Suggested filename:** `lessons_learned.md`

Each researcher should document:

- Three skills they improved.
- Two methodological difficulties.
- One important correction discovered during review.
- What they would change in a future investigation.

---

## 13. Quality Assurance Checklist

Before publishing, confirm:

- [ ] Research scope and authorization are documented.
- [ ] Both researchers completed their assigned work.
- [ ] The asset inventory distinguishes verified and unverified relationships.
- [ ] Historical information is not misrepresented as current.
- [ ] Every important observation has a source reference.
- [ ] Findings distinguish facts, hypotheses, and inferred risks.
- [ ] Risk ratings have documented explanations.
- [ ] Evidence records include collection dates.
- [ ] Relevant evidence integrity hashes are recorded.
- [ ] Significant findings received independent review.
- [ ] No real credentials or unnecessary personal data are included.
- [ ] Public materials are sanitized.
- [ ] All sources are attributed.
- [ ] Diagrams are accurate and readable.
- [ ] The report contains actionable conclusions.
- [ ] Both researchers approve the final version.

---

## 14. Project Success Criteria

The project is considered successfully completed when:

**Research quality**
- The authorized digital footprint has been systematically investigated.
- All available, relevant asset categories within scope have been considered.
- The evidence register supports the conclusions.
- Findings are reproducible or appropriately qualified.

**Technical skills**
- Both researchers can explain DNS, RDAP, certificate transparency, and public repository research.
- Both can distinguish public presence from actual vulnerability.
- Both understand basic evidence collection and risk assessment.

**Teamwork**
- Tasks are documented and balanced.
- Peer reviews are completed.
- Both members can explain the overall findings, not only their own sections.

**Portfolio quality**
- A complete professional report exists.
- A sanitized public version is available.
- The GitHub project explains the methodology and individual contributions.
- No unsupported security claims or sensitive information are published.

---

## 15. Official Methodology References

- OWASP Attack Surface Analysis — https://cheatsheetseries.owasp.org/cheatsheets/Attack_Surface_Analysis_Cheat_Sheet.html
- OWASP Web Security Testing Guide — https://owasp.org/www-project-web-security-testing-guide/
- NIST SP 800-115 — https://csrc.nist.gov/pubs/sp/800/115/final
- FIRST Traffic Light Protocol 2.0 — https://www.first.org/tlp/
- ICANN RDAP Lookup — https://lookup.icann.org/en
- Certificate Transparency Search — https://crt.sh/
- Internet Archive Wayback Machine — https://web.archive.org/
- GitHub Code Search documentation — https://docs.github.com/en/search-github/github-code-search/using-github-code-search
- Google Safe Browsing — https://safebrowsing.google.com/
- Have I Been Pwned — https://haveibeenpwned.com/

---

**End of Project Brief — DFRA-2026-009**

*This brief defines an educational external digital footprint assessment. It does not certify the security of an organization, and it does not substitute for a separately authorized penetration test or complete security audit.*
