# 2.3 Cloud / Web specific vuln.

Created time: 29 décembre 2024 19:38
Last edited by: OLB_
Last edited time: 4 avril 2025 15:26

- Password Attacks (BF, credential stuffing, password spraying ..)
    - 76% of organizations aren’t using MFA in their cloud management console
- DoS / DDoS
- Authentication bypass
    - weak auth
    - lack of control
- Directory traversal
- Remote code Execution RCE (mostly via CVE)
- XSS
- SQLi
- Buffer OverFlow

### CLOUD

- **VM escape**
- **VM sprawl** : when IaaS users create virtual service instances and then forget about them or abandon them, leaving them to accrue costs and accumulate security issues over time.
- Resource reuse : cloud providers take hardware resources that were originally assigned to one customer and reassign them to another customer. If the data was not properly removed from that hardware, the new customer may inadvertently gain access to data belonging to another customer.