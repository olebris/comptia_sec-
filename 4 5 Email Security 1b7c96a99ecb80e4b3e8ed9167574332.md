# 4.5 Email Security

Created time: 15 mars 2025 19:00
Last edited by: OLB_
Last edited time: 5 avril 2025 16:01

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
    - define rules when email from **OUR DOMAIN** are not compliant to SPF / DKIM
    - Protection against Domain Usurpation
    - policy written in DNS TXT record (accept / spam / quarantine / reject)
    - reports sent to email admin

```bash
#DKIM
default._domainkey.example.com. IN TXT "v=DKIM1; k=rsa; p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAuJdZ...<rest of the public key>...IDAQAB"

#SPF
example.com. IN TXT "v=spf1 ip4:192.0.2.0/24 ip6:2001:db8::/32 include:_spf.google.com ~all"

#DMARC
_dmarc.example.com. IN TXT "v=DMARC1; p=quarantine; rua=mailto:dmarc-reports@example.com; ruf=mailto:dmarc-forensic@example.com; pct=100"

```