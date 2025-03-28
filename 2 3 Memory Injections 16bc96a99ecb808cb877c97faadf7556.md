# 2.3 Memory Injections

Created time: 29 décembre 2024 18:34
Last edited by: OLB_
Last edited time: 13 mars 2025 19:54

- malware runs in memory
- memory contains running processes
    - dll
    - threads
    - buffers
    - memory management functions
- Memory Injection:
    - malware runs inside an existing process
    - hide the malware behind the process
    - take permission of the process (PrivEsc)
- DLL Injection
    - injection of DLL path
    - dll runs as part of the process
    - easy to implement