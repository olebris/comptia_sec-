# 3.2 Network Appliances

Created time: 14 mars 2025 18:52
Last edited by: OLB_
Last edited time: 5 avril 2025 12:00

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
            - can forward request to the correct backend serveur based on content analysis
    - active / passive
        - some servers on standby or passive
        - passive servers only become active on failure of an active server
        
    
    ### Load-balancing algorithms
    
    - Round-robin sends each request to servers by working through a
    list, with each server receiving traffic in turn.
    - Least connection sends traffic to the server with the fewest
    number of active connections.
    - Agent-based adaptive balancing monitors the load and other
    factors that impact a server's ability to respond and updates the
    load balancer's traffic distribution based on the agent's reports.
    - Source IP hashing uses a hash of the source IP to assign traffic to
    servers. This is essentially a randomization algorithm using client-
    driven input
- Network logs
    - SNMP sensors
    - IDS / IPS logs
    - Web logs
    - Firewall logs
    - App logs
    - Database logs …
- Log Collectors
    - Syslog servers (syslog-ng, rsyslog)
    - SIEM (with correlation engine)
    

## Network security devices TAP / IDS / IPS

- active (powered- ex: **SPAN** -switch port mirroring  )
- OR passive / unpowered - ex: **TAP** : Y cable + collector
- Installation can be i**nline mode** OR **tap mode**

![image.png](image%2032.png)

- **Out of band management**
    - A separate means of accessing the FW/IDS/UTM administrative interface should exist. (physical or separate management VLAN)