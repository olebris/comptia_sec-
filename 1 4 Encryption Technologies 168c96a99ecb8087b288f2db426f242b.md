# 1.4 Encryption Technologies

Created time: 26 décembre 2024 19:39
Last edited by: OLB_
Last edited time: 13 mars 2025 17:21

- TPM - Trusted Platform Module
    - Cryptographic hardware
        - key and random number generator
        - Persistent memory
            - store a unique key burned during manufacturing (trust/primary  key)
            - store encryption keys (bitlocker keys ..)
        - Password Protected
        - Resistant to bruteforce attack
    
    **⇒** Useful Key provider for **Disk Encryption** 
    

- HSM
    - Hardware Security Module
    - For datacenters
    - Installed in clusters
        - Secure key storage
        - perform fast encryption/decryption tasks
    
    ⇒ **PKI: Key and Certificate Storage**
    

- Key Management systems
    - Create, delete and rotate keys
    - Associate keys with servers / users / services
    - logs / reporting
    - Key rotation policy
    
    **⇒ WEB UI for Key management**
    
- Enclave
    - ZONE / AREA in Memory isolated from the main processor
    - can be hardware or software
    - has its own boot ROM
    - RAM data encryption
    - Monitor boot process
    - True random number generator
    
    ⇒ **Secure data in memory during crypto processing** 
    

![image.png](image%205.png)