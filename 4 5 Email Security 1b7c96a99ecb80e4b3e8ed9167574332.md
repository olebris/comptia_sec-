# 4.5 Email Security

Created time: 15 mars 2025 19:00
Last edited by: OLB_
Last edited time: 15 mars 2025 19:15

- Mail Gateway
    - in a screened subnet / DMZ
    - check inbound email messages before sending to internal email server
- SPF
    - list of authorized SMTP
    - DNS TXT Record
- DKIM
    - Digital signature of outgoing emails
    - Public key is in DKIM TXT record
- DMARC
    - define rules when email are not compliant to SPF / DKIM
    - policy written in DNS TXT record (accept / spam / quarantine / reject)
    - reports sent to email admin