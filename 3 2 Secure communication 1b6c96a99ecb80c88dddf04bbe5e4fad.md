# 3.2 Secure communication

Created time: 14 mars 2025 20:01
Last edited by: OLB_
Last edited time: 14 mars 2025 20:20

- VPN
    - encrypt private data across public network in **a tunnel**
    - often embedded in FW
    - hardware of software
    
    ![image.png](image%2025.png)
    

*Encapsulation IPSEC*

- VPN TLS / SSL
    - port 443 = no FW issues
    - usually for a single device or small VPN
    - light client (browser / small app)
- VPN IPSEC
    - always on
    - site to site
    - no need software on PC :  just 2 VPN concentrator (1 at each site)
    - VPN concentrators = often FW
- SD-WAN
    - a WAN build for the cloud
    - no central point
    - each node is connected dynamically without the central point
- SASE - Secure Access Service Edge
    - next GEN for VPN
    - SD WAN + Secure services (CASB (cloud access), ZTNA (zero trust) ,FWaaS )
    - zero trust
    - Deep packet Inspection
    - Access from everywhere

![image.png](image%2026.png)