# 2.4 Replay Attack

Created time: 14 mars 2025 14:57
Last edited by: OLB_
Last edited time: 14 mars 2025 15:11

- Need a network TAP (Test Access Point)
    - a device that copy packet for further analysis (or replay)
- or need ARP poisoning

⇒ reply copied frames without the need of computer victim (so it’s not MITM/on path attack)

- “Pass the Hash” is a replay attack !
- Cookies manipulation
    - Steal cookies (session ID) for reuse is a replay attack
- Header manipulation (HTTP)
    - Wireshark , Kismet (wifi)  for sniffing HTTP streams
    - Tamper, Firesheep , Scapy for manipulating headers and replay
- Remediation:
    - End to end encryption (HTTPS)