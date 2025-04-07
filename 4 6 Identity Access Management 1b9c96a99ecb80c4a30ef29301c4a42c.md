# 4.6 Identity Access Management

Created time: 17 mars 2025 19:22
Last edited by: OLB_
Last edited time: 5 avril 2025 16:40

- IAM
    - identity lifecycle management
        - provisioning / de-provisioning accounts
    - access control
        - permissions assignement
    - authentication and authorization
        - identity proofing
        - SSO
    - identity governance
    - Ldap a protocol of X.500 SPECIFICATION
    - X.500
        - (attributes) Distinguished names (CN=xx ,OU= xx , DC = xx ..)
        - Directory information tree
            - Root > Country > Organization (O) > Organization unit (OU) > Common Name (CN)
    - SAML
        - XML open standard for authentification
        - not really implemented for mobiles
        - common solution for federated environments
    - OAuth
        - authorization framework
        - not an indentification protocol (need to add OpenID)
        - OAuth provides a method for users to determine what information to provide to third-party applications and sites without sharing credentials
    - OpenID is an open standard for decentralized authentication
        - Relying parties (RPs or Service Provider SPs) redirect authentication requests to the IdP(Identity Provider) and then receive a response with an assertion that the user is who they claim to be due to
        successful authentication
    - SSO
        - Internet (based on OAuth + OpenID)
        - Internal (based on LDAP + Kerberos)
    - Federation
        - Authentication and Authorization (SSO) between two organization
        - share Authent. and Author. between 2 parties
    
    ![image.png](image%2050.png)