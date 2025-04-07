# 5.2 Recovery

Created time: 17 mars 2025 22:35
Last edited by: OLB_
Last edited time: 5 avril 2025 17:59

- RTO : objectif of recovery time after an incident (back to normal level of service)
- RPO: how much data is loss . Data loss aceptable
- MTTR : Mean time to repair / average time to fix an issue (measured)
- MTBF: Mean time between failures (measured) . Total uptime / nb of breakdowns
- MTTF : Mean time to failure (length of time before complete failure and replacement)

## Continuity of operations

- a design target for many organizations
- Add redundancy
    - power / network / hardware / software / sites
- Geographic dispersion
    - rule of thumb is to place datacenters at least 90 miles apart
    - Separation of servers and other devices in datacenters
        - placed in two or more racks in case of a
        single-point failure of a power distribution unit (PDU)
- Use of multiple network paths (multipath) solutions
- Redundant network devices / High Availability
    - Load balancing
        - redundancy
        - load management
        - patch / upgrade management
    - Clustering
        - redundancy through scale
        
        ![image.png](image%2046.png)
        
- Power
    - uninterruptible power supply (UPS) for battery
    - generator systems provide power for longer outages
    - dual-supply or multisupply hardware
    - Managed power distribution units (PDUs) (power remote control)
- Systems and storage redundancy
    - RAID
    
    ![image.png](image%2047.png)
    
    - Backups
        - full
        - incremental (changes since the last backup- faster to backup but slower to recover)
        - differential (changes since the last full backup- slower to backup but faster to recover)
    - Replication
        - synchronous or asynchronous methods to copy live data to another location or device
    - Journaling
        - mainly for database recovering to a point in time
    - Snapshots
- Platform diversity
    - diversity of technologies and vendors is another way to build resilience into an infrastructure
- HA Architecture
    - Availability
    - Resilience
    - Cost
    - Responsiveness
    - Scalability / Elasticity
    - Ease of deployment
    - Risk transference
    - Ease of recovery
    - Patch availability and vendor support
    - Power consumption
    - Compute requirements
- **Site restoration order**
    1. Restore network connectivity and a bastion or shell host.
    2. Restore network security devices (firewalls, IPS).
    3. Restore storage and database services.
    4. Restore critical operational servers.
    5. Restore logging and monitoring service.
    6. Restore other services as possible.

- Capacity Planning

<aside>
👉

Resilience requires capacity planning to ensure that capacity—including staff, technology, and infrastructure—is available when needed.

</aside>

- Areas of Capacity Planning
    - people
    - technology
    - infrastructure
- Testing Resilience and Recovery Controls and Designs
    - Tabletop exercises (discussions)
    - Simulation exercises
    - Parallel processing exercises (move processing to a hot site or alternate/backup system)
    - Failover exercises (full failover to an alternate site or system)