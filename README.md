# AIRMAC v1.1.0

Application released October 28, 2026. README updated October 29, 2026 to include the AIRMAC demonstration package. Implements the approved AIRMAC Assessment Method Specification Draft 0.1. The original AIRMAC v1.0.0 file is unchanged.



## Overview:

AIRMAC assesses the organization's ability to manage AI risk across every system it builds, buys or uses. It rates 33 practices mapped to all 19 NIST AI RMF GOVERN subcategories and the program-level MAP, MEASURE and MANAGE outcomes. Each practice is judged on whether it is designed and whether sampled systems show it working. A domain's maturity level cannot go above what that evidence supports.



\*\*AIRMAC — AI Risk Management Capability Assessment\*\*



AIRMAC is a browser-based assessment tool that helps organizations evaluate how effectively they govern and manage AI risk. It provides a repeatable, evidence-supported assessment of organizational capability and translates identified gaps into an actionable roadmap for leadership.



\*\*Purpose and Use\*\*



AIRMAC helps leaders and assessors answer three questions:



\- Are appropriate AI risk management practices established?

\- Does evidence show those practices operating across the organization’s AI systems?

\- What actions, resources, and decisions are needed to improve?



The tool supports internal assessments, program reviews, improvement planning, and leadership reporting. Intended users include AI governance teams, risk managers, assurance professionals, internal assessors, and accountable executives.



\*\*Assessment Capability\*\*



AIRMAC evaluates \*\*33 practices across eight domains\*\*: governance and accountability; risk appetite and decision criteria; AI inventory and lifecycle; people and human oversight; third-party and supply chain management; stakeholder engagement and transparency; testing, monitoring, and incident response; and program performance and improvement.



Assessors define the scope, establish an AI inventory, examine supporting evidence, and perform \*\*14 operating tests on selected systems\*\*. AIRMAC distinguishes documented design from demonstrated operation, identifies incomplete assessment work, and limits maturity ratings to the level supported by the evidence.



Its five-level capability scale ranges from \*\*Initial\*\* to \*\*Optimizing\*\*. Current and target domain ratings help leadership understand strengths, weaknesses, and improvement priorities. Portfolio risk indicators are reported separately from capability maturity.



\*\*Leadership Outputs\*\*



AIRMAC connects assessment conclusions to findings with accountable owners, severity, due dates, recommendations, resource needs, leadership decisions, and verification criteria. It produces:



\- A capability scorecard and current-to-target domain profile.

\- An evidence register and system-test results.

\- Prioritized findings and an improvement roadmap.

\- A standalone HTML report suitable for printing to PDF.

\- Inventory and findings CSV exports, plus portable assessment JSON.

\- Review and sign-off records, revision history, and preserved final assessment baselines.



AIRMAC operates as a standalone HTML application with browser storage and manual import/export. Assessment conclusions rely on qualified human judgment. Its practices map to NIST AI RMF 1.0 outcomes; its maturity scale and scoring rules are AIRMAC-defined. Results support organizational improvement and framework alignment, without establishing certification or regulatory compliance.

## 

## Start

1. Download AIRMAC-v1.1.0.html and open it in a current desktop browser.
2. The first opening shows the fictional Harborview example. It intentionally contains incomplete assessment work and is not ready for finalization.
3. Choose Method \& files → Start a new assessment, or Import JSON to bring in exported v1.0 or v1.1 assessment data.
4. Set the current editor identity in Scope. Define coverage and limitations, then complete the inventory, test plan, observations, practice conclusions, targets and findings.
5. Complete lead sign-off, reviewer approval and sponsor disposition under Report \& sign-off. Resolve readiness items before marking Final.
6. Export assessment JSON regularly, especially after finalization. Download the standalone HTML report for leadership and print that report to PDF when needed.

Work is saved in this browser. A separate v1.1 storage key avoids overwriting v1.0 browser data. Moving the HTML file may change the browser's local-file storage behavior. JSON is the portable backup and transfer format.

## Demonstration package

`AIRMAC\_Demonstration\_Package.zip` provides a guided, fictional assessment of **Coastal Engineering Services — Engineering Operations**. Use it to learn how evidence and sample observations support practice ratings, domain maturity, findings and a leadership roadmap.

The demonstration package is separate from `AIRMAC-v1.1.0-release.zip`. It contains training materials and importable assessment data; it does **not** include the HTML application or automated test suite. Use the existing `AIRMAC-v1.1.0.html` application.

### Package contents

