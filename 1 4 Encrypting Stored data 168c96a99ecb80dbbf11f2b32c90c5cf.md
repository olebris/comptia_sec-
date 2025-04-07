# 1.4 Encrypting Stored data

Created time: 26 décembre 2024 19:00
Last edited by: OLB_
Last edited time: 6 avril 2025 13:57

- Encryption to protect data at rest (hard drive, cloud drive)
    - Full disk encryption / Partition
        - LUKS (Linux) or
        - Bitlocker (Windows)
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
    - *(AES ECB ⇒ Weak)*
    - AES/Rijndael
    - fast
    - key exchange is a problem (insecure )
    - Cannot be used for non-repudiation
    - algorithm not scalable for groups (number of keys)
    - must change often (if someone quit the group)
- Asymetric keys
    - Complex calculation of prime numbers
    - Very large keys (3072 bits or larger)
    - Key exchange easy
    - No preexisting communication needed
    - provide non-repudiation / integrity / authentication
    - key regeneration only if private key compromised
    - key revocation possible
    - scalable for groups
- Key Stretching
    - multiple hash avec une clé jugée faible (hash du hash)
    - ralenti le bruteforce
- Ciphers
    - block ciphers (ex: AES)
        - use block by block
        - appropriate for data at rest and authentication
    - stream ciphers (ex: ChaCha20)
        - bit by bit
        - apropriate for data in transit like **streaming** (less ressources needed)

![image.png](image%2011.png)

<aside>
👉

The three main methods used to exchange secret keys
securely are ****

- **Offline distribution**
- **Public key exchange**
- **Diffie-Hellman key exchange**
</aside>

ECC (Elliptic Curve Cryptography)

- replace (modern variant of)  **RSA / DH** in modern app for Public Key Exchange
- more secure & with smaller Key (256bits generally instead of 3072bits for RSA)

![image.png](image%2012.png)

- Hashing
    - SHA-1 obsolete
    - SHA2 is widely used
        - SHA256 (most used) or SHA512 (more secure but slower)
    - SHA3 for the future (post quantique)
- Digital signatures
    - Integrity
    - non-repudiation
    - code signing

<aside>
👉

The Hash-Based Message Authentication Code (HMAC) algorithm
implements a partial digital signature with a hash + a shared secret key

*Signature = HMAC(key+message)*

HMAC guarantees the integrity of a message during transmission, but it does not provide for non-repudiation. 

> Bien que HMAC garantisse l'intégrité et l'authenticité des messages entre les parties partageant une clé secrète, il ne garantit pas la non-répudiation. Pour la non-répudiation, il est nécessaire d'utiliser des signatures numériques basées sur des paires de clés publique/privée, où chaque partie possède une clé privée unique. Cela permet de prouver de manière indépendante qui a envoyé un message, car seul l'expéditeur peut créer une signature valide avec sa clé privée.
> 
</aside>

<aside>
👉

**Homomorphic Encryption**

When you encrypt data with a homomorphic algorithm and then perform computation on that data, you get a result that, when decrypted, matches the result you would have received if you had performed the computation on the plain-text data in the first place.

</aside>