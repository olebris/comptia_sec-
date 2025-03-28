# 3.2 Firewall types

Created time: 14 mars 2025 19:37
Last edited by: OLB_
Last edited time: 14 mars 2025 20:01

- Filter Traffic
    - OSI layer 4 Vs Layer 7
    - Traditional FW Vs NGFW
- Encrypt traffic
    - VPN site to site
- Routing (layer 3)
    - NAT
    - Dynamic Routing
- UTM Unified Threat Management (all in one device)
    - URL filter / Content Filter
    - Malware inspection
    - Spam filter
    - IDS / IPS
    - Routing
    - VPN
    - Authentication
    - CSU / DSU (Channel Service Unit/Data Service Unit)
        - LAN / WAN interface
        - Connect to telecom network (similar to a MODEM)
    - OSI level 4 and level 7 ⇒ performance problems
- NGFW
    - OSI level 7 (see everything in the packet)
    - Stateful multilayer inspection
    - Application layer gateway
    - deep packet inspection DPI
    - control traffic based on application
    - act as IPS
    - Content / URL filtering
- WAF
    - for HTTP/HTTPS
    - filter input stream towards web applications
    - protect from SQLi or XSS