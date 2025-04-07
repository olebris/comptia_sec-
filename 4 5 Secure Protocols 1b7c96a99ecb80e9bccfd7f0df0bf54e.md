# 4.5 Secure Protocols

Created time: 15 mars 2025 18:51
Last edited by: OLB_
Last edited time: 5 avril 2025 16:28

- TELNET, FTP, SNMTP , IMAP are not secured
    - Telnet ⇒ SSH
    - HTTP ⇒ HTTPS
    - IMAP ⇒ IMAPS
    - POP ⇒ POP3S
    - FTP ⇒ SFTP
    - NTP ⇒ NTS
    - SIP ⇒ SIPS /SRTP
    - LDAP ⇒ LDAPS
    - DNS ⇒ DNSSEC (DNS record is signed by DNZ Zone server)
    - SNMP ⇒ SNMPv3 with authPriv
    - RTP ⇒ SRTP
- WIFI ⇒  802.11 WPA3
- VPN Ipsec or VPN SSL
- S/MIME
    - sign email en encrypt content
    - need a certificate signed by CA to send AND receive !
- VPN IPSEC protocols
    1.  ****Association (SA):
        1. **ISAKMP**  & IKE : Security Association (SA) before exchange (using X.509 certificates)
    2.  Data Exchange 
        1. Authentication Header (**AH**) : hash to ensure packet integrity and authentication
        2. **ESP** :  encrypt data for confidentiality
    -