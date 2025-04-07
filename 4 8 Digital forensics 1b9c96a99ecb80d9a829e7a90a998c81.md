# 4.8 Digital forensics

Created time: 17 mars 2025 21:29
Last edited by: OLB_
Last edited time: 5 avril 2025 17:10

- Evidence collection after an incident
    - Exculpatory evidence (to prove innocence)
    - Inculpatory evidence (to prove guilt)
    - Documentary evidence (to support a definitive assertion)
    - Demonstrative evidence (to help non technical people)
- RFC 3227 : guidelines for evidence collection

### PROCESS: Acquisition, analysis, reporting

- Acquisition
    - legal hold : a legal notice that informs an organization that they must preserve data and
    records
    - E-discovery: process that allow each side of a legal case to obtain evidence from each other
        - e-discovery use EDRM model
            - information: control what data needs to be provided
            - identification of ESI (Electronically Stored Information)
            - preservation *(more challenging part)*
            - collection of ESI
            - processing (cleaning, formatting …)
            - review of data
            - analysis
            - production to provide the information to third parties
            - presentation for testimony in court
        
- Chain of custody
    - maintain integrity of data used for Forensic
    - Chain-of-custody forms are simple sign-off and documentation forms used each time the evidence is accessed / transferred (see eg. below)
    - use hash and digital signatures
    - avoid tampering
    - put a tag and catalog data
    
    ![image.png](image%2052.png)
    
- Acquisition
    - Extract from RAM, Firmware, OS files …
        - order of volatility
        
        ![image.png](image%2053.png)
        
    - collect and correlate data on different systems
    - Snapshot of virtual systems
    - collect Left behind artefacts (tmp files , recycle bin …)
    - analyse **slack space** (space left on disk where partially deleted files could be found)
        - a bit by bit copy must be made (w/ dd or FTK)
    - always compare hash between extracted data and original
    - always work in read-only without write permission (Write blocker)
- Preservation
    - isolate and protect the data
    - manipulate copies
    - work with live system (dont power off the system)
    - follow best practice to ensure admissibility of data in court
        - Evidence in court cases is typically legally admissible if it is offered to
        prove the facts of a case, and it does not violate the law
        - admissibility for digital forensics requires that the data be intact and unaltered and have provably remained unaltered before and during the forensic process
- Cloud Forensics
    - ensure you have “Right-to-audit clauses” in Cloud provider contracts
    - Regulatory requirements may vary depending on where the cloud service
    provider operates

### Forensics acquisition Tools

- dd / FTK imager/ WinHex for disk image
- volatility
- Wireshark (to analyse captured packets)
- Encase, Autopsy
- CFReDS (NIST) : data to train at forensic analysis (example: Rhino Hunt files)

- Forensic Report
    - for internal reporting (intelligence and counterintelligence)
    - for legal proceedings
    - summary information (investigation and findings)
    - overview of forensic process (tools, assumptions made, limitations)
    - details on findings for each device
    - conclusion (w/ recommendation if needed)