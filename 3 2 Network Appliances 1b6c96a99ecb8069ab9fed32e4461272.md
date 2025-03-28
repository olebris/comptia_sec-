# 3.2 Network Appliances

Created time: 14 mars 2025 18:52
Last edited by: OLB_
Last edited time: 14 mars 2025 19:11

- Jump server
    - access to a protected network
    - hardened and monitored
    - VPN / SSH to the jump server
    - SSH/ RDP  from jump server
- Proxy server
    - between stations and internet
    - Cache
    - URL filtering
    - Content Scanning
    - Explicit (browser config) or Transparent (gateway)
    - Forward Proxy (user ⇒ internet)
    - Reverse Proxy (internet ⇒ web server)
    - Open proxy (proxy open on internet and managed by third party - eg: for anonymisation)
- Load Balancer
    - distribute load
    - fault tolerance
    - use by server farms / clusters
    - **active / active**
        - TCP offload (TCP connection with servers could stay open)
        - SSL offload (encryption managed in load balancer)
        - Caching
        - Priority / QoS
        - Content switching
            - give some content to the correct serveur
    - active / passive
        - some servers on standby or passive
        - passive servers only becom active on failure of an active server
- Sensors
    - SNMP
    - IDS / IPS
    - Web logs
    - Firewall logs
    - App logs
    - Database logs …;
- Collectors
    - Log aggregation
    - SIEM (with correlation engine)
    - Syslogs servers