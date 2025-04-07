# 3.2 Secure communication

Created time: 14 mars 2025 20:01
Last edited by: OLB_
Last edited time: 5 avril 2025 14:26

- VPN
    - encrypt private data across public network in **a tunnel**
    - often embedded in FW
    - hardware of software
    
    ![image.png](image%2039.png)
    

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
    - SD WAN + Secure services (SWG, CASB (cloud access), ZTNA (zero trust) ,FWaaS )
    - zero trust
    - Deep packet Inspection
    - Access from everywhere

![image.png](image%2040.png)

- SWG: Secure web gateways (SWGs) also provide a layer of application
security for cloud-dependent organizations. SWGs monitor web
requests made by internal users and evaluate them against the
organization's security policy, blocking requests that run afoul of these
requirements. SWGs are commonly used to block access to potentially
malicious content but may also be used to enforce content filtering

![image.png](image%2041.png)

### CASB:

Cloud access security brokers (CASBs) are software tools that serve as
intermediaries between cloud service users and cloud service providers. This positioning allows them to monitor user activity and enforce policy requirements. CASBs operate using two different
approaches:

- **Inline CASB solutions** :

seeing requests before they are sent to the cloud service, allowing the CASB to block requests that violate policy

- **API-based CASB solutions**

it also does not allow the CASB to block requests that violate policy. API-based CASBs are limited to monitoring user activity and reporting on or correcting policy violations after the fact.

###