|File|Purpose|
|-|-|
|`AIRMAC\_Demonstration\_Use\_Case.docx`|Ten-page guide covering scope, inventory, evidence, all 14 tests, all 33 practices, maturity, findings, review, exports and baseline preservation.|
|`AIRMAC\_Demo\_Starter.json`|Hands-on starting point with scope, inventory, evidence metadata, eligibility and proposed test criteria prefilled. Results, ratings, findings, target agreement and sign-off remain unfinished.|
|`AIRMAC\_Demo\_Worked\_Assessment.json`|Worked assessment with test results, evidence links, ratings, target agreement, findings and executive summary completed. Lead sign-off and reviewer approval remain for the demonstration.|
|`AIRMAC\_Demo\_Evidence.md`|Nineteen synthetic evidence packages referenced by the assessment files, including system-specific test observations.|
|`START\_HERE.txt`|Quick setup instructions and expected outcomes.|

### Quick demonstration

Allow approximately 15–25 minutes.

1. Download and extract `AIRMAC\_Demonstration\_Package.zip`.
2. Open your downloaded `AIRMAC-v1.1.0.html` application in a desktop browser.
3. **Export existing assessment JSON before importing.** Import replaces the current working assessment in that browser.
4. Select **Method \& files → Import JSON**, choose `AIRMAC\_Demo\_Worked\_Assessment.json`, and confirm **Import**.
5. Confirm the organization is **TRAINING ONLY Coastal Engineering Services**. Do not choose **Load the fictional example**; that loads the different, built-in Harborview scenario.
6. Review **Overview**, then inspect **Sample tests**: S-01/T5 fails because residual risk was accepted outside delegated authority; S-02/T10 fails because monitoring has no assigned reviewer. S-03/T8 is N/A because the fictional in-house system has no third-party AI components.
7. Review the two linked findings in **Findings \& roadmap**, then the scorecard, executive summary and readiness items in **Report \& sign-off**.
8. Follow page 8 of the guide to record demonstration lead sign-off, reviewer identity/date and independence statement. Leave sponsor disposition **Pending**, or complete the required fields if demonstrating **Accepted**. Select reviewer approval **last**; substantive edits clear it.
9. Resolve all readiness items, select **Mark as final**, and export the assessment JSON and full HTML report. Open the downloaded report to print or save it as PDF.
10. In **Method \& files**, inspect the preserved Final revision 1 baseline. After exporting a backup, edit a commitment to demonstrate return to Draft revision 2 with reviewer approval cleared and revision 1 retained.

### Hands-on practice

Allow approximately 60–90 minutes. Import `AIRMAC\_Demo\_Starter.json` instead of the worked file, then follow pages 2–8 of the guide. Keep `AIRMAC\_Demo\_Evidence.md` open alongside the application. The practice maps on pages 9–10 identify the design evidence, operating evidence and expected operating conclusion for every practice.

Record the fictional historical test-plan approval before entering the dated observations. Complete each test's eligibility, result, assessor, date, evidence and explanation; a result dropdown alone is insufficient. Complete both design and operating evidence-sufficiency explanations for each practice. Export JSON checkpoints between major stages.

Some edits redraw the screen and collapse expanded sections. Reopen the same section and continue; completed entries are retained. If comparing your work with the worked file, export your practice assessment before importing the comparison.

### Expected worked results

|Checkpoint|Expected result|
|-|-|
|Inventory and sample|3 operating systems; all 3 sampled; 1 high-impact.|
|Test entries|42 results: 39 Pass, 2 Fail, 1 N/A.|
|T5 residual risk acceptance|Not operating: the high-impact authorization failure overrides the 2-of-3 pass rate.|
|T10 monitoring|Inconsistent: 2 of 3 systems pass.|
|T8 third-party due diligence|Effective: both applicable systems pass; S-03 is excluded with an explanation.|
|Practices|33 assessed; 31 Meets; 2 gaps: RSK-4 and MON-2.|
|Domains|Risk Appetite \& Decision Criteria is level 2; the other seven domains are level 3.|
|Overall capability|Current 3 Defined; target 4 Managed.|
|Findings|2 Open findings with owners, November 27, 2026 due dates and verification criteria.|
|Readiness on initial worked-file import|Two messages remain: lead sign-off and reviewer approval.|

An assessment can be Final while findings remain Open. Finalization establishes a complete, reviewed assessment; it does not establish that all corrective actions are finished. A higher target does not raise the current evidence ceiling.

### Training boundaries and validation

All organizations, people, approvals, dates and evidence are fictional. The package demonstrates tool operation and assessment reasoning, not assurance for real systems. The evidence file is supplied training content, not a real repository. Use the historical dates only for this fictional record-entry exercise; do not backdate real assessment work or imply that an actual independent review occurred.

Both demonstration JSON files passed the v1.1.0 import normalizer. The worked case produced the expected overall score, target, practice statuses and two gaps; adding valid demonstration sign-off satisfied readiness. Visual browser click-through remains unverified in the test environment. The package does not modify the application file.

## Main changes

