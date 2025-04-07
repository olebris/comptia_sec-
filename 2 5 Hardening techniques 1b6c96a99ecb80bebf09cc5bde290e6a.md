# 2.5 Hardening techniques

Created time: 14 mars 2025 16:25
Last edited by: OLB_
Last edited time: 4 avril 2025 18:00

- System hardening
    - update
    - password policy (**length**, complexity)
    - limit accounts
    - limit Network access
    - AV, EDR
    - Monitoring , logs
    - apply Security baseline w/ CIS Benchmark
- Encryption
    - EFS (files)
    - Bitlocker (Full disk Encryption - FDE)
    - VPN
    - Encrypted protocol
- Endpoint
    - start of the defense in depth
    - EDR - Endpoint detection and Response
        - behavioral analysis
        - machine learning
        - process monitoring
        - lightweight agent
        - Detection: investigate the threat
        - Response: isolate the endpoint, quarantine the threat , rollback to previous config
        - API driven , Automated, Central management
- Software Firewall
    - Control outgoing and incoming traffic
    - Alllow / disallow traffic
    - can prevent malware execution
- HIPS - Host Intrusion Prevention System
    - block attacks based on signatures, heuristics (already known process), behavioral (anormal behavior)
    - block registry change, buffer overflow …
- Open Ports and services
    - close everything except required ports
    - NGFW - New Generation Firewall
    - deactivate unused services
    - use nmap scan to verify
    - default password change + add MFA
- Remove unused Software