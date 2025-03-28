# 4.1 Application Security

Created time: 15 mars 2025 14:44
Last edited by: OLB_
Last edited time: 27 mars 2025 22:47

- Security as part of the SDLC - Software Development Life Cycle
    - planning
    - requirement
        - ! Security requirements !
    - design
        - ! Security architecture !
    - coding
        - best practice / secure coding (OWASP)
        - code review
        - unit test
        - SAST / DAST
        
        **OWASP** 
        
        <aside>
        👉
        
        Define Security Requirements Implement security
        throughout the development process.
        
        **Leverage Security Frameworks** and Libraries Preexisting
        security capabilities can make securing applications easier.
        
        **Secure Database Access Prebuild SQL queries** to prevent
        injection and configure databases for secure access.
        
        **Encode and Escape Data Remove special characters.**
        Validate All Inputs Treat user input as untrusted and filter
        appropriately.
        
        **Implement Digital Identity** Use multifactor authentication,
        secure password storage and recovery, and session handling.
        
        **Enforce Access Controls** Require all requests to go through
        access control checks, deny by default, and apply the principle of
        least privilege.
        
        **Protect Data Everywhere** Use encryption in transit and at
        rest.
        
        **Implement Security Logging** **and Monitoring** This helps
        detect problems and allows investigation after the fact.
        
        **Handle All Errors and Exceptions** Errors should not provide
        sensitive data, and applications should be tested to ensure that
        they handle problems gracefully.
        
        </aside>
        
    - Testing
        - UAT
    - training and transition
    - operations and maintenance
        - patching / updating
    - decommissioning
    
- Different environment
    - Development
    - Testing / Quality
    - Staging
    - Production
- Devops / DevSecOps
    - optimizing SDLC
    - include security in SDLC
    - CI /CD + continuous validation + continuous monitoring
    - 

**Application Security**

- TEST TEST TEST
- check input method
    - documentation
    - sanitization
    - fuzzing to test
- cookies
    - secure attribute set (httponly)
    - no sensitive data in cookies
- SAST
    - Static Application Security Testing
    - find SQLi , XSS, Buffer Overflow
- DAST
    - running application dynamic tests
- FUZZING
    - sending invalid or random data
- Code signing
    - developper sign code with his private key
    - developper public key is signed by a CA
- Sandboxing
- app monitoring (build in app)
    - audit log
    - view blocked request
    - anomaly detection