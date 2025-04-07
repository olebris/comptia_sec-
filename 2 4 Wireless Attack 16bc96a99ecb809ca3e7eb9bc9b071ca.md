# 2.4 Wireless Attack

Created time: 29 décembre 2024 22:44
Last edited by: OLB_
Last edited time: 4 avril 2025 17:56

- Evil twins
    - malicious AP (often more powerful AP than the legitimate one)
- Rogue Access Points
    - non authorized but not necessarily malicious AP
- Wireless deauthentication attack
    - Not working anymore w/ WPA3 (encrypted management frames)
- bluetooth
    - bluejacking : send unsolicited messages
    - bluesnarfing : unauthorized access to a device
- 802.11 management frames (access point, QoS, association/disassociation)
    - not protected by design of IEE 802.11
    - until WPA3 : management frames sent in clear / easy to manipulate
- WPA3 /  :
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
- Radio Frequency Jamming
    - DoS by interfering with wireless signals
- Wireless jamming
    - send constants or big amount of legitimate frames

Remediation w/ FOX Hunting

- with directionnal antenna searching for the jamming source

- War (Drone) driving attack
    - Use car or drone to scan vulnerable WIFI