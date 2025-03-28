# 1.4 Encrypting Stored data

Created time: 26 décembre 2024 19:00
Last edited by: OLB_
Last edited time: 28 mars 2025 14:44

- Encryption to protect data at rest (hard drive, cloud drive)
    - Full disk encryption / Partition
        - LUKS (Linux) or
        - Bitlocker (Window)s)
        - FileVault (Mac)
        - Veracrypt (All)
    - File Encryption
        - EFS (Windows over NTFS)
        - EncFS, 7zip …
    - Database Encryption
        - TDE : transparent encryption (symetric key for the whole table)
        - CLE : column level encryption (different symetric key for colums)
        - RLE: Record-level encryption (for one record)
- Transport Encryption
    - HTTPS
        - TLS
    - VPN
        - TLS
        - IPsec
    - SSH
- Symetric keys
    - 128 bits or larger (192,256)
    - AES ECB ⇒ Weak
    - AES/Rijndael
    - fast
    - key exchange is a problem (insecure )
    - Cannot be used for nonrepudiation
    - algorithm not scalable for groups (number of keys)
    - must change often (if someone quit the group)
- Asymetric keys
    - Complex calculation of prime numbers
    - Very large keys (3072 bits or larger)
    - Key exchange easy
    - No preexisting communication needed
    - provide nonrepudiation / integrity / authentication
    - key generation only if private key compromised
    - key revocation
    - scalable for groups
- Key Stretching
    - multiple hash avec une clé jugée faible (hash du hash)
    - ralenti le bruteforce
- Cyphers
    - block ciphers
        - use block by block
        - appropriate for data at rest and authentication
    - stream ciphers
        - bit by bit
        - apropriate for data in transit like streaming (less ressources needed)

![image.png](image%206.png)

<aside>
👉

The three main methods used to exchange secret keys
securely are offline distribution, public key encryption, and the Diffie–
Hellman key exchange algorithm.

</aside>

ECC (Elliptic Curve Cryptography)

- replace RSA / DH in modern app for  Public Key Exchange
- more secure with smaller Key (256bits generally instead of 3072bits for RSA)

![image.png](image%207.png)

- Hashing
    - SHA-1 obsolete
    - SHA2 is widely used
        - SHA256 (most used) or SHA512 (more secure but slower)
    - SHA3 for the future (post quantique)
- Digital signatures
    - Integrity
    - nonrepudiation
    - code signing

<aside>
👉

The Hash-Based Message Authentication Code (HMAC) algorithm
implements a partial digital signature—it guarantees the integrity of a
message during transmission, but it does not provide for non-
repudiation. EX: link to activate an account sended by email by website with HMAC = (email + expiration time + secret key)

</aside>