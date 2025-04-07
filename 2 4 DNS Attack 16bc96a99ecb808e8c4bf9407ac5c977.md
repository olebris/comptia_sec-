# 2.4 DNS Attack

Created time: 29 décembre 2024 22:33
Last edited by: OLB_
Last edited time: 4 avril 2025 17:05

- **Dns Poisoning / Pharming**
    - modify DNS server itself (uneasy)
    - modify client host files
    - send a fake DNS response (MITM / on path attack)
    - domain hijacking
        - access to registrar website (brute force, password leak ..)
        - change domain settings (zone records)
- Typosquatting
    - misspelling
    - typing error
    - different top-level domain (.com / .org) …
- Mitigation
    - DNSSEC
        - DNSSEC provides authentication of DNS data, allowing DNS queries to be validated even if they are not encrypted.
    - Prevent zone transfert
    - Activate DNS logging
    - DNS Filtering :
        - block DNS of malicious domains (ex: NextDNS)
        - Use domain reputation service