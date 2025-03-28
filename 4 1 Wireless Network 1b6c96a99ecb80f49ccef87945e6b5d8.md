# 4.1 Wireless Network

Created time: 14 mars 2025 23:59
Last edited by: OLB_
Last edited time: 15 mars 2025 14:44

- WPA2
    - PSK hash can be listen during handshake
    - PSK can be bruteforced
- WPA3
    - use GCMP / AES encryption
    - key not send across network ⇒ SAE (derived from Diffie Hellman)
- Use 802.1x Auth.
- WPA3-802.1X remplace la PSK par une authentification Radius
- RADIUS
    - most common AAA protocol
    - centralize Authentication for
        - routers, switches, firewall
        - server authentication
        - remote VPN acess
        - NAC / 802.1X Network (Wireless or Ethernet)

![image.png](image%2027.png)