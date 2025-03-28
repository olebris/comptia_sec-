# 3.1 Cloud Infrastructure

Created time: 14 mars 2025 16:46
Last edited by: OLB_
Last edited time: 14 mars 2025 17:01

- responsability matrix

![image.png](image%2020.png)

- Hybrid cloud
    - complexity
    - authentificaation across platform
    - logs are diverse
    - data leak risk (lot of data in transit)
- Cloud Vendors - Third parties
    - vendor risk management policy is necessary
    - do vendor risk assessment
    - include them in  incident response
    - constant monitoring
- Infra as code IAC
    - describe infrastructure in a code
    - manage version of infrastructure like code version (modifications stored with GIT)
    - buid always the same infrastructure (like it is in the code)
- Serverless Architecture
    - FAAS - function as a service
    - code runs in a stateless container
    - easy to scale
- Microservices
    - replace monolithic app
    - use APIs
    - more scalable
    - more resilient
    - more secure (containment)