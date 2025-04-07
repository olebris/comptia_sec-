# 4.6 Access Controls

Created time: 17 mars 2025 19:22
Last edited by: OLB_
Last edited time: 5 avril 2025 16:38

- Least Privilege
- **Permission Creep** signifie qu’avec le temps, une personne accumule trop de droits d’accès à un système. Cela arrive souvent quand elle change de rôle sans que ses anciens accès soient retirés.
- PAM Privilege Access Management
    - JIT Just in time permissions
    - Password vaulting
        - you don’t know the master password
        - logged and auditable event
    - Ephemeral accounts

## Access Control Scheme

- MAC Mandatory Access Control
    - based on labels (ex: accès bloqué aux dossiers confidential)
        - decided by admin
        - user cannot change settings
        - Selinux or Windows  MIC
- DAC Discretionary Access control (ex Linux w/ chmod)
    - owner control who has access
    - flexible access control but weak security
- RBAC Role Based access  control (ex: sudo in Linux)
    - based on role (manager, team lead , user ..)
    - easy to implement / maintain
- Rule-base Access Control (ex Firewall rules)
    - generic for rules not based on who you are
    - rules depend on the object
        - ex: no SSH from 9PM to 5AM
    - rules = ACL Access Control List
- ABAC Role base on attributes
    - more flexible
    - combine different criteria

![image.png](image%2051.png)