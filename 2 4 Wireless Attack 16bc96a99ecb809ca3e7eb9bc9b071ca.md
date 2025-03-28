# 2.4 Wireless Attack

Created time: 29 décembre 2024 22:44
Last edited by: OLB_
Last edited time: 14 mars 2025 14:51

- Wireless deauthentication attack
- 802.11 management frames (access point, QoS, association/disassociation)
    - not protected by design of IEE 802.11
    - sent in clear / easy to manipulate
- 802.11ac :
    - protect deauth attacks
    - encrypt some management frames
        - disassociation
        - deauthentication
        - channel switch
    - not everything is encrypted
        - beacons
        - probes
        - authentication
        - association
- Rado Frequency Jamming
    - DoS by interfering with wireless signals
- Wireless jamming
    - send constants or big amount of legitimate frames

Remediation w/ FOX Hunting

- with directionnal antenna searching for the jamming source