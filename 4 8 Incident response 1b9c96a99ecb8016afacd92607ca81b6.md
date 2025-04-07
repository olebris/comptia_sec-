# 4.8 Incident response

Created time: 17 mars 2025 20:42
Last edited by: OLB_
Last edited time: 5 avril 2025 17:17

- 1- Preparation
    - build and train an IR team
    - build incident analysis infrastructure (documentation, KB, SIEM, NetFlow, SOAR)
    - set tools for incident response (Ticketing solution, Jump kit for analysis and malware eradication tools…)
    - POLICIES and PROCEDURES !
        - IR Policy (team, authority, description of the IR process, rules in case of emergency …)
            - contacts and procedure in case of emergency
            - communication plan (methods, teams, stakeholders, medias)
        - BC: Business continuity Plan (restore plan or alternate solutions )
        - DR: Disater recovery Plan (response for natural or human-made disaster)
        
- 2- Detection and analysis
    - SIEM / log analyse
        - correlates logs from FW/IDS/EDR/Apps ..
        - use **Netflow (cisco)** or sFlow or IPFIX for network flow analysis
    - real time alerts (IPS, EDR, Firewall)
    - detect IoC
        - Network problems
        - Production incident (shut down, slow down, alerts from operational team)
        - Threat hunting (proactive search of IoC) & MITRE ATTACK analysis
    
- 3- Containment eradication and recovery
    - Isolation or Containment
        - host isolation (remove from network) or segmentation (vlan)
        - host containment (keep online but set firewall rules to block malware or set application level containment)
    - Remove the malware
    - Root cause analysis
        - five whys
        - event analysis
        - Diagramming
    - Fix vulnerabilities
    - Restore or rebuild
- 4- Post incident Activity
    - Lesson learned
    - post incident meeting
    - timeline of the events
    - incident plan retex/ retrospective
    - How to improve the plan
- Training
    - train team before an incident