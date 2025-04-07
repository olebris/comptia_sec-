# 4.1 Wireless Network

Created time: 14 mars 2025 23:59
Last edited by: OLB_
Last edited time: 5 avril 2025 15:04

- Cellular
    - LTE / 4G / 5G
- Bluetooth
    - 2.4Ghz
    - 4 security mode
    - Use pin on both devices for encryption
- Zigbee

- Wi-Fi
    - 2.4Ghz or 5Ghz
    - 802.11 Standard
- WPA2
    - use CCMP protocol which use AES for encryption and user authentication (but not network authentication)
    - WPA2-Personal / WPA2-PSK
        - PSK hash can be listen during handshake
        - PSK can be bruteforced
    - WPA2-Enterprise
        - use 802.1.X / Radius
- WPA3-Personal
    - use GCMP / AES encryption
    - (no more PSK) key not send across network ⇒ **use SAE** Simultaneous authentication of equals ****(derived from Diffie Hellman)
    - implements **perfect forward secrecy** (single exposed key won't result
    in the entire communication being exposed)
- WPA3-Enterprise
    - Stronger Encryption (192 or 256 bits)
    - Use 802.1x Auth.
    - WPA3-802.1X use Radius

# NAC / 802.1X

- RADIUS
    - most common AAA protocol
    - centralize Authentication for
        - routers, switches, firewall
        - server authentication
        - remote VPN acess
        - NAC / 802.1X Network (Wireless or Ethernet)

![image.png](image%2042.png)

- EAP

Extensible Authentication Protocol (EAP) is an authentication
framework that is commonly used for wireless networks

- EAP-TLS ( need client certificate )
- EAP-TTLS (no client certificate but password - need sometimes a agent on client)
- PEAP (no client certificate, no agent ,wrap EAP in TLS )

Other auth. protocols:

- LEAP (Cisco protocol , less secure)
- CHAP (challenge based Auth)
- PAP (no more secure)

<aside>
👉

Open Wi-Fi networks also get an upgrade with the Wi-Fi
Enhanced Open certification, which uses opportunistic wireless
encryption (OWE) to provide encrypted Wi-Fi on open networks
when possible

</aside>