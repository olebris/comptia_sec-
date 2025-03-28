# 2.4 Cryptography attacks

Created time: 14 mars 2025 15:34
Last edited by: OLB_
Last edited time: 28 mars 2025 17:36

- bad cryptography implementation
- birthday attack
    - use of hash collision
    - md5 is prone to birthday attack
- downgrade attack (lower encryption level)
    - ssl stripping (remove ssl with a “mitm proxy”)

![image.png](image%2024.png)

- brute force
- frequency analysis (find patterns in cypher text)
- Known plain text (try to derive the key from a known plain text and his cypher text) EX: “Heil Hitler” for Enigma
    - chosen plain text
    - related key attack
- Rainbow table attack
    - use salt & pepper
    - key stretching (lot of iterations with salt)
- TOR
    - perfect forward secrecy