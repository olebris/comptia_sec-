# 2.4 Application Attack

Created time: 14 mars 2025 15:18
Last edited by: OLB_
Last edited time: 27 mars 2025 23:21

- Code injection (sqli, xss, xxe, ldap)
    - reflected XSS Vs Stored XSS
- Command injection Attacks `param & rm -rf`
- buffer overflow
- replay attack (need network tap or arp poisoning)
- privilege escalation
- CSR - Cross site request
    - are legitimate most of the time (ex youtube embedded video)
    - CSRF attack : “Cross side request forgery” attack use CSR

![image.png](image%2023.png)

CSRF attack

<aside>
👉

XSS attacks exploit the trust that a user has in a website to execute code on the user's computer. 

X/CSRF attacks exploit the trust that remote sites have in a user's system to execute
commands on the user's behalf.

</aside>

- Directory/Path Traversal
    - read file outside of website directory
- IDOR Insecure direct object reference
- File inclusion
    - LFI
    - RFI
- Session cookie stealing
- Pollution parameter

[`https://exemple.com/login?user=admin&user=attaquant`](https://exemple.com/login?user=admin&user=attaquant)