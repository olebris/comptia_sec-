# 2.4 Application Attack

Created time: 14 mars 2025 15:18
Last edited by: OLB_
Last edited time: 4 avril 2025 16:31

- Code injection (sqli, xss, xxe, ldap)
    - reflected XSS Vs Stored XSS
- Command injection Attacks `param & rm -rf`
- buffer overflow
- replay attack (need network tap or arp poisoning)
- privilege escalation
- CSRF attack : “Cross side request forgery”

![image.png](image%2036.png)

<aside>
👉

XSS attacks exploit the trust that a user has in a website to execute code on the user's computer. 

X/CSRF attacks exploit the trust that remote sites have in a user's session to execute
commands on the user's behalf.

</aside>

- Directory/Path Traversal
    - read file outside of website directory
- IDOR Insecure direct object reference
- File inclusion
    - LFI
    - RFI
- Session cookie stealing
    - XSS or on-path/MITM attack
- Pollution parameter

[`https://exemple.com/login?user=admin&user=attaquant`](https://exemple.com/login?user=admin&user=attaquant)