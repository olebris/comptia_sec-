# 2.3 Misconfiguration Vuln.

Created time: 29 décembre 2024 21:14
Last edited by: OLB_
Last edited time: 14 mars 2025 13:25

- Cloud storage (Amazon S3) open permission
- Unsecured Admin accounts
    - admin/admin : root/root
    - easy password
- Don’t log with root account and use sudo
- limit root permissions to a few accounts
- Insecure protocols
    - FTP / TELNET / SMTP / IMAP
    - disclosure in packet capture
- Default settings
    - change default login / password
- Open ports and services
    - Firewall rules to limit Attack surface