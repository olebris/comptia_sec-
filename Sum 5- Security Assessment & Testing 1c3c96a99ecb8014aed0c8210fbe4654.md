# Sum: 5- Security Assessment & Testing

Created time: 27 mars 2025 21:27
Last edited by: OLB_
Last edited time: 27 mars 2025 22:00

<aside>
👉

Security assessment and testing plays a crucial role in the ongoing
management of a cybersecurity program. The techniques discussed in
this chapter help cybersecurity professionals maintain effective
security controls and stay abreast of changes in their environment that
might alter their security posture.
Vulnerability scanning identifies potential security issues in systems,
applications, and devices, providing teams with the ability to
remediate those issues before they are exploited by attackers. The
vulnerabilities that may be detected during these scans include
improper patch management, weak configurations, default accounts,
and the use of insecure protocols and ciphers.
Penetration testing puts security professionals in the role of attackers
and asks them to conduct offensive operations against their targets in
an effort to discover security issues. The results of penetration tests
provide a roadmap for improving security controls.

**Many vulnerabilities exist in modern computing**
environments. Cybersecurity professionals should remain aware of
the risks posed by vulnerabilities both on-premises and in the cloud.
Improper or weak patch management can be the source of many of
these vulnerabilities, providing attackers with a path to exploit
operating systems, applications, and firmware. Weak configuration
settings that create vulnerabilities include open permissions,
unsecured root accounts, errors, weak encryption settings, insecure
protocol use, default settings, and open ports and services. When a
scan detects a vulnerability that does not exist, the report is known as
a false positive. When a scan does not detect a vulnerability that
actually exists, the report is known as a false negative.

**Threat hunting discovers existing compromises.** Threat
hunting activities presume that an organization is already
compromised and search for indicators of those compromises. Threat
hunting efforts include the use of advisories, bulletins, and threat
intelligence feeds in an intelligence fusion program. They search for
signs that attackers gained initial access to a network and then
conducted maneuver activities on that network.

**Vulnerability scans probe systems, applications, and devices
for known security issues.** Vulnerability scans leverage
application, network, and web application testing to check for known
issues. These scans may be conducted in a credentialed or
noncredentialed fashion and may be intrusive or nonintrusive,
depending on the organization's needs. Analysts reviewing scans
should also review logs and configurations for additional context.
Vulnerabilities are described consistently using the Common
Vulnerabilities and Exposures (CVE) standard and are rated using the
Common Vulnerability Scoring System (CVSS). CVE and CVSS are
components of the Security Content Automation Protocol (SCAP).

**Penetration testing places security professionals in the role
of attackers.** Penetration tests may be conducted in a manner that
provides the testers with full access to information before the test
(known environment), no information at all (unknown environment),
or somewhere in between those two extremes (partially known
environment). Testers conduct tests within the rules of engagement
and normally begin with reconnaissance efforts, including war driving,
war flying, footprinting, and open source intelligence (OSINT). They
use this information to gain initial access to a system. From there, they
seek to conduct privilege escalation to increase their level of access
and lateral movement/pivoting to expand their access to other
systems. They seek to achieve persistence to allow continued access
after the vulnerability they initially exploited is patched. At the
conclusion of the test, they conduct cleanup activities to restore
systems to normal working order and remove traces of their activity.

**Bug bounty programs incentivize vulnerability reporting.**
Bug bounty programs allow external security professionals to probe
the security of an organization's public-facing systems. Testers who
discover vulnerabilities are provided with financial rewards for their
participation. This approach is a good way to motivate hackers to work
for good, rather than using discovered vulnerabilities against a target.

**Recognize the purpose and types of security audits.** Audits are
formal examinations of an organization's security controls. They may
be performed by internal audit teams or independent third-party
auditors. At the conclusion of an audit, the audit team makes an
attestation about the adequacy and effectiveness of the organization's
security controls.

**Understand the stages of the vulnerability life cycle.** The
stages of the vulnerability life cycle are vulnerability identification,
analysis, response and remediation, validation of remediation, and
reporting. Vulnerability identification can come from scans,
penetration tests, responsible disclosure or bug bounty programs, and
audit results. Analysis involves confirming the vulnerability,
prioritizing it using CVSS and CVE, and considering organization-
specific factors. Responses include applying patches, isolating affected
systems, implementing compensating controls, transferring risk
through insurance, or formally accepting the risk. Validation ensures
the vulnerability is no longer present, and reporting informs
stakeholders about the findings, actions, trends, and
recommendations for improvement

</aside>

## CHECK EXAM

THE COMPTIA SECURITY+ EXAM OBJECTIVES
COVERED IN THIS CHAPTER INCLUDE:
Domain 4.0: Security Operations

4.3. Explain various activities associated with vulnerability
management.

- Identification methods (Vulnerability scan, Penetration
testing, Responsible disclosure program, Bug bounty
program, System/process audit)
- Analysis (Confirmation, Prioritize, Common
Vulnerability Scoring System (CVSS), Common
Vulnerabilities and Exposures (CVE), Vulnerability
classification, Exposure factor, Environmental
variables, Industry/organizational impact, Risk
tolerance)
- Vulnerability response and remediation (Patching,
Insurance, Segmentation, Compensating controls,
Exceptions and exemptions)
- Validation of remediation (Rescanning, Audit,
Verification)
- Reporting

4.4. Explain security alerting and monitoring concepts and
tools.

- Tools (Security Content Automation Protocol (SCAP),
Vulnerability scanners)

4.8. Explain appropriate incident response activities.

- Threat hunting

Domain 5.0: Security Program Management and
Oversight

5.3. Explain processes associated with third-party risk
assessment and management.

- Rules of engagement

5.5. Explain types and purposes of audits and assessments.

- Attestation
- Internal (Compliance, Audit committee, Self-
assessments)
- External (Regulatory, Examinations, Assessment,
Independent third-party audit)
- Penetration testing (Physical, Offensive, Defensive,
Integrated, Known environment, Partially known
environment, Unknown environment, Reconnaissance,
Passive, Active)