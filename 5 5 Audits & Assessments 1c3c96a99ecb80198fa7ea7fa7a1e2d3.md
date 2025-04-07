# 5.5 Audits & Assessments

Created time: 27 mars 2025 20:03
Last edited by: OLB_
Last edited time: 5 avril 2025 18:01

3 assessments:

- security tests
- security assessments
- security audits

## Security Tests

- verify a control is functioning properly
- automated tests, pentests, manual tests
- frequently made
- bug bounty (part of responsible disclosure program)

## Security assessments

- security tests + risk assessment
- threat environment evaluation
- produce a report with recommandations (non technical)

## Security audits

One of the primary outcomes of an audit is an **attestation** by the
auditor. This is a formal statement that the auditors have reviewed the
controls and found that they are both adequate to meet the control
objectives and working properly.

- same as security assessments but by independent auditors
- internal audit
    - independant internal staff
    - CAE (chief audit executive) report directly to CEO
    - for self assessment or compliance
- external audit
    - lead by third party (Ernst&Young, Deloitte, PWC, KPMG - the big 4)
- independent third party audits
    - on behalf of an other organization (law , contracts)
    - For an independent third-party audit, the request comes
    from a regulator, customer, or other outside entity.

Auditing Standards

- use of framework :
    - Control Objectives for Information and related Technologies (COBIT)
    - ISO27001 / 27002

Vulnerability lifecycle

- Identification (Scans, pentests, bug bounty, reports, audits …)
- Analysis (confirm, prioritizing and categorizing using CVE +  organization exposure factors + environment variables + org. risk tolerance)
- Response and remediation
    - patch
    - network segmentation
    - compensating controls
    - insurance
    - exception or exemption (risk acceptance)
- Validation of remediation
    - rescan
    - new audit
- Reporting
    - describe vuln.
    - describe remediation
    - recommendations