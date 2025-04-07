# 3.1 Network Infrastructure concepts

Created time: 14 mars 2025 17:01
Last edited by: OLB_
Last edited time: 4 avril 2025 18:27

- Physical  isolation
    - different devices
    - different racks generally
    - can isolate customers and not mixing data between networks
    - could communicate **but generally not**
- Physical segmentation
    - differents switches. 1 per  customer
    - same rack
    - communication is controlled
- Logical segmentation
    - VLANs in the same device / switch
    - 1 switch for 2 customers
- SDN (Software Defined Networking) - (model for building Software Network devices)
    - 3 layers: Data , control and management plane
    - Data plane : process the frames, encrypt, NAT
    - Control plane : control data plane actions, provide : routing tables, NAT tables, Dynamic Routing rules
    - Management Plane: configure the device, Web UI, SSH, SNMP
    - SDN: Allow central management of Network devices (settings, quarantined, isolation,dynamic config…)
- SD-WAN
    - Software defined WAN : MPLS + 5G + broadband networks (fiber) network with smart routing based on application requirements while controlling costs. Ex: email won’t use MPLS but Voice or video use MPLS
- CASB cloud access security broker
    - PEP Policy Enforcement Point used between service providers and service
    consumers to allow organizations to enforce their policies for cloud
    resources
- SASE (”sassy”) Secure Access Service Edge
    - VPN + CASB + FW + Zero Trust + SD-WAN  (= SD-WAN + secure services)
    - SASE is deployed to ensure that endpoints are secure, that
    data is secure in transit, and that policy-based security is delivered as
    intended across an organization's infrastructure and services.
- Zero Trust
    - each action is validated when requested as part of a continuous authentication
    process and access is only allowed after policies are checked, including
    elements like **identity, permissions, location, device fingerprint, system configuration and security status, threat intelligence data review, and security posture**.

![image.png](image%2035.png)

- NAC network access control
    - protecting networks from unauthorized access
    - Agent-based NAC or agentless
    - Preadmission NAC decisions : keep potentially dangerous systems off a network
    - Postadmission decisions can help with response and prevent failed NAC access
    attempts from stopping business
- NAC and 802.1X
    - 802.1X is a standard use in NAC
    - 802.1X use EAP for centralized authentication
- Jump servers
    - way to securely operate insecurity zones with different security levels