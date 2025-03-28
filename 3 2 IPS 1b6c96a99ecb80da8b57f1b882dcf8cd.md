# 3.2 IPS

Created time: 14 mars 2025 18:42
Last edited by: OLB_
Last edited time: 14 mars 2025 18:51

- Intrusion Prevention system
- IDS - detect
- IPS - block XSS, buffer overflow, network scan …
- Failure mode
    - Fail-open  : if system fails ⇒ leave data flow open
    - Fail-closed  : if system fails ⇒ block the data flow
- IPS active monitoring
    - IPS is in real time and analyse real traffic
- IPS passive monitoring
    - IPS use a copy of network traffic
        - via a port mirror SPAN (switch port analyser) or network TAP (test access point)
    - Can only alert / detect but not block traffic
    - IPS act more like an IDS
-