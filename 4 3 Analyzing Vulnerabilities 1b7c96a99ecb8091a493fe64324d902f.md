# 4.3 Analyzing Vulnerabilities

Created time: 15 mars 2025 15:26
Last edited by: OLB_
Last edited time: 27 mars 2025 21:12

- Update Signatures to avoid
    - false positive (annoying)
    - false negative (more dangerous)
- Prioritize Vulnerabilities
    - use CVSS for that
- CVSS 3.1 is a component of SCAP (Security Content Protocol)

```bash
#CVSS Vector
CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:N/A:N
```

- AV : Attack vector
    - P Physical / L Local / A Adjacent (LAN)  / N Network
- AC: Attack Complexity
    - H High / L Low
- PR: Privileges Required
    - H High / L Low / N None
- UI : User Interaction (user other than attacker)
    - N None / R Required
- C Confidentiality
    - N / L / H
- I Integrity
    - N / L / H
- A Availability
    - N / L / H
- S Scope (linked with PR , if vuln. affect system components)
    - U Unchanged / C Changed

<aside>
👉

**CVSS BASE SCORE Rating**
0.0 None
0.1–3.9 Low
4.0–6.9 Medium
7.0–8.9 High
9.0–10.0 Critical

</aside>

- Vulnerabilty classification
    - Improper Patch management
    - Legacy platforms
    - Weak configuration
    - Default accounts
    - Error messages
    - Insecure Protocols
    - Weak encryption