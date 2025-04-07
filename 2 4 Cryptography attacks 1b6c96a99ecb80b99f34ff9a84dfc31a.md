# 2.4 Cryptography attacks

Created time: 14 mars 2025 15:34
Last edited by: OLB_
Last edited time: 4 avril 2025 16:35

- bad cryptography implementation
- birthday attack
    - use of hash collision
    - md5 is prone to birthday attack
- **downgrade attack** (lower encryption level)
    - **ssl stripping** (remove ssl with a “mitm proxy”)
        - possibilité de faire proxy SSL mais il faut que la victime accepte le certificat de l’attaquant
        - plus simple est de simuler une réponse en http a un site qui répond en http avant de passer en https (cf ci dessous)

![image.png](image%2038.png)

- brute force
    - John / Hashcat …
- frequency analysis (find patterns in cypher text)
- Known plain text (try to derive the key from a known plain text and his cypher text) EX: “Heil Hitler” for Enigma
    - chosen plain text
    - related key attack
- Rainbow table attack
    - use salt & pepper to mitigate
    - key stretching (lot of iterations with salt)
- TOR
    - perfect forward secrecy protection
    - PFS prevent nodes in the relay chain
    from reading anything other than the specific information they need to accept and forward the traffic