* Separate design and operating evidence links, sufficiency judgments and confidence explanations. Blank or incomplete evidence records cannot support conclusions.
* “Operation not verified” replaces misleading Meets status for untested or insufficiently supported operation.
* Test-level eligibility, observations, evidence, assessor and date; population eligibility is editable for unsampled systems as well.
* Pending observations and incomplete observation records prevent Effective conclusions. Approved genuine observation limitations can be finalized with an owned follow-up and a ceiling of 2.
* Documented sampling coverage, deviations and review. A one-system eligible population can support operation with its limited coverage disclosed.
* Critical high-impact authorization and risk-acceptance failures override the pass rate. For T6/T14 failures, assessors classify whether a required stop or override capability is unavailable; that classification triggers the critical override. Other deficiencies use the ordinary aggregation rule.
* Excluded domains have no numeric level. A comparable overall score requires all eight applicable, completed domains within their evidence ceilings. Overall uses the lower median, capped at one above the weakest domain.
* Sponsor agreement on targets; reviewer identity, date, independence statement and approval before finalization. Substantive changes invalidate review approval.
* Finding due dates, affected practices and systems, evidence, severity rationale, safeguards, dependencies, resources, decisions, closure criteria and verification.
* Risk acceptance authority, rationale, conditions, review and expiry. Closed findings cannot hide continuing gaps without reviewed disposition.
* Assessment IDs, method version, revisions, field-change history and preserved final snapshots. A substantive edit after Final starts a Draft revision; baseline JSON and reports remain downloadable under Method \& files.
* Schema 2 import validation with v1.0 migration. Invalid ratings, malformed dates, negative risk counts, duplicate IDs and broken links are rejected. Legacy v1.0 sign-off details are retained, while the working assessment becomes Draft for the new method requirements.
* Full standalone report includes evidence traceability, test plan and observations, limitations, roadmap commitments, review and change history. Inventory and findings CSV exports include the new fields.
* Portfolio recency is anchored to the reporting date; unknown history is separated from explicitly reported Never assessed. Conditional operation counts only systems in the Operation stage.
* Removed external font loading. No server or AI API is required. Reference links open only when selected.

## Method and reference scope

The 33 practices and eight domains remain the organizational assessment baseline. Maturity levels and decision thresholds are AIRMAC rules. The assessment does not constitute certification, a complete NIST AI RMF Profile, or an exhaustive federal compliance review.

Selected mappings and federal tags were reviewed against these primary sources:

* NIST AI RMF 1.0 Core: https://airc.nist.gov/airmf-resources/airmf/5-sec-core/
* OMB M-25-21: https://www.whitehouse.gov/wp-content/uploads/2025/02/M-25-21-Accelerating-Federal-Use-of-AI-through-Innovation-Governance-and-Public-Trust.pdf
* OMB M-25-22: https://www.whitehouse.gov/wp-content/uploads/2025/02/M-25-22-Driving-Efficient-Acquisition-of-Artificial-Intelligence-in-Government.pdf

Mapping refinements add MANAGE 1.3 to residual risk acceptance and MAP 5.2 to stakeholder engagement and feedback practices. STK-4 disclosure retains GOVERN 1.4 rather than treating MAP 5.2 as a disclosure-specific outcome. Federal tags remain selected references; users must establish their own applicability and current obligations.

## Verification

* 44 automated method, regression, migration, export and report checks passed.
* All ten screens and a populated finding-detail form were generated and inspected programmatically: 614 field bindings checked, with no duplicate IDs, broken labels or unresolved data bindings.
* Acceptance checks cover A01–A07, including incomplete samples, all-N/A domains, blank evidence, small populations, critical overrides, continuing gaps, imported Final data and baseline preservation.
* Additional checks cover evidence sufficiency, reviewer invalidation, approved observation limitations, import validation, reporting-date posture, CSV fields and escaped report content. Imported baseline HTML is regenerated from validated assessment data.
* Visual browser QA and a real click-through/download session were not completed. The environment had no installed browser, and browser downloads failed. Template generation and simulated application actions were tested; visual behavior and browser-specific local storage/download behavior remain to be confirmed in a desktop browser.

## Reproduce automated checks

`AIRMAC-v1.1.0-release.zip` includes the application, the original release notes and the test suite. The separate `AIRMAC\_Demonstration\_Package.zip` contains the training materials listed above. This README update does not rebuild either ZIP.

Run from the extracted release folder:

```bash
node tests/verify.cjs
python3 tests/verify\_structure.py
```

The Node suite uses standard Node modules. The optional structure check requires Python's lxml package and reads the generated surfaces from the first command. Test output goes to tests/generated.

## Operational boundaries

Identity, reviewer approval and sign-off are self-declared. This standalone application does not provide authenticated users, cryptographic signatures, a tamper-evident audit log, shared concurrent editing, or a server evidence repository. Evidence remains a register of retrievable references; final snapshots are locally preserved copies. Export final baselines into the organization's records process.

