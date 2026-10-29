# AIRMAC v1.1.0

Released October 28, 2026. Implements the AIRMAC Assessment Method Specification Draft 0.1 approved for implementation in this conversation. The original AIRMAC v1.0.0 file is unchanged.

## Start

1. Download AIRMAC-v1.1.0.html and open it in a current desktop browser.
2. The first opening shows the fictional Harborview example. It intentionally contains incomplete assessment work and is not ready for finalization.
3. Choose Method & files → Start a new assessment, or Import JSON to bring in exported v1.0 or v1.1 assessment data.
4. Set the current editor identity in Scope. Define coverage and limitations, then complete the inventory, test plan, observations, practice conclusions, targets and findings.
5. Complete lead sign-off, reviewer approval and sponsor disposition under Report & sign-off. Resolve readiness items before marking Final.
6. Export assessment JSON regularly, especially after finalization. Download the standalone HTML report for leadership and print that report to PDF when needed.

Work is saved in this browser. A separate v1.1 storage key avoids overwriting v1.0 browser data. Moving the HTML file may change the browser's local-file storage behavior. JSON is the portable backup and transfer format.

## Main changes

- Separate design and operating evidence links, sufficiency judgments and confidence explanations. Blank or incomplete evidence records cannot support conclusions.
- “Operation not verified” replaces misleading Meets status for untested or insufficiently supported operation.
- Test-level eligibility, observations, evidence, assessor and date; population eligibility is editable for unsampled systems as well.
- Pending observations and incomplete observation records prevent Effective conclusions. Approved genuine observation limitations can be finalized with an owned follow-up and a ceiling of 2.
- Documented sampling coverage, deviations and review. A one-system eligible population can support operation with its limited coverage disclosed.
- Critical high-impact authorization and risk-acceptance failures override the pass rate. For T6/T14 failures, assessors classify whether a required stop or override capability is unavailable; that classification triggers the critical override. Other deficiencies use the ordinary aggregation rule.
- Excluded domains have no numeric level. A comparable overall score requires all eight applicable, completed domains within their evidence ceilings. Overall uses the lower median, capped at one above the weakest domain.
- Sponsor agreement on targets; reviewer identity, date, independence statement and approval before finalization. Substantive changes invalidate review approval.
- Finding due dates, affected practices and systems, evidence, severity rationale, safeguards, dependencies, resources, decisions, closure criteria and verification.
- Risk acceptance authority, rationale, conditions, review and expiry. Closed findings cannot hide continuing gaps without reviewed disposition.
- Assessment IDs, method version, revisions, field-change history and preserved final snapshots. A substantive edit after Final starts a Draft revision; baseline JSON and reports remain downloadable under Method & files.
- Schema 2 import validation with v1.0 migration. Invalid ratings, malformed dates, negative risk counts, duplicate IDs and broken links are rejected. Legacy v1.0 sign-off details are retained, while the working assessment becomes Draft for the new method requirements.
- Full standalone report includes evidence traceability, test plan and observations, limitations, roadmap commitments, review and change history. Inventory and findings CSV exports include the new fields.
- Portfolio recency is anchored to the reporting date; unknown history is separated from explicitly reported Never assessed. Conditional operation counts only systems in the Operation stage.
- Removed external font loading. No server or AI API is required. Reference links open only when selected.

## Method and reference scope

The 33 practices and eight domains remain the organizational assessment baseline. Maturity levels and decision thresholds are AIRMAC rules. The assessment does not constitute certification, a complete NIST AI RMF Profile, or an exhaustive federal compliance review.

Selected mappings and federal tags were reviewed against these primary sources:

- NIST AI RMF 1.0 Core: https://airc.nist.gov/airmf-resources/airmf/5-sec-core/
- OMB M-25-21: https://www.whitehouse.gov/wp-content/uploads/2025/02/M-25-21-Accelerating-Federal-Use-of-AI-through-Innovation-Governance-and-Public-Trust.pdf
- OMB M-25-22: https://www.whitehouse.gov/wp-content/uploads/2025/02/M-25-22-Driving-Efficient-Acquisition-of-Artificial-Intelligence-in-Government.pdf

Mapping refinements add MANAGE 1.3 to residual risk acceptance and MAP 5.2 to stakeholder engagement and feedback practices. STK-4 disclosure retains GOVERN 1.4 rather than treating MAP 5.2 as a disclosure-specific outcome. Federal tags remain selected references; users must establish their own applicability and current obligations.

## Verification

- 44 automated method, regression, migration, export and report checks passed.
- All ten screens and a populated finding-detail form were generated and inspected programmatically: 614 field bindings checked, with no duplicate IDs, broken labels or unresolved data bindings.
- Acceptance checks cover A01–A07, including incomplete samples, all-N/A domains, blank evidence, small populations, critical overrides, continuing gaps, imported Final data and baseline preservation.
- Additional checks cover evidence sufficiency, reviewer invalidation, approved observation limitations, import validation, reporting-date posture, CSV fields and escaped report content. Imported baseline HTML is regenerated from validated assessment data.
- Visual browser QA and a real click-through/download session were not completed. The environment had no installed browser, and browser downloads failed. Template generation and simulated application actions were tested; visual behavior and browser-specific local storage/download behavior remain to be confirmed in a desktop browser.

## Reproduce automated checks

The release ZIP includes the application, these notes and the test suite.

Run from the extracted release folder:

```bash
node tests/verify.cjs
python3 tests/verify_structure.py
```

The Node suite uses standard Node modules. The optional structure check requires Python's lxml package and reads the generated surfaces from the first command. Test output goes to tests/generated.

## Operational boundaries

Identity, reviewer approval and sign-off are self-declared. This standalone application does not provide authenticated users, cryptographic signatures, a tamper-evident audit log, shared concurrent editing, or a server evidence repository. Evidence remains a register of retrievable references; final snapshots are locally preserved copies. Export final baselines into the organization's records process.
