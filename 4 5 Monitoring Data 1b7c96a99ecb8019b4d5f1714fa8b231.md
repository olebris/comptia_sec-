# 4.5 Monitoring Data

Created time: 15 mars 2025 19:00
Last edited by: OLB_
Last edited time: 21 mars 2025 12:01

- FIM (File Integrity Monitoring)
    - fingerprint and monitor/track file change
    - Windows SFC
    - Linux Tripwire
    - HIPS (on OS important files)
- DLP
    - on a computer ⇒ endpoint DLP / Agent-based DLP
        - block USB
        - search for sensitive data with pattern matching (number or sensitive words)
        - monitor system config and can block action
        - block watermarked data (DRM or Data tagged as sensitive)
    - on network ⇒ data in motion /Agentless (network-based) DLP
        - block transmission of sensitive data (watermark or pattern)
        - can automatically encrypt data
    - on server ⇒ data at rest / Agent-based DLP
    - cloud base DLP
    - can check Emails
        - can automatically encrypt data IN EMAIL
    
- **Data at rest** is stored data that resides on hard drives, tapes, in
the cloud, or on other storage media. This data is prone to theft by
insiders or external attackers who gain access to systems and are
able to browse through their contents.
- **Data in transit** is data that is in motion/transit over a network.
When data travels on an untrusted network, it is open to
eavesdropping attacks by anyone with access to those networks.
- **Data in use** is data that is actively in use by a computer system.
This includes the data stored in memory while processing takes
place. An attacker with control of the system may be able to read
the contents of memory and steal sensitive inform