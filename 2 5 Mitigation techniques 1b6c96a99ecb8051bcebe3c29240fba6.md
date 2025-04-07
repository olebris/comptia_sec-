# 2.5 Mitigation techniques

Created time: 14 mars 2025 16:12
Last edited by: OLB_
Last edited time: 4 avril 2025 18:04

- Patching
    - updates (auto or manual)
- Encryption
    - Encryption of file system (bitlocker, filevault, luks, veracrypt)
    - encryption of sensitive files (encfs, windows efs)
    - application data encryption
- Monitoring
    - log agreggation in central place (SIEM …)
    - monitor sensor (ids, firewall,email)
    - correlate logs with SIEM
- Least Privilege
    - limit to bare minimum
    - no user with admin privilege
- Configuration enforcement
    - posture assessment (evaluation de sécurité)
        - CONFIG CHECKLIST
    - CIS Benchmark
    - extensive check for os ,edr , firewall , certificate …
    - EOL systems
        - private VLAN
        - Quarantined
- Decommissining
    - have a formal policy
    - format and destroy drives