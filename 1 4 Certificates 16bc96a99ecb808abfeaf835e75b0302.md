# 1.4 Certificates

Created time: 29 décembre 2024 16:07
Last edited by: OLB_
Last edited time: 28 mars 2025 16:36

- Certificate:
    - contains server public key + digital signature (from CA)
    - X.509 format
        - serial number
        - version
        - signature algorithm
        - issuer
        - validity
        - Common Name (CN)
        - public key
        - SANs (Subject Alternative Name) ⇒ OPTIONAL ! (ex IP,email, wildcards domains…)
- CA - certificate authority
    - real time verification (built-in inside browser)
    - verif. based on CA public key
    - Major CAs
    
    ```bash
    IdenTrust
    Amazon Web Services
    DigiCert Group
    Sectigo/Comodo
    Technet24
    GlobalSign
    Let's Encrypt
    GoDaddy
    ```
    
    - some CA are offline and delegate to “intermediate CA”
- RA _ Registration Authorithies
    - help CA to verify user identities
- Enrollment / Create certificate
    - create CSR
        - CSR = public key + informations on host
    - CSR validation and signature from CA = Signed Certificate
    
    ![image.png](image%2015.png)
    
- Wildcard Certificate
    - Subject alternative name (SAN) (extension of X.509)
    - one certificate for multiple domains
- CRL
    - List of revoked certificated provided by CA (link [http://xxxx.crl](http://xxxx.crl) inside certificate)
- OCSP
    - protocol to check in real time the status of one certificate (instead CRL whole  list)
    - occurs during TLS handshake
    - OCSP responder provided by CA

<aside>
👉

When you receive a digital certificate from someone with whom you
want to communicate, you verify the certificate by checking the CA's
digital signature using the CA's public key. Next, you must check and
ensure that the certificate was not revoked using a certificate
revocation list (CRL) or the Online Certificate Status Protocol (OCSP).
At this point, you may assume that the public key listed in the
certificate is authentic, provided that it satisfies the following
requirements:
- The digital signature of the CA is authentic.
- You trust the CA.
- The certificate is not listed on a CRL.
- The certificate actually contains the data you are trusting

</aside>

- Certificate pinning
    - certificate (public key) is attached to browser which verify this stored certificate with the server and alert if it doesn't match (kind of hard coded certificate…)
- Certificate Stapling
    - webserver contacts OSCP server itself and send a signed answer from OSCP to the client
- certifcates file format
    - .der .crt . cer (DER binary format)
    - .pem or .crt (Ascii format)
    - .pfx / .p12 for windows (bin)
    - .p7b for windows (ascii)