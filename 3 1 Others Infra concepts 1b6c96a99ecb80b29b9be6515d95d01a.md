# 3.1 Others Infra concepts

Created time: 14 mars 2025 17:12
Last edited by: OLB_
Last edited time: 4 avril 2025 18:39

### on-premises Vs cloud-based infra

- On-premises
    - full control on security
    - local team maintains availability
- Cloud Based
    - geographical dispersion (resilience)
    - availability and platform security is delegated

### Centralized Vs Decentralized Infra

- Centralized:
    - correlated alerts
    - consolidated logs
    - easy to maintain / update / monitor
    - Single point of failure !!
- Virtualization
    - run many OS in same physical Host
    - adds complexity, maintenance and overhead
    - relatively expensive
- Containerization
    - isolated apps
    - standardized unit of software for portability
- IoT - Internet of things
    - sensors
    - smart devices
    - wearable technology
    - a lot of security weakness !!
- Scada (Supervisory Control And Data Aquisition) systems
    - popular ICS (Industrial Control Systems)
    - manage power, manufacturing equipment …
    - requires extensive segmentation
    - there are remote telemetry units (RTUs) that collect data from
    sensors and programmable logic controllers (PLCs) that control and
    collect data from industrial devices like machines or robots. Data is
    sent to the system control and monitoring controls, allowing operators
    to see what is going on and to manage the SCADA system

![image.png](image%2037.png)

- RTOS (Real Time OS)
    - industrial equipment
    - military equipment
    - only one process / one goal for this kind of OS
- Embedded Systems
    - part of larger system
    - optimize for size and cost
- HA - High Availability
    - always on / available equipment
    - active / active configuration
    - higher costs