<!--
Svast Healthcare Technologies - Pull Request
Fill in every section. Delete lines that do not apply, do not leave them blank.
Feature PRs target dev. Release PRs (dev/uat -> main) must link a CHG ticket.
-->

## Jira
<!-- Story/bug key, e.g. REVXL-231. Release PRs: CHG key, e.g. CHG-14 -->
Ticket:

## Type of PR
- [ ] Feature / bug fix -> `dev`
- [ ] Promotion -> `uat`
- [ ] Release -> `main` (CHG ticket required)
- [ ] Hotfix -> `main` (Emergency CHG ticket required)

## What changed and why
<!-- 2-5 lines. What does this change do, and which acceptance criteria does it meet? -->

## How it was tested
<!-- Environment (dev / uat), what you tested, link to the test cases on the Jira story -->

## Review checklist (author fills, reviewer verifies)
**Logic**
- [ ] Meets the acceptance criteria on the Jira story
- [ ] Edge cases handled (empty data, large data, invalid input)

**Security and PHI**
- [ ] No PHI, credentials, API keys or secrets in code, comments, logs or test data
- [ ] User input validated; database queries parameterised
- [ ] Authentication / authorization checks in place on new endpoints or screens
- [ ] No new PHI written to logs, error messages or analytics

**Data and infrastructure**
- [ ] DB migration included? If yes, it was reviewed and has a rollback
- [ ] New environment variables / secrets added to Secrets Manager (not committed)
- [ ] New third-party library? Licence and known vulnerabilities checked

**Testing**
- [ ] Tested in dev against the story's test cases, results recorded on the Jira story
- [ ] Existing features touched by this change re-checked (regression)

## Release PRs only (into `main`)
- [ ] CHG ticket linked, with impact, risk, PHI flag and rollback plan
- [ ] Every story in this release shows "UAT passed" from its manager
- [ ] High-risk change (PHI schema, IAM, network, data migration): deployment window agreed

## Screenshots / notes for the reviewer
