# Sum: 7- Cryptography & PKI

Created time: 28 mars 2025 18:06
Last edited by: OLB_
Last edited time: 3 avril 2025 15:26

<aside>
👉

Cryptography is one of the most important security controls in use
today and it touches almost every other area of security, ranging from
networking to software development. The use of cryptography
supports the goals of providing confidentiality, integrity,
authentication, and non-repudiation in a wide variety of applications.

Symmetric encryption technology uses shared secret keys to provide
security for data at rest and data in motion. As long as users are able to
overcome key exchange and maintenance issues, symmetric
encryption is fast and efficient. Asymmetric cryptography and the
public key infrastructure (PKI) provide a scalable way to securely
communicate, particularly when the communicating parties do not
have a prior relationship.

**Understand the goals of cryptography.** The four goals of
cryptography are confidentiality, integrity, authentication, and non-
repudiation. Confidentiality is the use of encryption to protect
sensitive information from prying eyes. Integrity is the use of
cryptography to ensure that data is not maliciously or unintentionally
altered. Authentication refers to uses of encryption to validate the
identity of individuals. Non-repudiation ensures that individuals can
prove to a third party that a message came from its purported sender.

**Explain the differences between symmetric and asymmetric
encryption.** Symmetric encryption uses the same shared secret key
to encrypt and decrypt information. Users must have some
mechanism to exchange these shared secret keys. The Diffie–Hellman
algorithm provides one approach. Asymmetric encryption provides
each user with a pair of keys: a public key, which is freely shared, and a
private key, which is kept secret. Anything encrypted with one key
from the pair may be decrypted with the other key from the same pair.

**Explain how digital signatures provide non-repudiation.**
Digital signatures provide non-repudiation by allowing a third party to
verify the authenticity of a message. Senders create digital signatures
by using a hash function to generate a message digest and then
encrypting that digest with their own private key. Others may verify
the digital signature by decrypting it with the sender's public key and
comparing this decrypted message digest to one that they compute
themselves using the hash function on the message.

**Understand the purpose and use of digital certificates.** Digital
certificates provide a trusted mechanism for sharing public keys with
other individuals. Users and organizations obtain digital certificates
from certificate authorities (CAs), who demonstrate their trust in the
certificate by applying their digital signature. Recipients of the digital
certificate can rely on the public key it contains if they trust the issuing
CA and verify the CA's digital signature.

**Demonstrate familiarity with emerging issues in
cryptography.** Tor uses perfect forward secrecy to allow anonymous
communication over the Internet. The blockchain is an immutable
distributed public ledger made possible through the use of
cryptography

</aside>

## **CHECK EXAM**

THE COMPTIA SECURITY+ EXAM OBJECTIVES
COVERED IN THIS CHAPTER INCLUDE:

Domain 1.0: General Security Concepts
1.4. Explain the importance of using appropriate
cryptographic solutions.

- Public key infrastructure (PKI) (Public key, Private key,
Key escrow)
- Encryption (Level (Full-disk, Partition, File, Volume,
Database, Record), Transport/communication,
Asymmetric, Symmetric, Key exchange, Algorithms,
Key length)
- Obfuscation (Steganography)
- Hashing
- Salting
- Digital signatures
- Key stretching
- Blockchain
- Open public ledger
- Certificates (Certificate authorities, Certificate
revocation lists (CRLs), Online Certificate Status
Protocol (OCSP), Self-signed, Third-party, Root of
trust, Certificate signing request (CSR) generation,
Wildcard)

Domain 2.0: Threats, Vulnerabilities, and Mitigations
2.3. Explain various types of vulnerabilities.

- Cryptographic

2.4. Given a scenario, analyze indicators of malicious
activity.

- Cryptographic attacks (Downgrade, Collision, Birthday)