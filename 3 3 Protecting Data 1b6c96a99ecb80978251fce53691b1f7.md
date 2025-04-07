# 3.3 Protecting Data

Created time: 14 mars 2025 22:11
Last edited by: OLB_
Last edited time: 5 avril 2025 14:30

- Geographic restriction
    - IP subnet
    - GPS
    - WIFI localisation
    - Mobile provider
- Geofencing
    - access if the user is in a particular location
- Encryption
- Hashing / Fingerprint
- Obfuscation
- Masking
- Tokenization
    - with lookup table
- Segmentation / isolation
    - separate data in different network
        - network can still communicate with restriction ⇒ segmentation
        - network is completely cut off ⇒ isolation
    - sensitive data ⇒ additionnal security
- Access Restriction
    - Permissions based on Authentication / level of authorization
    - Geographic restriction (with geofencing)
- DLP based on pattern matching or watermark
- **Data Minimization**
    - Data minimization techniques seek to reduce risk by reducing the
    amount of sensitive information that we maintain on a regular basis
    - by deidentification (anonymisation)
    - by data obfuscation (can loss the original data !)
        - hashing / tokenization / masking
- Data purpose limitation
    - information should be used only for the purpose that it was originally
    collected and that was consented to by the data subjects
- Right to Be Forgotten
    - allows individuals to request the deletion
    of personal data about them under certain circumstances
- Data retention policy
    - Reducing the amount of data that you retain is a great way to
    minimize your security risk.